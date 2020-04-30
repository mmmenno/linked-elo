# Voornamen

Het bestand [givennames.csv](givennames.csv) bevat vrijwel alle voornamen die voorkomen in de volgende akten:

- doopakten van voor 1811
- trouwakten van voor 1811
- begraafakten van voor 1811
- geboortenakten Burgerlijke Stand na 1811
- huwelijksakten Burgerlijke Stand na 1811
- overlijdensakten Burgerlijke Stand na 1811

Alle (eerste) voornamen van gedateerde akten tussen 1500 en 2000 zijn meegenomen, al zijn er voor 1575 en na 1975 nauwelijks akten gevonden. De unieke namen zijn opgeslagen, waarbij bijgehouden is hoe vaak een naam voorkwam, hoe vaak een naam voorkwam als vrouwen- of mannennaam (als het geslacht bekend was, bijvoorbeeld omdat het een bruid of bruidegom betrof), hoe vaak een naam voorkwam in verschillende tijdvakken en in de verschillende bronnen.

Daarmee zijn al aardige lijstjes te maken, zoals bijvoorbeeld de populairste namen per tijdvak.

## Standaardiseren

De namen zijn zo goed mogelijk gestandaardiseerd naar een 'stamnaam' - Antony, Antonyus en Antoon, maar ook Antonnette, Antonyntgen en Antoonia zijn allemaal verbonden met de stam `antonius`. Om een idee te geven van de aantallen: met de stam `antonius` zijn meer dan 270 varianten verbonden.

## Het NAMES corpus

Bij het standaardiseren van de namen is zwaar geleund op het [NAMES corpus](https://www.clariah.nl/projecten/research-pilots/names/names#abstract) van o.a. Gerrit Bloothooft. Dat CLARIAH project heeft bijna 190.000 voornamen verzameld uit 19e-eeuwse akten zoals die op [wiewaswie.nl](https://www.wiewaswie.nl/) voorkwamen. Die voornamen zijn op een slimme manier geclusterd - gekeken is naar verschillende varianten/schrijfwijzes waarmee dezelfde persoon in verschillende akten werd aangeduid. Die automatisch tot stand gebrachte clusters zijn door experts bekeken en van standaarden voorzien, waarbij zij soms ook clusters aanpasten. De [handleiding bij het corpus](http://www.gerritbloothooft.nl/Publications/NAMES%20corpus%201.1%20manual.pdf) gaat daar dieper op in.

## Methode

In eerste instantie zijn de gevonden naamvarianten tegen het NAMES corpus gehouden en naar de daarbij vermelde standaard gestandaardiseerd. Daarbij is geen rekening gehouden met de verschillende waarschijnlijkheidsniveaus die het NAMES project hanteert.

De verwachting was dat de namen uit de Burgerlijke Stand goed te standaardiseren zouden zijn. Maar de vraag was in hoeverre het 19e-eeuwse NAMES corpus toepasbaar was op 16e, 17e en 18e-eeuwse Leidse namen.

Dat ging gelukkig redelijk goed. Van de eerste honderd meestvoorkomende namen in de trouwakten van voor 1811 konden zeven namen niet op die manier thuisgebracht worden.  Het zijn vooral de op '-gen' eindigende vrouwennamen die niet gevonden werden: Annetgen, Jannetge, Marytgen, Maertgen, Annetge, Maertge, Maycken.

De komende tijd wordt bekeken hoe we de namen verder kunnen standaardiseren. Dat kan scriptmatig (bijvoorbeeld '-gen' in nog niet gestandaardiseerde namen hierboven bij het zoeken vervangen door '-je'). Maar ook handmatig natuurlijk, al is het wel zaak daarbij de aantallen in het oog te houden.

## Aantallen

- in totaal zijn **5.382.891** voornaamvermeldingen gevonden
- uniek gemaakt zijn dat **53.820** voornamen
- daarvan konden er **22.430** m.b.v. NAMES gestandaardiseerd worden, dus dat is **41,6%**
- om op de eerdere vraag terug te komen hoeveel namen van voor 1811 met NAMES op te lossen zouden zijn: **15.300** van de  **39.880**, oftewel **38,3%** - niet zo heel veel slechter dus
- 41,6% lijkt weinig, maar het gaat dan wel om **5.020.071** voornaamvermeldingen, oftewel **93,3%** van het totaal aantal voornaamvermeldingen
- als je meegerekend hebt weet je dat er nog **31.390** namen niet gestandaardiseerd zijn
- maar er is een 'long tail' waar veel sporadisch voorkomende namen in zitten - als we ons beperken tot namen die vaker dan één keer voorkomen hoeven we er 'nog maar' **8.736** te standaardiseren
- en als we ons zouden beperken tot namen die vaker dan drie keer voorkomen moeten er nog **3.884** opgelost worden

## Wat kunnen we hier eigenlijk mee?

Op zich is het al leuk om te bekijken wanneer welke namen populair waren, en welke eigenlijk nooit. Als je graag origineel bent kan je die eens doornemen en je eerstvolgende Goletha, Benjamana, Crepijn, Godscalck, Zanderijntje, Baldinnus, Efjen, Ryckmoet, Widdeltje of Joleine noemen.

Maar je kunt er ook zoekfunctionaliteit mee verbeteren, door, als iemand op een specifieke naam zoekt, ook naar alle varianten op die naam te zoeken.

Persoonsvermeldingen waarvan je niet weet of het mannen of vrouwen betreft kan je met deze dataset in veel gevallen goed 'seksen'.

Er komen steeds meer transcripties beschikbaar van archiefmateriaal - door mensen maar steeds vaker ook door computers gemaakt. Als je bedenkt dat Transkribus binnen een seconde of dertig een hele pagina transcribeert, kun je je voorstellen dat dat de komende jaren snel kan gaan. Om die teksten betekenis te geven helpt het als algoritmes plaats- en persoonsnamen kunnen herkennen. Daar kan zo'n namenlijst goed bij helpen.

Als je, in persoonsreconstructies bijvoorbeeld, een gestandaardiseerde naam wilt gebruiken, dan kan je gewoon opzoeken welke variant het vaakst voorkomt bij een stamnaam. Nooit meer 'is het nou Jacob of Jacop' discussies. Het is 'Jacobus'. Dat wil zeggen, tot 1700 is het Jacob, en daarna Jacobus. Enfin.

En er zijn vast nog meer mogelijkheden te bedenken.
 
