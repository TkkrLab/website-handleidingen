---
title: "Wijzigen website / project"
date: 2020-08-07
weight: 50
---

## Introductie

We gebruiken github als date opslag voor al onze webpagina's. Hierop worden de pagina's als .md bestanden opgeslagen en met hulp van hugo naar HTML vertaald. Dit laastste zou automagisch moeten gebeuren, jij hoeft alleen een wijziging op github puschen, de achterliggende systemen zorgen er voor dat het uiteindelijk op de site komt.


#### Github
Als je met github werkt heb je een lokale copie (stage omgeving) en natuurlijk de github repositry zelf. Je werkt altijd eerst op de stage omgeving voordat je iets publiceerd. Een aanpassing gebeurt daarom altijd in 2 stappen, eerst in je stage die dan ge-pushed word naar github.



## Benodigdheden
- [Git](https://github.com) of [Github Desktop](https://desktop.github.com/) (handig als je geen terminal wil gebruiken).
- [Hugo](https://gohugo.io/) (als je wil controleren of layout goed is)
- Je favoriete tekst editor (bv sublime, vi, vscode etc.)

## Stappenplan

Als voorbeeld gaan we de pagina die je nu ziet aanpassen. De repositry staat op [github](https://github.com/TkkrLab/website-handleidingen)

#### Maak een clone van de site die je wil wijzigen.


##### CLI

Open een terminal en geef het commando :
```bash
	cd $een_dir #ga naar een directorie waar je het terug kunt vinden
	git clone git@github.com:TkkrLab/website-handleidingen.git
```

##### Desktop
Of als je via de desktop wil werken kun je onder het groene knopje 'Code' de optie 'Open with Github Desktop' vinden, gebruik deze optie. Bij het clonen word gevraagd waar je het neer wil zetten, kies hiervoor een goede plek.

Je hebt de bestanden voor de site nu lokaal op je systeem staan.

#### Maak de gewensde wijziging

##### CLI

```bash
	cd website-handleidingen
	nano content/huishouden/wijzigen_stite_project.md #gebruik je eigen favoriet zoals vi of emacs.
```
##### Desktop

In de github desktop kun je via menu 'Repository' of een verkenner openen of een terminal. Open hier het bestand 'content/huishouden/wijzigen_stite_project.md' met je favoriete editor.



Wijzig het bestand en sla deze op. Eventueel controleer met hugo (met commando 'hugo server' start je een [local server](http://localserver:1313)) of het goed is.


#### Publish de wijzigingen naar github.

##### CLI

```bash
	git commit
	git push
```

##### Desktop

In de github desktop laat nu zien dat er wijzigenen zijn. Je kunt deze via de knop 'commit to master' links onderin klaar zetten om te publiceren. Met de 'push' optie word deze naar github gestuurd.


De wijziging staat nu op github, je hebt de pagina gewijzigd.

#### Controleer wijziging
De wijziging zou automatisch na 30 min op de site moeten staan. Als dit niet het geval is check met een van de bestuursleden.