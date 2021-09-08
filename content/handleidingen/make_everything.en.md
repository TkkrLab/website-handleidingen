---
title: "How to make (almost) everything"
date: 2021-01-01
weight: 20
---

Inspired by the fablab courses 'how to make (almost) everything', we give practical tips below on how you can use our equipment to make (almost) everything.

The objective is to indicate what you can do with the equipment and how you could use it. If you then get started with this, you can find more information in the information of the relevant device. Of course there is a lot of information on the internet and youtube, if there are good sources they will also be mentioned. If you don't know where to start, ask one of our participants, they can help you on your way.

Especially if you combine several of the techniques below, you can make almost anything you can think of.

For all the devices below, you must have a digital design to have it performed on the relevant machine. You could download a design or make it yourself.

At TkkrLab you can use the equipment for free as a participant, you can buy the consumables at cost price. You can also bring your own materials.


# 3d printing

 ![Hackerspace TkkrLab Prusa mini+](/images/prusa_mini_tkkrlab.jpg)

With a 3d printer you can make complex shapes with various plastic materials (PLA, PETG, ABS, TPU). For this you need a digital design (STL) that is sent to the 3d printer by means of a slicer.

For designing a digital design you can actually use any program that can export to STL. Some commonly used programs
* [TinkerCad](https://www.tinkercad.com/) : easy to use (digital block box), therefore also limited in terms of design options. Web based, free to use.
* [OpenSCAD](https://openscad.org/) : 'programming' objects by adding/subtracting basic shapes. Open Source.
* [Fusion 360](https://www.autodesk.com/products/fusion-360/personal) : Full CAD/CAM program, complex to use but endless possibilities. Free to use for hobbyists.
* [FreeCAD](https://www.freecadweb.org/) : Open source CAD program.
* [Blender](https://www.blender.org/) : More for organic modeling and animating video. Open source.
* [OnShape](https://www.onshape.com/en/) : online web CAD program, suitable for (complex) technical drawings.

After you have made a design you have to slice the STL to g-code ('translate' for the relevant 3d printer), for this you can use [PrusaSlicer](https://www.prusa3d.com/prusaslicer/) or [Cura] (https://ultimaker.com/software/ultimaker-cura). Both are open source and free to download. They also support various 3d printers (so you don't have to create a profile yourself).

The created g-code has to be printed by the printer as the last step, this is usually done by putting the g-code on an SD card and putting it in the 3d printer.

## Costs for participants
Price for PLA filament (various colours) per gram is € 0.04 . In your slicer you can see how many grams the printer needs.

## 3d printers at TkkrLab
* [Prusa Mini+](/tools/prusa-mini/)
* [Up Mini](/tools/up-mini/)

## Internet resources 3d printing
* [TkkrLab online workshop](https://www.youtube.com/watch?v=c420UUFpsl0) Explanation basic 3d printer and tinkercad (online 3D design program)
* [Thomas Sanladerer](https://www.youtube.com/watch?v=nb-Bzf4nQdE&list=PLDJMid0lOOYnkcFhz6rfQ6Uj8x7meNJJx) Basic workshop 3d printers / slicers
* [Thingiverse](https://www.thingiverse.com/) Download STL design, also good place for inspiration.

# Laser cutter

![Lasercutter CW3040 TkkrLab](/images/TkkrLab_Laser_Cutter_CW3040.jpg)

With a laser cutter you can cut very precisely in flat materials. The most commonly used material in lasercutters is plywood between 3-6mm thick or acrylic (also known as PPMA, plexiglass)

You also need a digital design for the laser cutter. For our laser cutter we work with Lightburn to control the laser, it can import svg, dfx, ai and other vector files.

You can therefore make your own design with a program that can save one of the above formats. Within TkkrLab we prefer to work with svg, because you can easily create a design for this with Inkscape.

You don't have to design everything yourself, for example boxes you have very good online box generators. You indicate the dimensions and with a few mouse clicks you have a basic design that you can adjust to your own liking.

#### Costs for participants
All our plates have the maximum size of the laser (30x40cm). First check whether we have the material you want to use in stock.
* plywood 3/4 mm - € 2.00
* transparent arcylate ( 2 mm - € 3.00 / 3mm - € 4.00 / 4mm - € 5.00 / black 2mm - € 3.00)

## Lasercutter at TkkrLab
* [CW3040 40Watt](/tools/lasercutter-cw3040/) 30x40cm 40Watt

## Internet sources lasercutter
* [TkkrLab online workshop](https://www.youtube.com/watch?v=JtGMao8C_nw)
* [Logos by Nick](https://www.youtube.com/channel/UCEQXp_fcqwPcqrzNtWJ1w9w)
* [Inkscape](https://inkscape.org/)
* [Lightburn](https://lightburnsoftware.com/) (free 30 day trial version)
* [Box.py box maker](https://festi.info/boxes.py/)
* [Kunstofplatenshop](https://kunststofplatenshop.nl/plexiglas-plaat/) webshop for acrylic sheets (cut to size).
* Overview available [lasercutters](http://www.chainlab.nl/) in Enschede.

# Foil Cutter

 ![Silhouette](/images/Silhouette-Cameo-3.jpg)

With a foil cutter you can make PVC sticker or t-shirt prints. For this you need an svg vector design that you can import on 'Silhouette Studio' and send to the foil cutter. You can also work with multiple colors by gluing the different layers together.

For the design itself you can use inkscape, see the explanation of the lasercutter for more information about inkscape.

## Foil cutter at TkkrLab
* [Silhouette Cameo 3](/tools/silhouette/)


# Arduino / Electronics

This is a very broad topic, to familiarize people with electronics and micro controllers we have developed our [arduino workshop](https://arduino.tkkrlab.space/). You will learn both the electronics part and the programming of the arduino.

The arduino is not only the electronics board but an entire ecosystem that now supports many different processors such as ESP8266, ESP32 and much more.

Once you have made an electronics design you would like to design a PCB so that you can place all the components on it. You can create a design with [KiCad](https://www.kicad.org/) (open source). Nowadays it has become so easy to send it in and have your design at home a few days later that we no longer etch / mill a PCB ourselves.

#### Costs for participants
You can borrow an Arduino for the workshop for free, there are no costs involved. If you want to use an Arduino or components in your own project, you will have to buy one yourself. An exception to this is for small components that we have in stock, which you can use for free.

## Internet Resources Arduino
* [TkkrLab workshop](https://arduino.tkkrlab.space/)
* [Arduino.cc](https://www.arduino.cc/)
* [Arduino sample projects](https://create.arduino.cc/projecthub/projects/tags/arduino)
* [Dutch Arduino forum](https://arduinoforum.nl)

# Computer programming
Programming is also an important part of being able to make something, even if you don't use a micro controller. You can use it to create your own applications or automate routine work. A little basic knowledge of what programming is and what you can do with it always comes in handy.

We are often asked what the 'best' programming language is to learn. The challenge is that every language has its own (optimal) application. For example, C/C++ is especially suitable for hardware control (eg Arduino & ESP), javascript for web applications, etc. That said, you could use python script for hardware control or vice versa C++ for a web application. That makes it a bit difficult to give a universal answer as to what the best language is, depending on your application.

If you don't know in which language you should start, we would advise phython. This is a versatile, modern language that you really can't go wrong with. It is available on many systems and also suitable for controlling various hardware (python script). All the concepts you learn here are also present in most other programming languages.

Below are some tutorial resources, if you get stuck with one of these tutorials there are plenty of participants at TkkrLab who could help you further.

### Programming Internet Resources
* [freecodecamp](https://www.freecodecamp.org/) Free tutorials.
* [Udemy](https://www.udemy.com/) Commercial provider of many training courses.

# CNC milling machine

![CNC](/images/Big_CNC_machine_Picture.jpg)

With the cnc you can remove material from a block of material until you are left with the desired shape. This is possible in both 2D and 3D plane, depending on your wishes and available materials.
Suitable for POM plastic, aluminum, wood and other (technical) materials that are not too hard.
Here too you have to make a digital design and send it to the cnc via gcode. Fusion 360 is suitable for this (the CAM module) to make g-code, with BCNC you can send it to the CNC.

## CNCs at TkkrLab
* [Small CNC](/tools/cnc_zen/) 7"x7"x2" inch
* [Large CNC](/tools/cnc/) 50x50x10cm 5400 rpm spindle