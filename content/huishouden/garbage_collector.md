---
title: "Garbage collector"
date: 2019-11-02
weight: 30
---

Soms slingeren er objecten rond in de space die niet van iemand lijken te zijn maar ook niet meteen als afval bestempeld kunnen worden. Vaak zijn dit stukken van een oud of niet afgemaakt project waar niemand meer naar omkijkt. Omdat deze objecten vaak niet meteen als afval worden gezien blijven deze lang in de space rondslingeren.

De **garbage collector** is een bak voor dit soort spullen. Als je een object tegenkomt dat verwaarloosd lijkt te zijn of geen eigenaar heeft kan je deze in de garbage collector dumpen. Wanneer de garbage collector vol is mag deze geleegd worden. Op deze manier voorkomen we dat de space een dumpplek wordt voor willekeurige meuk. Als je je spullen niet opruimt loop je dus het risico dat het in de garbage collector belandt en daarmee het risico dat het in de vuilcontainer verdwijnt. Er is geen "grace period" voor de garbage collector, dus ruim je spullen op of check de garbage collector als je iets mist.

Voor iedereen die iets in de garbage collector wil stoppen: gebruik je gezonde verstand. Gooi niet lukraak alles wat je ziet liggen in de garbage collector. Om een idee te geven van objecten die bedoeld worden volgt hier een lijstje met objecten die in het verleden aangetroffen zijn:

* Een stuk afvoerpijp
* Lege gasfles
* Oude filmposters
* Houtplaten met verfvlekken
* Een of ander zelfgemaakt pluche beest wat heel lang op de keukenkast heeft gelegen
