# Data Scopes workshop - opdracht levensverwachting

[Terug naar programma dag 3](README.md)

+ [Introductie](#intro)
    + [Data](#data)
+ [Opdracht](#opdracht)
	+ [stap1](#stap1)
	+ [stap2](#stap2)
	+ [stap3](#stap3)
	+ [stap4](#stap4)
+ [Extra](#extra)


<a href="intro"></a>
## Introductie

In deze opdracht gaan we ons bezig houden met meer gestructureerde data. Ze zijn verzameld voor een ander doel dan waarvoor wij ze gaan gebruiken en moeten daarom eerst worden geschoond en stapsgewijs verwerkt.

In de <a href="#opdracht">opdracht</a> hieronder zijn de stappen aangegeven, maar probeer zelf eerst een globaal plan te maken hoe je dit zou aanpakken. Lees eerst de vraag door en bekijk de data.


## Centrale vraag
Originele aanleiding: In “Er was iets met die schilders in de Gouden Eeuw” (NRC, 24-11-2011, pp.14-15) werden demografen Frans van Poppel, Dirk van de Kaa en Govert Bijwaard opgevoerd die op basis van de database van het Rijksbureau voor Kunsthistorische Documentatie (RKD Artists) stelden dat in de zeventiende eeuw schilders langer leefden dan aristocraten. **De vraag: is dat zo?**

__N.B.__ Het originele artikel staat voor de geïnteresseerden bij de data in de map _schildersGoudenEeuw_

**vraag**
Hoe ontwikkelde zich de levensduur in de loop der eeuwen?


## Data
Input is een dataset van personen uit het _Biografisch Portaal_. Die is niet helemaal up-to-date, maar dat is voor deze opdracht verder niet bezwaarlijk.

De data zijn op <a href="https://surfdrive.surf.nl/files/index.php/s/KJx9RfbPwSOeaj6">https://surfdrive.surf.nl/files/index.php/s/KJx9RfbPwSOeaj6</a> toegankelijk, als gezipt bestand onder de naam *datasets_dag4*.

<a href="#opdracht"></a>
## opdracht
_Wat moet je doen_
- Opschonen en verwerken van tabellarische data tot overzicht

- Beginnen met de bioport interface zelf?

<a href="#stap1"></a>
### stap 1:
de data zijn in csv formaat, en niet helemaal in bruikbare vorm

_Opschonen:_
+ omzetten getallen in tekstvorm naar echte getallen;
+ datetime getallen naar data;
+ Verwijderen nulls (dat is optisch, maar al die Nullen storen);
+ controle op importfouten

_Tools:_
+ Open Refine,
+ Spreadsheet (Excel, Libre Office, Google Spreadsheets),
+ programmatisch (bv Python Pandas).

*Let Op:* er zit een encoding probleem in ivm '_locale_' gekte van MySql. Open Refine importeert de dataset goed, andere programmatuur kan er niet goed mee overweg zonder nadere ingrepen. Kijk in hoeverre dit een probleem is

<a href="#stap2"></a>
### stap 2:
Selecteer data voor verdere bewerking
Voor lang niet alle personen zijn de benodigde gegevens compleet.

_Probleem_
+ Welke datum kiezen we
+ Wat te doen met overbodige gegevens (namen, extra datums,  geboorte-/sterfplaats)?

_Tools:_ idem als boven.

_Uitwerking_
Geboortejaar en sterfjaar zijn het meest compleet, dus geven meeste resultaten. Dat is wel minder precies, maar in dit geval te verkiezen boven minder data (die ook niet altijd exact zijn). We gaan ervan uit dat de afwijkingen in leeftijdsberekeningen elkaar uitmiddelen. Alleen personen met zowel geboorte- als sterfjaar doen mee. Neem ook degenen mee zonder sterfdatum , maar met een begraafdatum en eventueel degenen die wel een doopdatum hebben maar geen geboortedatum.

<a href="#stap3"></a>
### stap 3:
Maak een overzicht van de data

+ sterfjaar en geboortejaar van elkaar aftrekken. Voeg extra kolom toe.

+ maak draaitabellen van de spreadsheet. Dit gaat niet automatisch helemaal goed, want de draaitabellen:
  + groeperen naar ranges jaren, bijvoorbeeld per eeuw. Bedenk ook dat een tabel op een pagina moet passen!
  + Houd daarbij ook rekening met de evidente fouten die in het bestand zitten (weggooien !), want die vertekenen de uitkomsten. Er zijn waarschijnlijk nog meer fouten, door verkeerde invoer, bijvoorbeeld. Die zijn niet uit te filteren, maar ga ervan uit dat ze uitmiddelen. Voor de periode vóór 1500 wordt het aantal personen wel erg klein, wat doen we daarmee?
  + Het overzicht kan worden gemaakt voor het totaal aan data, maar voor een fijnmaziger verdeling kan ook gebruik worden gemaakt van de onderverdeling naar categorieën. Dit behoeft wel enige massage (samenvoegen categorieën, ordenen, weglaten als er te weinig data zijn)

<a href="#stap4"></a>
### stap 4:
analyseer de data:
welke conclusies kunnen we trekken tav van de vraag?

+ Welke kanttekeningen zijn er te zetten bij de conclusies?
+ Zijn er behalve de oorspronkelijke vraag nog andere conclusies?
+ Hoe representatief zijn deze data?


<a href="#extra"></a>
## Extra mogelijkheden:

**Extra mogelijkheden**: andere analyses die met de dataset zijn te maken.

Voorbeelden:
- Van wie zijn de exacte geboorte/sterfdata bekend? Wat kun je met onbekende geboorte/sterfdata??
- Vergelijk geboorte en sterfteplaatsen in de tijd en per groep. Laat ze op een kaart zien.
- Uitbreiden van de dataset met de dominees uit [Mining Ministers](https://github.com/cltl/Mining-Ministers ).
