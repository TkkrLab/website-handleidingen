---
title: "Fabcreator Fabcore"
date: 2022-12-17
weight: 2
---

![Fabcreator Fabcore](/images/fabcreator_fabcore.png)


## Specificaties
 * Bed Afmetingen: 600x300mm
 * Vermogen buis: 40Watt

## Software

### Inkscape
Met [inkscape](http://inkscape.org/) (of ander vector teken programma) kun je een ontwerp maken voor de lasercutter. Als je ontwerp klaar hebt kun je deze opslaan als svg en in Lightburn importeren. Zet lettertypen om naar 'path', ander is de kans groot dat je de layout van je lettertype kwijt raakt.

{{< youtube JtGMao8C_nw >}}

### Lightburn

Lightburn is een veelzijdig programma dat de laser bestanden kan voorbereiden en de laser kan aansturen.

#### Lightburn op de PC van de laser

Lightburn staat geinstalleerd op de PC die bij de laser staat. Hier kan je met een USB stick de bestanden op de laptop zetten. 

Een gedetaileerde handleiding voor lightburn kun je [hier vinden](https://lightburnsoftware.github.io/NewDocs/BeginnerWalkthrough.html)

Alle belangrijke menu's staan aan de rechter zijde. In 'Cuts / Layers' staan alle snedes voor elke kleur. De laser snijdt de lijst van boven naar onder. 'Library' bevat alle snedes voor alle materialen. Bij 'Laser' kun je met 'Frame' kijken waar de laser gaat snijden. 'Start' begint het snijden.

### Camera in Lightburn




![Lightburn TkkrLab](/images/Lightburn_TkkrLab.png)

#### Lightburn op jouw eigen computer gebruiken

Als je Lightburn wil gebruiken op je eigen systeem, kun je de bestanden eerst op jouw eigen computer voorbereiden. Je kunt Lightburn eerst 30 dagen gratis gebruiken, hierna kun je het kopen voor $10 met kortingskode van het bestuur.

[Download](https://lightburnsoftware.com/pages/trial-version-try-before-you-buy) en installeer Lightburn op je systeem. Hierna kun je de TkkrLab laser aanmaken in Lightburn, start Lightburn op. 

Instellingen van de laser kun je <a href="TODO" download>hier</a> importeren.

Natuurlijk is het ook handig om wat instellingen voor de materialen te hebben zodat de preview tijden klopt. Je kunt [deze library](/files/tkkrLab_lightburn_fabcore.zip) gebruiken, zet deze ergens lokaal op je systeem. Via Library -> Load kun je dit bestand laden en gebruiken.

Mocht je een coplexe opdracht willen maken waarbij je veel verschillende instellingen wil gebruiken in 1 opdracht, gebruik [deze color pallet](/files/color_palette_lightburn.zip) in Inkscape met de gebruikte kleuren in Lightburn.

### Te snijden materialen

#### Wel

De laser kan de volgende materialen snijden:

 * Multiplex
 * MDF
 * Plexiglas (PMMA)
 * Karton/papier
 * Vilt

#### Niet
Gebruik van onderstaande materialen zou de laser kunnen beschadigen of geven een toxische gas. Als je niet weet welke materiaal het is deze ook niet gebruiken in de laser. 

 * Chloor houdende materialen (PVC)
 * ABS 
 * Teflon (PTFE)
 * Voor stempels : Rubber (er bestaat speciaal laser-rubber)

Check [Herkennen van (plastic) materiaal](https://hackaday.com/2015/03/14/how-to-identify-plastics-before-laser-cutting-them/) om te herkenen welk materiaal je gebruikt.

### Laser snijden

#### Laser starten

Je moet de werkplaats 'open' zetten, dit kan op de pads of de IoT schakelaar bij de ingang van de werkplaats. Zonder dit staat er geen stoom aan in de werkplaats.

Schakelaar om laser met koeler en compressor aanzetten.

Als je de laser echt gaat gebruiken de luchtpomp aanzetten. Na opdracht kun je deze weer uit zetten (ivm geluid).

Als het erg koud is in de werkplaats controleer dan of er condens op de buis zit. Je kunt de laser dan niet gebruiken ivm gevaar op kortsluiting in laserbuis.


#### Bedhoogte instellen

Leg de puck op het materiaal en verplaats de laser kop zodat deze boven de puck is. Schroef de kop voorzichtig los en laat het voorzichtig zakken zodat deze op de puck rust. Schroef de kop weer vast en verwijder de puck.

We hebben 2 nozzles voor de laser

* Snijden van <= 6 mm dikte met 1cm zwarte puck en lage nozzle. Dit zal voor de meeste materialen voldoende zijn.
* Snijden van > met 6mm dikte witte puck en hoge nozzle


#### Snijden

Zet op de laser de scakelaar met sleutel om zodat de laservoeding aan is. Controleer of luchtpomp, compressor en koeling aan is en de klep dicht zit. Het statuslampje zou nu groen moeten zijn hiermee is de laser klaar voor snijden. 

Als status lampje nog rood is doe dan even de klep open/dicht. Mocht die hierna nog rood blijven check dan of de randapparatuur goed is aangesloten.

Stuur je opdracht vanuit Lightburn met 'START' naar de laser. Blijf ALTIJD bij de laser!!!!! 

Als bij het snijden je werkstuk in brand vliegt druk dan de noodknop op de laser in. Dit is normaal genoeg om de brand te stoppen. Mocht het aanblijven doe de klep open en blaas het uit. We hebben ook een CO2 brandblusser bij de laser staan mocht dit allemaal niet helpen.

#### Afsluiten

Als je klaar bent met je opdracht zet de laser voeding uit met de sleutel. Als je helemaal klaar bent, zet de computer uit en haal schakelaar over voor lasercutter.

Maak het laserbed schoon en verwijder eventueele kleine stukjes uit het bed. Je kunt het rooster er uit halen en met stofzuiger alle kleine stukjes opzuigen.

# Nieuw Materiaal 
Als je een nieuw materiaal gebruikt die nog niet in de laser library staan zul je zelf de juiste instellingen moeten vinden. 

### Lightburn 'Material Test Generator' 
Hiermee kun je een matrix maken met instellingen voor snijden en/of graferen. Je zal normaal vooral met de instellingen voor 'speed' en 'power' willen testen, maar in de generator kun je ook 'interval' (voor graveren) en 'passes' testen.

Geef de waarden in die je wil testen en kijk met preview of dit is wat je wil gaan gebruiken.

Voor het snijden zoek je de waarde waarmee je net mee door het materiaal komt, met de minste power en hoogste snelheid. 

Maak voor de gevonden waarden een entry aan in de library en save deze. Zo kan de volgende gebruiker hiervan ook gebruik maken.



## Test type materiaal
Kijk of je op het materiaal een recycle icoon of driehoek met nummer in ziet staan. Als hier nummer 3 in staat is het PVC en niet geschikt voor de laser. Voor de andere getallen zie de [wikipedia artikel](https://en.wikipedia.org/wiki/Resin_identification_code).

Met een [Brand test](https://www.boedeker.com/Technical-Resources/Technical-Library/Plastic-Identification) kan men aan hand van de rook, geur en manier van branden veel plastics herkennen.

### PVC
Met [Beilstein test](https://en.wikipedia.org/wiki/Beilstein_test) kun je beoordelen of materiaal chloor bevat.

Other useful tests for discriminating plastics are the Beilstein copper wire test (which indicates the presence of chlorine, e.g. in PVC), susceptibility to acetone (most plastics besides polyethylene and polypropylene will become “tacky” on exposure), and whether the plastic turns white under stress, e.g. when bent (PVC whitens; PET does not).

# Onderhoud

Heb je het idee dat de laser niet meer met vol vermogen snijd/graveerd kan het zijn dat de spiegels vuil zijn. Deze moeten dan schoongemaakt worden, voor nu geef dit aan het bestuur aan. 

Filters zullen eens in de tijd vervangen moeten worden. (Hoe weten we dat het tijd is om filter te vervangen??)


### Externe links


* Handleiding [ENG](/files/FabCore_EN_Manual_V4.pdf) / [NL](/files/FabCore_NL_Handleiding_V4.pdf)
* [Hackaday lasercutter tips](https://hackaday.com/2016/05/31/how-to-fail-at-laser-cutting/)
* [Herkennen van (plastic) materiaal](https://hackaday.com/2015/03/14/how-to-identify-plastics-before-laser-cutting-them/)
* [Make: indentivying unknown plastics](https://makezine.com/article/science/identifying-unknown-plastics/)
* [Brand test](https://www.boedeker.com/Technical-Resources/Technical-Library/Plastic-Identification) 
