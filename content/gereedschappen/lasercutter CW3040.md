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

## Software

### Lightburn

![Lightburn TkkrLab](/images/Lightburn_TkkrLab.png)

Als je Lightburn wil gebruiken op je eigen systeem, kun je de laser met USB aansluiten. Je kunt Lightburn eerst 30 dagen gratis gebruiken, hierna kun je het kopen voor €10 met kortingskode van het bestuur.

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

### Visicut


### Laser

Zet laser aan

Doe materiaal in laser en zorg dat bed op de goede hoogte is. Dit kun je zien doordat er op het materiaal 1 puntje van de focuslaser moet zijn. Zie je er meer dan 1 dan is je bed te hoog of laag.

Stuur je opdracht naar de laser. Blijf ALTIJD bij de laser!!!!! 

