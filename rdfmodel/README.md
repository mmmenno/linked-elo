# RDF datamodel

## Beeldbank

Voor de beeldbank gebruiken we het Europeana Data Model (edm). Kort gezegd valt een beeldbankitem in dit model in twee delen uiteen: een `aggregation`, waarin gegevens zijn opgenomen over het geaggregeerde object (o.a. plaats waar metadatarecord en afbeelding te vinden zijn, de dataprovider en rechten) en daarnaast het metadatarecord zelf, met titel, beschrijving, maker, trefwoorden, etc.

```
<https://id.erfgoedleiden.nl/03f79efc-26bd-11e3-b4f6-3cd92befe4f8:aggregation>
	edm:aggregatedCHO elobb:03f79efc-26bd-11e3-b4f6-3cd92befe4f8 ;
	edm:isShownAt eloat:03f79efc-26bd-11e3-b4f6-3cd92befe4f8 ;
	edm:isShownBy <https://images.memorix.nl/lei/thumb/1000x1000/70b147bb-7375-cd33-40a7-b3d33bd2c897.jpg> ;
	edm:isShownBy <https://images.memorix.nl/lei/thumb/1000x1000/5d9861fe-793c-d790-e4ff-d0e40becc642.jpg> ;
	edm:dataProvider "Erfgoed Leiden" ;
	edm:provider "Erfgoed Leiden" ;
	a ore:Aggregation . 

elobb:03f79efc-26bd-11e3-b4f6-3cd92befe4f8
	dc:title "Station Loket van de NS" ;
	dc:description "Stationsplein 3J. Kantoor en loketruimten van de Nedrelandse Spoorwegen." ;
	dc:creator <https://id.erfgoedleiden.nl/person/7184a0aa-2744-11e3-abe3-3cd92befe4f8> ;
	sem:hasEarliestBeginTimeStamp "1987-01-01"^^xsd:date ;
	sem:hasLatestEndTimeStamp "1987-12-31"^^xsd:date ;
	dct:spatial wd:Q19546878 ;
	a edm:ProvidedCHO . 
```

## Personen en organisaties

```
<https://id.erfgoedleiden.nl/person/7184a0aa-2744-11e3-abe3-3cd92befe4f8>
  a schema:Person ;
  schema:gender schema:Male ;
  rdfs:label "Wim Lamboo" ;
  dc:description "fotograaf" ;
  owl:sameAs <http://www.wikidata.org/entity/Q96604134>, <https://rkd.nl/explore/artists/47600> ;
  schema:birthDate "1949"^^xsd:gYear .
```

## Gebeurtenissen

Op het moment zijn er nog geen gebeurtenissen opgenomen in de collectiedata (anders dan dat sommige afbeeldingen met het trefwoord 'gebeurtenissen' zijn getagd. Voor gebeurtenissen is het [Simple Event Model](https://semanticweb.cs.vu.nl/2009/11/sem/) een logische keuze. Door Wikidata identifiers te gebruiken voor typen gebeurtenissen, actoren en plaatsen verbinden we de gebeurtenis weer met een hoop andere gegevens.

```
eloevent:e5d7037b-7101-4d46-b4cb-45190ca0d596
	sem:eventType wd:Q3769366 ; 
	rdfs:label "Van der Werff biedt zijn degen aan het muitend volk" ; 
	sem:hasEarliestBeginTimeStamp "1574-01-01"^^xsd:date ;
	sem:hasLatestBeginTimeStamp "1574-12-31"^^xsd:date ;
	sem:hasEarliestEndTimeStamp "1574-01-01"^^xsd:date ;
	sem:hasLatestEndTimeStamp "1574-12-31"^^xsd:date ;
	sem:hasActor wd:Q2242334 ;
	sem:hasPlace wd:Q33456378 ;
	a sem:Event . 

wd:Q3769366 a sem:EventType . 
wd:Q2242334 a sem:Actor .
wd:Q33456378 a sem:Place .

elobb:151a9f1e-9fc9-64d4-4750-9236714cc81e dc:subject eloevent:e5d7037b-7101-4d46-b4cb-45190ca0d596 .
```