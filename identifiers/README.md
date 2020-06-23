# Identifiers

Om data goed met elkaar te kunnen verbinden hebben we goede identifiers nodig - om bruikbaar te zijn in zowel linked data als browsers in de vorm van een URI (Uniform Resource Identifier - niets meer dan een url die je gebruikt om iets mee te identificeren).

Veel externe terminologiebronnen beschikken al over URIs. De URI van het Wikidata-item over Janus Doesa is [http://www.wikidata.org/entity/Q1229819](http://www.wikidata.org/entity/Q1229819), de URI van molen De Valk in de BAG (Basisadministratie Adressen en Gebouwen) is [http://bag.basisregistraties.overheid.nl/bag/id/pand/0546100000044130](http://bag.basisregistraties.overheid.nl/bag/id/pand/0546100000044130), de URI van het concept houtskooltekeningen in de AAT (Artist & Architecture Thesaurus) is [http://vocab.getty.edu/aat/300390908](http://vocab.getty.edu/aat/300390908).

Vanzelfsprekend behoeft zo'n URI enige mate van persistentie. Samen een web van linked data bouwen lukt niet als URIs om de haverklap wijzigen of verdwijnen. Dingen voor 'de eeuwigheid' willen maken is hoogmoed, maar meerdere decennia - waarbij de URIs dus ook een nieuwe website of leverancierswissel van het collectieregistratiesysteem overleven - zou het streven toch wel moeten zijn.

Er zijn allerlei manieren en services om URIs te maken, Lukas Koster geeft daar in het artikel [Persistent identifiers for heritage objects](https://journal.code4lib.org/articles/14978) een goed overzicht van.

In principe hebben alle 'data-objecten' die binnen de ELO systemen leven en waar we naar willen kunnen verwijzen op termijn een URI nodig. In de opsomming hieronder staat de beeldbank bovenaan, maar ook over de rest van het lijstje zou dus al moeten worden nagedacht.

N.B. De URIs hieronder hebben de status van *voorstel*, er is dus nog *geen* definitief besluit genomen!

### De beeldbank

Het ligt voor de hand het uuid waarmee beeldbankrecords nu al geidentificeerd worden, en dat ook in de url van het beeldbankrecord zit, te gebruiken in de URI.

`https://id.erfgoedleiden.nl/03f74ad8-26bd-11e3-8cbd-3cd92befe4f8`

### Archiefbestanddelen

Ook de archiefbestanddelen hebben nu al een permalink met een uuid. dat van de volkstelling van 1581 is bijvoorbeeld [https://www.erfgoedleiden.nl/collecties/archieven/archievenoverzicht/file/e9903ed6b6113bfb8c29c6ec4c68fa49](https://www.erfgoedleiden.nl/collecties/archieven/archievenoverzicht/file/e9903ed6b6113bfb8c29c6ec4c68fa49). Ook hier zou je het uuid in de URI kunnen hergebruiken. In principe is een uuid wereldwijd uniek, dus je zou dezelfde URI kunnen gebruiken als bij de beeldbank. Om praktische redenen is het waarschijnlijk handiger een tussenvoegsel als `archivalrecord` op te nemen.

`https://id.erfgoedleiden.nl/archivalrecord/e9903ed6b6113bfb8c29c6ec4c68fa49`


### Scans

De volkstelling van 1581 bevat 279 scans, en een rechtstreekse verwijziging kunnen maken naar een specifieke scan is in veel gevallen handig.

`https://id.erfgoedleiden.nl/scan/580b1a99-e9dc-655e-1d3e-cc633f57431a`


### Referentiedata

Met de term 'referentiedata' wordt hier gedoeld op interne thesauri of lijsten waar beeldbankrecords of archiefbestanddelen mee verbonden zijn. Het gaat dan om personen, organisaties, locaties, trefwoorden, objecttypen en wellicht binnenkort ook gebeurtenissen. 

Alleen voor personen en organisaties worden nu al minstens drie lijsten gebruikt: vervaardigers, rechthebbenden en personen (als onderwerp). In het ideale geval worden die lijsten samengevoegd tot één lijst. Al die lijsten gebruiken uuids, wat integratie eenvoudiger maakt. Wel zullen er personen zijn die op meerdere lijsten voorkomen en samengevoegd moeten worden.

Behalve personen zouden ook organisaties opgenomen kunnen worden, denk bijvoorbeeld aan archiefvormers. Een mooi tussenvoegsel om zowel persoon als organisatie mee aan te duiden is lastig te vinden. Misschien moeten we, net als in zoveel andere systemen, gewoon doen alsof onze neus bloedt en het tussenvoegsel `person` gebruiken.

`https://id.erfgoedleiden.nl/person/b287c33c-2746-11e3-9d80-3cd92befe4f8`

Locaties zouden zoveel mogelijk rechtstreeks kunnen verwijzen naar Wikidata, GeoNames en BAG. Wellicht dat een eigen lijst met eigen identifiers helemaal niet nodig is.

Hetzelfde geldt voor objecttypen, daar zou de [AAT](http://vocab.getty.edu/aat) voor gebruikt kunnen worden.

De 'events' die als pilot binnen dit project gedefinieerd zijn hebben de volgende URI gekregen:

`https://id.erfgoedleiden.nl/event/e5d7037b-7101-4d46-b4cb-45190ca0d596`

