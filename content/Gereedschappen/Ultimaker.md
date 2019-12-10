---
title: "Ultimaker"
date: 2019-11-15
weight: 10
---

De "Ultimaker" is een printer van Yvo de Haas, permanent in het gebruik van het Tkkrlab. De printer is in 2015 gekocht als een project van een maker die een Ultimaker 1 van de bronbestanden wou maken. Deze Ultimaker was mechanisch af, maar electrisch niet. De electronica is vervangen, en de Ultimaker is werkend gemaakt.

In de loop der jaren is de Ultimaker meerdere malen herbouwd. De extruder en hotend zijn vervangen voor 1.75mm versies, de electronica is vervangen nadat de RAMPS bijna in de brand vloog. Het bed is vervangen voor een verwarmd exemplaar. Het frame is nog steeds Ultimaker, maar alle andere hardware al lang niet meer. 

## Overview

 1. X-as
 2. Y-as
 3. Hot-end (E3D V6)
 4. Bowden buis
 5. Printbed (Z-as)
 6. Interface
 7. Encoder knop
 8. Licht schakelaar
 9. SD kaart
 10. Extruder
 11. Extruder release arm
 12. Hoofdschakelaar
 13. Spoelhouder
 
 ![Ultimaker](/images/Ultimaker_vooraanzicht.png)
 ![Ultimaker](/images/Ultimaker_achteraanzicht.png)  
 
## Specificaties
 * Afmetingen: 180x180x180mm (ongeveer)
 * Filament maat: 1.75mm
 * Nozzle grootte: 0.4mm
 * Verwarmd printbed: Ja (ca. 80C)
 * Controller: Megatronics V2 (of V3)
 * Firmware: Marlin 
 * voltage: 12V
 * Maximaal vermogen: 240W (of 360W)
 * Hot-end: E3D V6
 * Extruder: E3D Titan
 
## Interface

## Slicen

De Ultimaker draait op open source marlin en kan alle Gcode van standaard slicers aan (met als Gcode smaak Marlin). Dit kan worden gegenereerd door Cura, Slic3r, of elke andere slicer die deze smaak gcode kan genereren.

Standaard profielen op de PC naast de Ultimaker volgen nog.

## Printen

Printen met de Ultimaker gaat als volgt:

 1. Zet het te printen bestand op de SD kaart
 2. Laad het te printen bestand in de Ultimaker
 3. Doe met de lijmstift een dunne laag lijm op de plaats waar je gaat printen
 4. Selecteer uit het menu "Print from SD"
 5. Selecteer het bestand dat je wilt printen
 6. Terwijl de printer aan het voorverwarmen is, verwijder het lekkende filament dat onder de nozzle verschijnt
 7. Bevestig of de eerste laag goed vast zit
 
De printer zal nu zelf verder gaan. De printer geeft geen alarm als hij klaar is, maar op het scherm staat wel het huidige percentage van het bestand dat op dat moment geprint is.

## Materiaal laden / ontladen

