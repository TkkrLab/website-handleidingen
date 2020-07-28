---
title: "Lasercutter CW3040"
date: 2020-06-10
weight: 5
---

![Lasercutter CW3040 TkkrLab](/images/TkkrLab_Laser_Cutter_CW3040.jpeg)
De lasercutter van TkkrLab.
  
## Specificaties
 * Bed 30x40CM
 * Vermogen 40W
 * Smoothieboard als controller

## Mechanisch

### Onderdelen van de laser

De laser bestaat uit de volgende onderdelen:

 * Laser interface
 * Laser veiligheid
 * Afzuiging ventilator
 * Schakelaar laser
 * Laser bed
 * Laptop (aan/uit knop binnen in de laptop)
 * Laser kop
 * Richt laser
 

### Laser veiligheid

De laser veiligheidscontroller zorgt er voor dat de laser zich zelf niet kan slopen en veilig blijft. Deze controller controleert een aantal parameters om te bepalen of de laser aan mag staan. Wanneer de veiligheid de laser niet aan zet staat op het scherm waarom dit zo is.

 * Er moet water stromen door de laser
 * Het water moet kouder zijn dan 40C (bij 30C verschijnt er een waarschuwing)
 * De deur moet gesloten zijn

## Software

### Lightburn

Lightburn is een veelzijdig programma dat de laser bestanden kan voorbereiden en de laser kan aansturen.

#### Lightburn op de PC van de laser

Lightburn staat geinstalleerd op de laptop die bij de laser staat. Hier kan je met een USB stick de bestanden op de laptop zetten. 

Voor een gedetaileerde handleiding voor lightburn kun je op de onderstaande link klikken:
https://lightburnsoftware.github.io/NewDocs/BeginnerWalkthrough.html

Alle belangrijke menu's staan aan de rechter zijde. In 'Cuts / Layers' staan alle snedes voor elke kleur. De laser snijdt de lijst van boven naar onder. 'Library' bevat alle snedes voor alle materialen. Bij 'Laser' kun je met 'Frame' kijken waar de laser gaat snijden. 'Start' begint het snijden.

![Lightburn TkkrLab](/images/Lightburn_TkkrLab.png)

#### Lightburn op jouw eigen computer gebruiken

Als je Lightburn wil gebruiken op je eigen systeem, kun je de bestanden eerst op jouw eigen computer voorbereiden. Je kunt Lightburn eerst 30 dagen gratis gebruiken, hierna kun je het kopen voor €10 met kortingskode van het bestuur.

[Download](https://lightburnsoftware.com/pages/trial-version-try-before-you-buy) en installeer Lightburn op je systeem. Hierna kun je de TkkrLab laser aanmaken in Lightburn, start Lightburn op. Als er nog geen laser aangemaakt is gaat een wizard voor je de laser zoeken. 

Maak de volgende selecties :

 * Device is 'Smoothieware', selecteer 'Next'.
 * Verbinding via 'Serial/USB', selecteer 'Next'.
 * Geef de machine een naam, bv 'CW3040 TkkrLab'
 * Geef grote van het bed in, X 400mm en Y 300mm, selecteer 'Next'.
 * Geef origin in, dat is voor deze laser 'Rear Right', selecteer 'Next'.
 * Selecteer 'Finish'

Gefeliciteerd, je hebt de laser nu aangemaakt. Als je computer via USB aansluit aan de laser kun je deze gebruiken.

Natuurlijk is het ook handig om wat instellingen voor de materialen te hebben. Je kunt [deze library](/files/Tkkrlab.clb) gebruiken, zet deze ergens lokaal op je systeem. Via Library -> Load kun je dit bestand laden en gebruiken.

Mocht je een coplexe opdracht willen maken waarbij je veel verschillende instellingen wil gebruiken in 1 opdracht, gebruik [deze color pallet](/files/color_palette_lightburn.zip) in Inkscape met de gebruikte kleuren in Lightburn.

### Te snijden materialen

#### Wel

De laser kan de volgende materialen snijden:

 * Multiplex
 * Plexiglas (PMMA)

#### Niet

 * Chloor houdende materialen (PVC, bepaalde rubbers)
 * Teflon (PTFE)

### Laser snijden

#### Laser starten

Raam openen

Afzuiging ventilator op het raam

Schakelaar van de stekkerdoos inschakelen

Ventilator aan

Zwarte schakelaar schakelen

Laptop aan zetten (2 minuten opstarttijd)

#### Bedhoogte instellen

De draaiknop op de voorkant van de laser wordt gebruikt om de hoogte van het bed in te stellen. Dit is belangrijk om de afstand van het brandpunt goed te krijgen. Onder het snijpunt staat een rode richtlaser. Wanneer de 2 lasers 1 punt vormen dan is de laser op de juiste afstand.

#### Snijden

Stuur je opdracht naar de laser. Blijf ALTIJD bij de laser!!!!! 

#### Afsluiten

Laser met zwarte schakelaar uitzetten

Laptop afsluiten

Raam sluiten

Stroom van laser af



