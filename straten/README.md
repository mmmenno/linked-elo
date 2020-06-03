# Straten

Op Wikidata zijn zo goed als alle straten binnen de gemeente Leiden te vinden. Ze zijn daar vrijwel allemaal van [BAG](https://nl.wikipedia.org/wiki/Basisregistratie_Adressen_en_Gebouwen) id en grotendeels ook van coördinaten voorzien.

Als collectie-items (via de interne locatiethesaurus bijvoorbeeld) met die Wikidata straten verbonden zijn, hebben we onder andere toegang tot vernoemingen, periode van bestaan en alternatieve straatnamen.

Vernoemingen en dateringen kunnen in Wikidata ook ingegeven worden. Op de kaart hieronder zie je dat er op moment van schrijven (mei 2020) nog geen enkele datering bekend is. Wel zijn er 163 vernoemingen bekend.

![kaart](imgs/stratenleiden.png)

De kaart toont bij aanvang van dit projectje (mei 2020) nog geen enkele datering en 163 vernoemingen. Je kunt [de kaartapplicatie bekijken](https://www.hicsuntleones.nl/straten/?gemeente=Q43631) om te zien wat de laatste stand van zaken is.

## Vernoemingen

Met de property `P138` (vernoemd naar) geef je aan waar een straat naar vernoemd is. Kijk bijvoorbeeld bij het [Amsterdamse Jofferpad](https://www.wikidata.org/wiki/Q18935260), daar zie je hoe die property gebruikt wordt om aan te geven dat de straat vernoemd is naar de [Amsterdamse Joffers](https://www.wikidata.org/wiki/Q3515741), een Nederlandse groep vrouwelijke kunstenaars in de 19e eeuw.

## Periode van bestaan

De datum waarop de fysieke straat is aangelegd geef je aan met de property `P571` (datum van oprichting of creatie). Mocht je een slag om de arm willen houden, dan kan je zo'n datum een precisie van een jaar, decennium, eeuw of desnoods een millenium meegeven. En vervolgens kan je met een 'qualifier' ook nog aangeven wat bijvoorbeeld binnen die eeuw de laatsmogelijke datum is. Handig als je niet precies weet wanneer een straat is aangelegd, maar wel een eerste vermelding hebt - zoals we bijvoorbeeld bij de [Oosterkerkstraat](https://www.wikidata.org/wiki/Q19395577) weten dat die in 1659 in een bron vermeld wordt als 'Kercsteech'.

Het is netjes om bij zo'n 'datum-van-oprichting-bewering' een bron te geven. Dat kan met `P248` ('vermeld in'). Het helpt als de bron al over een eigen Wikidata item beschikt - kandidaten zijn bijvoorbeeld:

- [Database Geschiedenis Leidse Straatnamen](https://www.wikidata.org/wiki/Q95992074), die te raadplegen is op [online.leiden.nl/straatnaam/](https://online.leiden.nl/straatnaam/)
- Het boekje [Gedemptegrachtenwandeling](https://www.wikidata.org/wiki/Q54925463)
- Het [Leids Jaarboekje](https://www.wikidata.org/wiki/Q2486316), waarbij je met een aparte qualifier ook aan kunt geven om welk deel het gaat
- 