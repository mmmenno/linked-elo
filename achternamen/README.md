# Achternamen

Het bestand [surnames.csv](surnames.csv) bevat vrijwel alle achternamen die voorkomen in de volgende akten:

- doopakten van voor 1811
- trouwakten van voor 1811
- begraafakten van voor 1811
- geboortenakten Burgerlijke Stand na 1811
- huwelijksakten Burgerlijke Stand na 1811
- overlijdensakten Burgerlijke Stand na 1811

Alle achternamen van gedateerde akten tussen 1500 en 2000 zijn meegenomen, al zijn er voor 1575 en na 1975 nauwelijks akten gevonden. De unieke namen zijn opgeslagen, waarbij bijgehouden is hoe vaak een naam voorkwam, hoe vaak een naam voorkwam bij vrouwen en mannen (toegegeven, wat minder relevant dan bij voornamen), hoe vaak een naam voorkwam in verschillende tijdvakken en in de verschillende bronnen.


## Standaardiseren

De namen zijn gestandaardiseerd naar de in het [NAMES corpus](https://www.clariah.nl/projecten/research-pilots/names/names#abstract) gebruikte standaard bij een specifieke naam. De [handleiding bij het corpus](http://www.gerritbloothooft.nl/Publications/NAMES%20corpus%201.1%20manual.pdf) gaat dieper in op de daarvoor gebruikte methode.

Het veld `standard` en `NAMES_standard` komen overeen. De waardes in het eerste veld kunnen worden aangevuld en aangepast - zolang dat in het tweede veld niet gebeurt is altijd te achterhalen waar een andere standaardisering wordt gebruikt dan in het NAMES corpus. 

De standaardisering moet niet gezien worden als etymologische herkomst, maar als een hulpmiddel, bijvoorbeeld bij het zoeken naar een persoon of verwanten in verschillende bronnen en in verschillende tijden.


## Aantallen

- in totaal zijn **4.877.523** achternaamvermeldingen gevonden
- uniek gemaakt zijn dat **278.922** achternamen, flink meer dus dan de 53.820 voornamen
- daarvan konden er **96.744** m.b.v. NAMES gestandaardiseerd worden, dus dat is **34,7%**
- 34,7% lijkt weinig, maar het gaat dan wel om **4.175.456** achternaamvermeldingen, oftewel **85,6%** van het totaal aantal achternaamvermeldingen
- als je meegerekend hebt weet je dat er nog **182.178** namen niet gestandaardiseerd zijn
- maar er is een 'long tail' waar veel sporadisch voorkomende namen in zitten - als we ons beperken tot namen die vaker dan één keer voorkomen hoeven we er 'nog maar' **76.655** te standaardiseren (namen die maar één keer voorkomen kunnen ook op transcriptie- of schrijffout duiden)
- en als we ons zouden beperken tot namen die vaker dan drie keer voorkomen moeten er nog **23.219** opgelost worden


## Wat kunnen we hier eigenlijk mee?

Aangezien het NAMES corpus vooral 19e-eeuwse namen uit heel Nederland bevat, zouden de daar niet gevonden, en in Leidse data veel voorkomende, achternaamvarianten specifiek moeten zijn voor de 17e en 18e eeuw en/of voor Leiden. Dit zijn de tien meest voorkomende namen zonder standaard:

1 Hennebo
2 Longepee
3 Melander
4 Vaa
5 Sauvage
6 Dusoswa
7 Charité
8 Verkinderen
9 Hasius
10 Verleus

Maar je kunt er ook zoekfunctionaliteit mee verbeteren, door, als iemand op een specifieke naam zoekt, ook naar alle varianten op die naam te zoeken.

De verschillende varianten bij een bepaalde standaard geven natuurlijk ook inzicht in veranderende spellingsgewoontes (tot 1725 kwam 'Backer' vaker voor, daarna 'Bakker') en een enkel geval van mogelijk snobisme ('Bacquers').

Er komen steeds meer transcripties beschikbaar van archiefmateriaal - door mensen maar steeds vaker ook door computers gemaakt. Als je bedenkt dat [Transkribus](https://transkribus.eu/Transkribus/) binnen een seconde of dertig een hele pagina transcribeert, kun je je voorstellen dat dat de komende jaren snel kan gaan. Om die teksten betekenis te geven helpt het als algoritmes plaats- en persoonsnamen kunnen herkennen. Daar kan zo'n namenlijst ook goed bij helpen.

En er zijn vast nog meer mogelijkheden te bedenken.
 
