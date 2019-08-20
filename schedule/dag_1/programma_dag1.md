# Workshop Data Scopes

Coherente methoden voor onderzoek met heterogene digitale bronnen

- Data scope: bijeen brengen van verschillende materialen en ze zodanig opschonen, aanvullen en verbinden zodat je bepaalde analyses kunt doen
    - Weinig consensus over hoe je dingen doet
    - Weinig begrip van hoe dit proces eruit ziet en hoe het vervolgstappen (e.g. analyse) beinvloed
    - Vaak onterecht gezien als voorbereiding op het "echte" onderzoek

## Doel workshop

Het doel is onderzoekers zich bewust te laten worden van de verschillende aspecten van de omgang met grootschalige data. Met data scopes willen we het volgende bereiken:

- **Inzicht in databewerkingsproces**: data verwerking is een essentieel en onlosmakelijk onderdeel van het onderzoek, en niet een noodzakelijk technisch proces waarna het echte onderzoek kan beginnen,
- **Transparantie van onderzoek**: zorgen voor meer transparantie bij de totstandkoming van onderzoek dat gebaseerd is op de verwerking en analyse van grote en complexe hoeveelheden data
- **Methodologische discussie**: consolideren van digitale methoden om te komen tot coherente en breed gedragen onderzoeksmethodologieën
- **Ontwikkelen van samenwerkingsvorm**: data bijeenbrengen, opschonen en koppelen vergt veel kennis, zowel technisch als inhoudelijk. Een goede manier om samen te werken en kennis te delen is essentieel.

## Opzet workshop

+ **Tutorial**: uitleg Data scopes concepten
+ **Hands**-on sessies: werken in kleine groepen aan opdrachten rondom Data scopes concepten
    + **wees creatief**: opdrachten hebben geen "correcte" oplossing, wij hebben de goede antwoorden ook niet
    + **zen**: het wordt een zootje, alles gaat mis, maar dat hoort erbij en alles komt ook weer goed
+ **Discussie**: vergelijken van groepsopdrachten, reflectie op Data scopes als handvat voor onderzoeksproces

## Programma


Vandaag:

+ 11:00-11:30 Workshop introductie
+ 11:30-12:00 Data Scopes achtergrond
+ 12:00-13:00 Hands-on sessie 1: greppen in TvG data
+ 13:00-13:30 Lunch
+ 14:00-16:00 Hands-on sessie 2: Frequentielijsten, namen en temporele expressies
+ 16:00-16:30 Bespreken van bevindingen, reflectie op Data Scopes

Rest van de maand:

- 09-09:
    - ochtend: Generale Missiven, vergelijken indices, linken en classificeren van trefwoorden
    - middag: Generale Missiven, vergelijken indices, linken en classificeren van trefwoorden
- 16-09:
    - ochtend: Biografisch Portaal
    - middag: werken met eigen data
- 23-09:
    - ochtend: werken met eigen data
    - middag: werken met eigen data
- 30-09:
    - ochtend: werken met eigen data
    - middag: bespreken van eigen werk, extra onderwerpen, discussie en evaluatie

## Introductie Data Scopes

[Data Scopes achtergrond](data_scopes_intro.md)

## Deelnemers

- Wat is je achtergrond? Wat is je ervaring met digitale methoden in onderzoek/data ontsluiting?
- Wat voor data gebruik je? Wat wil je ermee? Wat zijn eigenschappen?
- Waarom doe je mee? Wat zijn je verwachtingen?


## Deel 1

- vaardigheden:
    - grip krijgen op grote tekstbestanden met grotendeels onbekende inhoud en grote variatie
    - mogelijkheden om patronen te ontdekken
    - gestructureerd omgaan met ongestructureerde data
- Corpus: Tijdschrift voor Geschiedenis
- Voorbereidende stappen:
  - Open in een nieuw venster/tab en ga naar de [HuC Jupyter Hub](https://jupyterhub.diginfra.net) omgeving.
  - Login met je gebruikersnaam.
  - In het volgende scherm, klik rechtsboven op `New` en kies de optie `Terminal`. Dit opent een nieuwe browser tab met daarin een terminal window waarin je commando's kunt typen. 
  - Klik in het terminal scherm om de cursor te activeren en voer het volgende commando in: `/data/data_scopes_2019/setup_workshop_env.sh` (het is het makkelijkst om dit te knippen en plakken, want een typefout is snel gemaakt).
  - Klik rechtsboven op `Control Panel` en kies vervolgens voor `My Server`.
  - Je ziet nu als het goed is een lijst met bestanden waaronder `Data-Scopes-2019-Dag-1-Deel-1.ipynb`. Klik deze aan om de eerste opdracht te openen.


## Tijdschrift voor Geschiedenis (TvG)

- [Retrodigitalisering TvG](http://resources.huygens.knaw.nl/retroboeken/tvg/) online beschikbaar
- edities: 121 (1886-2008) 
    - teksten: 22,682 (artikelen, mededelingen, boekbesprekingen, ...)
    - pagina's: 60,751
    - Woorden - totaal = 30,861,146
    - Woorden - uniek = 932,766
- OCR data:
    - incompleet, ongestructureerde tekst, beperkte ontsluiting

## UNIX Command Line

- Exotische commando's en syntax:
    - grep, awk, sed, cat, tr, sort, uniq, cut, paste
- Waarom?
    - laat goed zien waar moeilijkheden met data interactie zitten
    - biedt natuurlijke methode voor transparant onderzoek
    - generieke toolset voor data exploratie en extractie
    - pipelines voor ketens van stappen


## Reguliere expressies
    - CTRL-F on steroids
    - voor patronen herkennen en transformeren

--

## Hoe hou ik bij wat ik gedaan heb?

- gebruik `history` commando
- kopieer commando's naar een bestand
- script: UNIX kan bestand met lijst van commando's uitvoeren (herhaalbaarheid)

- We claimen niet dat alle onderzoek voortaan via de command line moet!
    - maar het illustreert goed waar data scopes over gaat: transparent maken van het process

--

## Transparantie

Op welk detail niveau moet het process vastgelegd zijn voor transparantie?



