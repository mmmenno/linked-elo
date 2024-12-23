# Straten in Katwijk

Hier vind je (binnenkort) naamvarianten en schrijfwijzes van Katwijkse straatnamen, zoals die zijn aangetroffen in Katwijkse politierapporten uit de oorlogsjaren.

## Atlantikwall

In de oorlogsjaren is de hele Katwijkse kuststrook [gesloopt](https://katwijkinoorlog.nl/de-huizensloop-in-het-kustgebied/) om de Atlantikwall aan te leggen. Na de oorlog is het oorspronkelijke stratenplan deels teruggekomen, maar er zijn ook een aantal straten verdwenen. Het stratenplan van voor de sloop is [hier als geojson](atlantikwall-stratenplan.geojson) te vinden. Kopieer de geojson (bekijk 'code' of 'Raw') en plak in [geojson.io](https://geojson.io/) om ook de straatnamen te kunnen bekijken.

![Topotijdreis kaart](topotijdreis.jpg)

Het gearceerde deel op deze kaart, ook te bekijken op [Topotijdreis](https://topotijdreis.nl/kaart/1951/@87160,468830,10.94), is in de periode 1943-1944 gesloopt.

Dankzij een aantal kaarten, zoals die hieronder, die ik van het Katwijks Museum gemaild kreeg kon ik de ligging van de meeste van die straten achterhalen.

![Kaart met percelen](kaart2.jpg)

Deel van het gesloopte stuk van Katwijk. Bekijk voor de alle delen de kaarten [kaart 1](kaart1.jpg), [kaart 2](kaart2.jpg), [kaart 3](kaart3.jpg), [kaart 4](kaart4.jpg), [kaart 5](kaart5.jpg) in deze map.

## Verdwenen straten Katwijk

Verdwenen straten zijn zo goed mogelijk aan Wikidata toegevoegd. Op moment van schrijven zijn het 14 voor de Atlantikwall verdwenen straten en 2 straten die niet langer in de BAG voorkomen. Met [deze query](https://w.wiki/CV$o) krijg je de laatste stand van zaken er uit:

```
SELECT ?item ?itemLabel ?coords ?einddatum ?oorzaakLabel WHERE {
  ?item wdt:P31 wd:Q79007 .
  optional{
    ?item wdt:P770 ?oorzaak .
  }
  ?item wdt:P17 wd:Q55 .
  ?item wdt:P131 wd:Q208764 .
  ?item wdt:P625 ?coords .
  ?item wdt:P576 ?einddatum .
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],mul,en". }
}
```


