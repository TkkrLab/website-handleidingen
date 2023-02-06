---
title: "Lasercutter CW3040 *OUD*"
date: 2020-06-10
weight: 999
---

## Laser is vervangen door [FabCreator](/gereedschappen/fabcore_lasercutter/)


![Lasercutter CW3040 TkkrLab](/images/TkkrLab_Laser_Cutter_CW3040.jpg)
De lasercutter van TkkrLab.

{{< youtube JtGMao8C_nw >}}


## Specificaties
 * Bed 30x40CM
 * Vermogen 40W
 * Smoothieboard als controller

## Mechanisch

### Onderdelen van de laser

De laser bestaat uit de volgende onderdelen:

 1. Schakelaar laser
 2. Laser veiligheid
 3. Laser interface
 4. Hoogte instelling
 5. PC (op de tafel)
 
![Lasercutter CW3040 TkkrLab](/images/Laser_overview.png)
 

### Laser veiligheid

![Lasercutter CW3040 TkkrLab](/images/TkkrLab_Laser_Safetycontr.jpg)

De laser veiligheidscontroller zorgt er voor dat de laser zich zelf niet kan slopen en veilig blijft. Deze controller controleert een aantal parameters om te bepalen of de laser aan mag staan. Wanneer de veiligheid de laser niet aan zet staat op het scherm waarom dit zo is. 

 * Er moet water stromen door de laser
 * Het water moet kouder zijn dan 40C (bij 30C verschijnt er een waarschuwing)
 * De laserdeur moet gesloten zijn

## Software

### Inkscape
Met [inkscape](http://inkscape.org/) (of ander vector teken programma) kun je een ontwerp maken voor de lasercutter. Als je ontwerp klaar hebt kun je deze opslaan als svg en in Lightburn importeren. Zet lettertypen om naar 'path', ander is de kans groot dat je de layout van je lettertype kwijt raakt.

Zie ook onze lasercutter workshop op [youtube](https://www.youtube.com/watch?v=JtGMao8C_nw)

### Lightburn

Lightburn is een veelzijdig programma dat de laser bestanden kan voorbereiden en de laser kan aansturen.

#### Lightburn op de PC van de laser

Lightburn staat geinstalleerd op de PC die bij de laser staat. Hier kan je met een USB stick de bestanden op de laptop zetten. 

Een gedetaileerde handleiding voor lightburn kun je (hier vinden)[https://lightburnsoftware.github.io/NewDocs/BeginnerWalkthrough.html]

Alle belangrijke menu's staan aan de rechter zijde. In 'Cuts / Layers' staan alle snedes voor elke kleur. De laser snijdt de lijst van boven naar onder. 'Library' bevat alle snedes voor alle materialen. Bij 'Laser' kun je met 'Frame' kijken waar de laser gaat snijden. 'Start' begint het snijden.

![Lightburn TkkrLab](/images/Lightburn_TkkrLab.png)

#### Lightburn op jouw eigen computer gebruiken

Als je Lightburn wil gebruiken op je eigen systeem, kun je de bestanden eerst op jouw eigen computer voorbereiden. Je kunt Lightburn eerst 30 dagen gratis gebruiken, hierna kun je het kopen voor $10 met kortingskode van het bestuur.

[Download](https://lightburnsoftware.com/pages/trial-version-try-before-you-buy) en installeer Lightburn op je systeem. Hierna kun je de TkkrLab laser aanmaken in Lightburn, start Lightburn op. 

Instellingen van de laser kun je <a href="https://handleidingen.tkkrlab.space/gereedschappen/cw3040.lbdev" download>hier</a> importeren.

Alternatief kun je het zelf handmatig aanmaken. Als er nog geen laser aangemaakt is gaat een wizard voor je de laser zoeken. 

Maak de volgende selecties:

 * Device is 'Smoothieware', selecteer 'Next'.
 * Verbinding via 'Serial/USB', selecteer 'Next'.
 * Geef de machine een naam, bv 'CW3040 TkkrLab'
 * Geef grote van het bed in, X 400mm en Y 300mm, selecteer 'Next'.
 * Geef origin in, dat is voor deze laser 'Rear Right', selecteer 'Next'.
 * Selecteer 'Finish'

Gefeliciteerd, je hebt de laser nu aangemaakt. Als je computer via USB aansluit aan de laser kun je deze gebruiken.

Natuurlijk is het ook handig om wat instellingen voor de materialen te hebben. Je kunt [deze library](/files/tkkrLab_lightburn.zip) gebruiken, zet deze ergens lokaal op je systeem. Via Library -> Load kun je dit bestand laden en gebruiken.

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
Gebruik van onderstaande materialen zou de laser kunnen beschadigen of geven een toxische gas. 

 * Chloor houdende materialen (PVC)
 * Teflon (PTFE)
 * Voor stempels : Rubber (er bestaat speciaal laser-rubber)

### Laser snijden

#### Laser starten

Je moet de werkplaats 'open' zetten, dit kan op de pads of de IoT schakelaar bij de ingang van de werkplaats. Zonder dit staat er geen stoom aan in de werkplaats.

Op de bovenzijde zit een zwarte drukknop die je uit moet trekken om de laser aan te zetten. Op de tafel staat een laptop die aangezet moet worden. De aan/uit knop van de PC zit aan de voorzijde. Houdt er rekening mee dat de PC circa 2 minuten nodig heeft om op te starten.

#### Bedhoogte instellen

De draaiknop op de voorkant van de laser wordt gebruikt om de hoogte van het bed in te stellen. Dit is belangrijk om de afstand van het brandpunt goed te krijgen. Onder het snijpunt staat een rode richtlaser. Wanneer de 2 lasers 1 punt vormen dan is de laser op de juiste afstand.

![Lasercutter CW3040 TkkrLab](/images/TkkrLab_Laser_spot_fout.jpg)

![Lasercutter CW3040 TkkrLab](/images/TkkrLab_Laser_spot_goed.jpg)

#### Snijden

Stuur je opdracht met 'START' naar de laser. Blijf ALTIJD bij de laser!!!!! 

#### Afsluiten

Om de laser af te sluiten kun je op de zwarte knop op de laser drukken. De schakelaar op de achterzijde hoeft niets uitgeschakeld te worden. De PC kan afgesloten worden. Nu kan de stroom met het stekkerblok van de laser gehaald worden.