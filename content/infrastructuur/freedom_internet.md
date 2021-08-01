---
title: "Freedom internet"
date: 2021-08-01
weight: 30
---

# Freedom internet for a hackerspace

[Freedom internet](https://freedom.nl/) (a hacker friendly ISP in The Netherlands) offered us a year of free internet.

This manual explains how we configured our own VDSL modem for pair-bonding and how we set up an OpenWRT router to make use of our internet connection.

## The modem

There doesn't seem to be a lot of affordable OpenWRT capable VDSL2 with pair-bonding routers available on the market.
Instead we started looking for an afforable VDSL2 modem which we could put in front of our existing OpenWRT router.

What we settled on is the [ZyXEL VMG4005-B50A](https://service-provider.zyxel.com/global/en/products/dsl-cpes/vdsl/residential-bonding-gateways/vmg4005-b-series) modem.

## Configuring the ZyXEL VMG4005-B50A

While the ZyXEL VMG4005-B50A can in theory be used as a router we want to configure it as a simple modem that converts the two pair-bonded VDSL2 lines into an
ethernet connection.

The end result of this configuration effort will be that you will have a modem of which the management interface is reachable on a static IP address while
internet access is provided to the OpenWRT router via a PPPoE tunnel.

### Getting initial access to the web interface

The web interface of the modem is by default available on [http://192.168.1.1](http://192.168.1.1) with username `admin`. The password is unique to your modem and can be found on the label on the bottom of the device.
Make sure the IP address of your computer is in the same range as the modem, for example you could configure your computer to have static IP address `192.168.1.2` with subnetmask `255.255.255.0`.

### Changing the password

Click on the burger menu on the top right and navigate to `Maintenance > User Account`. Here you can click on the edit button of the admin account to change it's password.

### Disabling the firewall and configuring management services

We're going to use this device as a simple modem. Because of this there is no need to run CPU intensive tasks like a firewall on this device, the OpenWRT router will take care of this instead.

Click on the burger menu on the top right and navigate to `Security > Firewall`. Now disable both the IPv4 and IPv6 firewalls and set the security level to low for both LAN to WAN and WAN to LAN.

Because we disabled the firewall it is a good idea to check which built-in services of the modem are exposed on which network interfaces. In the `Maintenance > Remote management` menu you can limit the management services of the
modem to be reachable only from the LAN connection. We recommend leaving only HTTP and HTTPS services enabled on only the LAN interface.

### Configuring the WAN interface

Go to `Network Setting > Broadband`. We configured the modem to have one broadband interface with the following settings:

- Name: Bridge_PTM
- Type: PTM
- Mode: Bridge
- Encapsulation: Bridge
- 802.1p: N/A
- 802.1q: N/A
- NAT: N
- Default Gateway: N
- IPv6: N

In the settings menu of the WAN interface this can be done by setting the mode to `Bridge` and disabling the `VLAN` option.

### Configuring the LAN interface

Go to `Network Setting > Home Networking`.

Configure the modem to have a static IP address in a range that is both private and outside of the subnet you use for your normal network.
At TkkrLab we use the `10.42.0.0/16` subnet for our normal network and `10.43.0.0/16` for devices we don't trust and want to keep separated from the internet.
Because of this we chose `10.44.1.1/24` for the modem. The `/x` notation indicates 

## The OpenWRT router

Our OpenWRT router is a [Ubiquiti EdgeRouter Lite](https://www.ui.com/edgemax/edgerouter-lite/), which can easily be converted into an OpenWRT router by
opening the case, removing the built-in SB drive which is plugged into the internal USB port and flashing OpenWRT to that USB drive.

### Configuring the PPPoE WAN interface

