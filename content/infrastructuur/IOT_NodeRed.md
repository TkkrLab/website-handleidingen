---
title: "TkkrLab Domotica"
date: 2022-12-12
weight: 30
---

### !!! Warning !!!
We have a Node-RED server where all our home automation is controlled. The internal/tkkrlab links here only works if you are inside tkkrlab on de 'www.tkkrlab.nl' wifi.

You can use this and add new flows / logic to it. BUT :
#### If you break it, you fix it

So be a bit carefull with what you do. If you not sure ask one of the other TkkrLab members to help you out. 

# Introduction
This page is meant to give you a general technical overview of the components we use for our internal domotica / home automation system. 

We have alle the needed componend installed on a desktop server system, but you could also do this on a Raspberry Pi system.

## Node-RED server
The [Node-RED](https://nodered.org) system is the heart of the system, this glue all the parts together. You programm Node-RED with javascript nodes that you can connect via graphical UI.

Node-RED can also communicate to the outside world, so we implemented a telegram bot and our space open/closed [status](https://mapall.space/heatmap/show.php?id=TkkrLab). 

The TkkrLab Node-RED server lives on :  [TkkrLab Node-RED server](http://server:1880)

If you change a flow be sure to Deploy your changes to the server. Normaly it is suficient to only push your current flow. If you push 'Full' the system might need a hand to get started again.

For our internal dashboard you can go to [TkkrLab Node-RED Dashboard](http://server:1880/ui/#!/0?socketid=DyRk_4jKD1whv3agAAAD)


## Zigbee
We have around 22 Zigbee sensors, ranging from lamps, doorsensors, relay controllers,  buttons, tempature sensor and more. These are all connected to Zigbee.

We use a linux compatable Zigbee USB stick (Texas Instruments, Inc. CC2531 ZigBee) on our sever. If you want to create your own system use one on the recommended list from [Zigbee2MQTT](https://www.zigbee2mqtt.io/guide/adapters/#recommended). This USB sticks have to be updated with alternative firmware  'coordinator firmware'.

With the [Zigbee2mqtt](https://www.zigbee2mqtt.io/) software all the Zigbee messages are converted to MQTT messages and can be used by other software such as Node-RED.

For the zigbee configuration check out [TkkrLab Zigbee server](http://server:8124/)

## MQTT
For a MQTT system you need a 'broker', so the server component of the MQTT messaging system. Most popular is [mosquito](https://mosquitto.org). With a MQTT system you can subscribe to a channel (e.g. a device) and see all messages or send messages to this device.  

## WLED
For our ledlights we use [WLED](https://kno.wled.ge) connected to the MQTT broker.

For the WLED webpage go to [TkkrLab wled-kast](http://wled-kast.tkkrlab/).

# Implemented functions
So, what do we do with all these sensors and automation? We can add some inteliance to our space to automaticly do certain things.

Open/close space:
- Turn lights on/off: nanoleaf, LED strings
- Turn TV off
- Turn on/off thermostat
- Turn on vacuum cleaner when the space is closed
- Update status spaceapi and on Tkkrlab website

General :
- CO2 status with with waring if this becomes to high.
- Trash reminder every other week when spacedoor opens/closes. 
- LED matrix and fridge matrix (with Weather forecast, Newsfeed, Videos/GIFs and Prusa mini status)

Presentation room:
- Switch projector and input from 8 devices


Telegram:
- !who - opt-in list of who's in the space
- !f - send message to flipboard


# More info

* [Nodered getting started](https://nodered.org/docs/getting-started/)
