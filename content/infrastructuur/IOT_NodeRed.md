---
title: "Node Red"
date: 2022-12-12
weight: 30
---

We have a node-red server where all our home automation is controlled. The links here only works if you are inside tkkrlab on de 'www.tkkrlab.nl' wifi.

You can use this and add new flows / logic to it. BUT :
#### If you break it, you fix it

So be a bit carefull with what you do. If you not sure ask one of the other TkkrLab members to help you out.

## Node-red server
The nodered server lives on :  [Node-red TkkrLab server](http://server:1880)

If you change a flow be sure to Deploy your changes to the server. Normaly it is suficient to only push your current flow. If you push 'Full' the system might need a hand to get started again.

For our internal dashboard you can go to [Node-red Dashboard](http://server:1880/ui/#!/0?socketid=DyRk_4jKD1whv3agAAAD)


## Zigbee server
For the zigbee configuration check out [Zigbee server](http://server:8124/)


## MQTT
We use a lot of MQTT and Zigbee2MQTT to control our space. 

You can install ("mosquitto")[https://mosquitto.org] software to give commands on cli and subscribe to channels (to test).



# More general information on

* [Nodered getting started](https://nodered.org/docs/getting-started/)
* MQTT
* Zigbee