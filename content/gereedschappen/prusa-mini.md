---
title: "Prusa Mini+"
date: 2021-06-30
weight: 5
---

![Prusa Mini+](/images/prusa_mini_tkkrlab.jpg)

## Specificaties
 * Afmetingen: 180x180x180mm
 * Filament maat: 1.75mm
 * Materialen: PLA, PETG, ASA, ABS, Flex
 * Nozzle grootte: 0.4mm
 * Verwarmd printbed: Ja
 * Filement sensor : Ja

 Meer informatie over Prusa Mini+ op site van [prusa](https://www.prusa3d.com/original-prusa-mini/)

## Slicen

Het mooie van een Prusa printer is dat je de Prusa Slicer kunt gebruiken, hierin is de prusa mini al helemaal voorgedefinieerd en kun je deze meteen gebruiken. Je kunt de [Prusa Slicer hier downloaden](https://www.prusa3d.com/prusaslicer/), installeer deze op je eigen systeem. Als je het de eerste keer start zal die vragen welke printer je hebt, selecteer hier Prusa Mini.

Binnen de prusa slicer selecteer het object wat je wil printen. Je kunt verder de defaults aanhouden, dit zijn wel goede waarden. Indien je wilt kun je hiervan natuurlijk afwijken.

### Basis instelling voor slicen 

#### Print Settings
Dit is de 'kwaliteit' waarmee geprint word, deze staat default op 0,15 mm laaghoogte. Deze instelling beïnvloedt de print tijd aanzienlijk, als je een lagere kwaliteit instelt, bijvoorbeeld 0,2 of 0,3 mm dan is je print aanzienlijk sneller klaar. Dit zie je dan ook wel terug in de print, maar voor bijvoorbeeld functionele delen is de look een stuk minder belangrijk.

#### Filament
Het materiaal waarmee je print, dit zal vooral PLA zijn, maar kan ook een ander materiaal zijn. Prusa levert instellingen voor veel  materialen, deze kun je dan eenvoudig selecteren.

#### Supports
De meeste modellen kun je zonder support printen, vooral als deze speciaal voor FDM-printers zijn gemaakt. Mocht je toch support nodig hebben kun je de optie 'Support on build plate only' beste gebruiken.

#### Infill
Hoe solide de print gemaakt moet worden, default is 15%. Voor puur display-modellen zijn je tot 5-10% kunnen gaan, voor prints die heel stevig moeten zijn kun je tot 80-90% gaan, hoger geeft geen extra stevigheid. Ook dit heeft weer impact op je print tijd.

#### Brim
Een brim is een extra dikke rand rond het object zodat deze beter hecht. Normaal alleen nodig voor objecten met weinig oppervlakte op de 1e laag, bijvoorbeeld een holle cilinder.

In PrusaSlicer zijn er veel meer instellingen (in totaal iets van 400), deze hoef je normaal alleen te gebruiken als je een specifiek probleem wil oplossen. Als je in de slicer met de muis op de tekst van de instelling blijft staan geeft deze een korte uitleg met link naar uitgebreide tekst.

Als je alles goed hebt ingesteld kun je de code genereren met 'Export G-code' en naar USB schrijven.

## Printen op de Prusa Mini
Onze printers hebben een filament sensor, dus als filament op is stopt de printer en vraagt of je weer filament wil laden. 

### Schoon maken printplaat
Indien je print niet goed hecht kan het zijn dat de magnetische printplaat smerig/stoffig is. Maak deze schoon met een doekje met alchohol en probeer het opnieuw. Je hebt geen lijmstift of haarlak nodig om op de Prusa Mini.

### Filament laden
Als er nog geen filament inzit zal de printer vragen om filament te laden. Aan de rechter zijkant is een witte buis waarin je filament in moet doen.

Beging van het filament moet glad zijn, als er sliertjes of verdikking aan zit knip dit stukje af onder hoek van 45<sup>o</sup> met een zijkniptang. 

Druk filament in de buis tot die niet verder gaat. Geef op de printer aan dat filament geladen kan worden, deze zal dan vragen welk materiaal het is en opwarmen. Als de printer op temperatuur is gekomen zal de printer 'purgen' en vragen of het de juiste kleur is. Indien dit nog niet geval is geef dan 'No' tot die het wel goed heeft.

Als filament is geladen kun je de print gaan starten

### Printen G-code
Selecteer gcode model op Prusa Mini+ en 'print'. 

Als je een printopdracht in de printer aanzet is het verstandig om de eerste printlaag goed in de gaten te houden, als deze misgaat kun je het beste meteen opnieuw opstarten. Hierna is het verstandig om de print met 1 oog in de gaten houden (check iedere 30 min oid). Bij TkkrLab mag je niet de printer laten draaien als je niet meer aanwezig bent. Eventueel kun je iemand anderes vragen om je print in de gaten houden, dat moet je dan zelf met die persoon overleggen. Je kunt dus niet een opdracht aanzetten, weggaan en volgende dag ophalen.

## Ander materiaal laden
Via menu kies 'Change filament', de printer begeleid je dan door de stappen.