Om het materiaal van de Ultimaker te vervangen moeten de volgende stappen doorlopen worden.

 1. Zet de printer aan
 2. Verwarm de nozzle voor in het menu
 3. Als de nozzle op temperatuur is, druk op de extruder release arm
 4. Duw eerst de filament naar voren zodat er wat plastic uit de nozzle komt, trek daarna de filament de extruder uit
 5. Indien er van kunststof soort gewisseld wordt, verwarm de nozzle naar de nieuwe temperatuur
 6. Knip een schuine kant op de voorkant van de nieuwe filament zodat deze beter door de buis gaat.
 7. Druk op de extruder release arm. Voer de filament nu van onderen in
 8. (Als de filament lastig gaat kun je de arm loslaten en aan het tandwiel draaien om de filament te forceren)
 9. Duw de filament door de extruder totdat er kunststof uit de nozzle komt
 10. (Als je van soort kunststof wisselt, duw dan minimaal 10cm filament door de nozzle om het oude kunststof weg te spoelen
 11. De printer is nu klaar om met de nieuwe filament te printen


## Onderhoud

Er zijn een aantal taken die zo nu en dan moeten gebeuren. Er wordt een poging gedaan om deze taken zo goed mogelijk te omschrijven. Als er toch enige onduidelijkheid bestaat over de precieze details van de taken, stop dan, en vraag iemand die het wel weet.

### Lijmstift vervangen

Om de print op het bed te laten hechten gebruiken wij een lijmstift. Deze kan op raken. Als dit het geval is licht er in de printerkast waarschijnlijk nog ergens een lijmstift. Als deze niet te vinden is, meld dit dan bij het bestuur zodat zij voor nieuwe lijmstift kunnen zorgen. Als tijdelijke oplossing kun je met een nat stukje papier het bed bevochtigen. Dit maakt de lijmlaag opnieuw actief. 

### Bed schoonmaken 

Omdat er steeds een nieuwe dunne laag lijm op het bed wordt aangebracht, kan het zijn dat de lijmlaag uiteindelijk te dik wordt. Dit geeft een onregelmatig ondervlak van de print en een dikke witte waas op het printbed. Voor het schoonmaken van het printbed heb je de volgende zaken nodig:

 * Schoonmaak papier
 * Stromend water
 * Een printer plamuurmes
 * Een prullenbak met ruimte

Om het bed schoon te maken doorloop je de volgende stappen:

 1. Om het werk gemakkelijker te maken kun je de glasplaat van de printer af halen. Breng deze naar een plek die vies mag worden.
 2. Pak 1 prop papier en maak deze nat onder de kraan. Pak een tweede prop en houd deze droog.
 3. Met het vochtige papier, veeg over het printbed zodat de lijm vloeibaar wordt.
 4. Steek nu met het plamuurmes de laag lijm van het printbed af. Je kunt het plamuurmes schoon vegen aan het droge stuk papier.
 5. Herhaal stap 3 en 4 totdat alle lijm van het printbed af is. 
 6. Als je klaar bent kun je het resterende water en lijmresten van het bed vegen met een droog stuk papier.
 7. Als het bed van de printer was gehaald kun je deze terug plaatsen.
 
Doordat de lijmlaag vrij dik kan opbouwen, kan het zijn dat hoogte van de eerste laag is veranderd. Als dit te erg is kan de stap "Hoogte printbed instellen en bed levelen" worden doorlopen.

### Hoogte printbed instellen en bed levelen

Printers kunnen in de loop der tijd hen calibratie verliezen. De ultimaker is helaas niet anders. Er kunnen twee dingen gebeuren die ongeveer de zelfde oplossing hebben. De hoogte van het bed kan verkeerd worden, en het bed kan niet meer level (Waterpas) zijn. 

Voordat je begint zijn twee dingen belangrijk. Als eerste moet je weten waarom het bed niet meer goed is. Als het probleem langzaam maar zeker zo gekomen is kun je verder gaan, maar als het bed van het ene op het andere moment niet meer goed staat zit er wellicht iets los. Daarnaast moet het glazen printbed zijn schoon gemaakt voordat de volgende stappen worden doorlopen.

Om de hoogte van de printer in te stellen:

 1. Pak een inbus schroevendraaier maat 2, en een stuk papier.
 2. Bevestig dat het bed schoon is, en maar weinig lijm bevat.
 3. Verwarm de nozzle voor op ca. 200 graden, en het printbed op 60 graden.
 4. Home de printer.
 5. Verplaats de printkop voorzichtig (!) naar het midden van het bed.
    (Het kan zijn dat de leveling niet goed is en dat de nozzle over het bed schraapt. Als dit zo is, houd meteen op!)
 6. Draai aan de 4 schroeven in de hoeken van het bed totdat het papiertje met lichte weerstand onder de nozzle kan bewegen. Draai elke schroef precies even veel.
 7. Om te bevestigen of het bed nog level is kun je (Wederom voorzichtig) de nozzle naar de 4 hoeken bewegen en met het papiertje testen of de nozzle op de juiste hoogte staat.
 
Als je concludeert dat het bed niet meer level is moeten de volgende stappen worden doorlopen:

 1. Pak een inbus schroevendraaier maat 2, en een voelermaat of stuk materiaal van ca. 0.5-1mm dik.
 2. Bevestig dat het bed schoon is, en maar weinig lijm bevat.
 3. Verwarm de nozzle voor op ca. 200 graden, en het printbed op 60 graden. 
 4. Beweeg met de hand het printbed naar een hoogte vlak boven (2-5mm) boven het printbed.
 5. Bevestig dat op alle plaatsen de printkop ongeveer even ver boven het bed zit.
 6. Verplaats de printkop naar een hoek van het printbed.
 7. Plaats de voelermaat onder de nozzle en schroef het bed omhoog of omlaag totdat de voelermaat lichte weerstand heeft. Vanaf nu mag je niet meer aan de hoofte van het printbed zitten.
 8. Verplaats de printkop naar een van de vier hoeken en herhaal stap 7 totdat je niet meer hoeft af te stellen in ELKE hoek.
 9. Verplaats de printkop nu naar het midden om te bevestigen dat de instelling klopt.
 10. Voer nu de hoogte calibratie uit om de bed hoogte opnieuw in te stellen.

## Indien kapot

Als er iets kapot is aan de Ultimaker, dan kun je dat melden aan Yvo de Haas. Hij kent de machine van binnen en van buiten. Bij gebrek aan Yvo kun je atijd het bestuur vragen.
