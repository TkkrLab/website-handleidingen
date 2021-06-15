---
title: "How to make (almost) everything"
date: 2021-01-01
weight: 20
---

Geïnspireerd op de fablab cursussen ‘how to make (almost) everything’ geven we hieronder praktische tips hoe je onze apparatuur kunt gebruiken om (bijna) alles te maken. 

De doelstelling is om aan te geven wat je met de apparatuur kunt doen en hoe je deze zou kunnen gebruiken. Als je dan hiermee aan de slag gaat kun je bij de informatie van het betreffende apparaat meer informatie vinden. Natuurlijk is er erg veel informatie op internet en youtube te vinden, indien er goede bronnen zijn zullen ze ook genoemd worden. Mocht je even niet weten waar je moet beginnen vraag dan een van onze deelnemers, die kunnen je vast op weg helpen.

Vooral als je meerdere van de onderstaande technieken combineert kunt je vrijwel alles maken wat je kunt bedenken.

# 3d printen

Met een 3d printer kun je eenmalige vormen maken met diverse plastic materialen (PLA, PETG, ABS, TPU). Hiervoor heb je een digitaal ontwerp nodig (STL) dat dmv een slicer naar de 3d printer gestuurd word. Kleinere aantallen kun je ook wel printen, maar hou er rekening mee dat 3d printen niet snel is.

Voor het ontwerpen van een digitaal ontwerp kun je eigenlijk elk programma gebruiken die kan exporteren naar STL. Enkele veel gebruikte programma’s
* [TinkerCad](https://www.tinkercad.com/) : eenvoudig in gebruik (digitale blokkendoos), hierdoor ook beperkt kwa ontwerp-mogelijkheden. Web based, gratis te gebruiken.
* [OpenSCAD](https://openscad.org/) : ‘programmeren’ van objecten dmv optellen/aftrekken basisvormen. Open Source.
* [Fusion 360](https://www.autodesk.com/products/fusion-360/personal) : Volledige CAD/CAM programma, complex in gebruik maar eindeloze mogelijkheden. Gratis te gebruiken voor hobbyisten.
* [FreeCAD](https://www.freecadweb.org/) : Open source CAD programma.
* [Blender](https://www.blender.org/) : Meer bedoeld voor organisch modelleren en animeren van video. Open source.
* [OnShape](https://www.onshape.com/en/) : online web CAD programma, geschikt voor (complex) technische tekeningen.

Nadat je een ontwerp heb gemaakt moet je de STL het slicen naar g-code, hiervoor kun je [Cura](https://ultimaker.com/software/ultimaker-cura) of [PrusaSlicer](https://www.prusa3d.com/prusaslicer/) gebruiken. Beide zijn open source en gratis te downloaden. Ze ondersteunen ook diverse 3d printers (zodat je niet zelf een profiel hoeft aan te maken).

De gemaakte g-code moet als laatste stop door de printer worden afgedrukt, dit gaat meestal dmv een SD kaart.

### 3d printers bij TkkrLab
* [Ultimaker original](/gereedschappen/ultimaker/)

## Internet bronnen
* [TkkrLab online workshop](https://www.youtube.com/watch?v=c420UUFpsl0)
* [Thomas Sanladerer](https://www.youtube.com/watch?v=nb-Bzf4nQdE&list=PLDJMid0lOOYnkcFhz6rfQ6Uj8x7meNJJx)

# Lasercutter

Met een lasercutter kun je heel precies snijden in vlakke materialen. Het meest gebruikte materiaal in lasercutter is triplex tussen de 3-5mm dik of acrylaat (ook bekend onder de naam PPMA, plexiglas)

Ook voor de lasercutter moet je een digitaal ontwerp hebben. Voor onze lasercutter werken we met Lightburn om de laser aan te sturen, deze kan svg, dfx, ai en andere vector bestanden importeren.

Om zelf een ontwerp te maken kan dus met een programma die een van de bovenstaande formats kan opslaan. Binnen TkkrLab werken we het liefst met svg, omdat je met Inkscape hiervoor eenvoudig een ontwerp kunt maken.

Je hoeft niet alles zelf te ontwerpen, voor bijvoorbeeld doosjes heb je hele goede box generators. Je geeft hierbij de maten aan en met een paar muisklikken heb je een basis ontwerp die je nog naar je eigen wensen kunt aanpassen.

## Lasercutter bij TkkrLab 
* [CW3040 40Watt](/gereedschappen/lasercutter-cw3040/)

### Internet bronnen 
* [TkkrLab online workshop](https://www.youtube.com/watch?v=JtGMao8C_nw)
* [Logo’s by Nick](https://www.youtube.com/channel/UCEQXp_fcqwPcqrzNtWJ1w9w)
* [Inkscape](https://inkscape.org/) 
* [Lightburn](https://lightburnsoftware.com/) (30 dagen test versie)
* [Box.py boxmaker](https://festi.info/boxes.py/)

# Arduino / Electronica 

Dit is een heel breed onderwerp, om mensen bekend te maken met electronica en micro controllers hebben we onze [arduino workshop](https://arduino.tkkrlab.space/) ontwikkeld. Hierbij leer je zowel het electronica gedeelte als het programmeren van de arduino.

De arduino is niet alleen de electronica board maar een heel ecosysteem dat inmiddels veel diverse processoren ondersteund zoals ESP8266, ESP32 en veel meer.

Als je eenmaal een electronica ontwerp heb gemaakt zou je een PCB willen ontwerpen zodat je hierop alle componenten kunt plaatsen. Je kunt een ontwerp maken met [KiCad](https://www.kicad.org/) (open source). Tegenwoordig is het zo makkelijk geworden om deze op te sturen en een paar dagen later je ontwerp thuis te hebben dat we zelf geen PCB meer etsen/frezen.

### Internet bronen
* [TkkrLab workshop](https://arduino.tkkrlab.space/)
* [Arduino.cc](https://www.arduino.cc/)
* [Nederlandstalige Arduino forum](https:/arduinoforum.nl)


# CNC 

Met de cnc kun je uit een blok materiaal materiaal verwijderen totdat je de gewenste form overhoud. Dit kan zowel in 2D als 3D vlak, afhankelijk van je wensen en beschikbare materialen.
Geschikt voor POM plastic, aluminium, hout, en andere (technische) materialen die niet te hard zijn.
Ook hier moet je een digitaal ontwerp maken en via gcode sturen naar de cnc. Hiervoor is Fusion 360 geschikt (de CAM module).

### CNC bij tkkrlab
* [CNC](/gereedschappen/cnc/)