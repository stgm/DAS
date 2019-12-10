

## Opdracht B1A - Duidelijk Plotten

Installeer de volgende twee files in een werkfolder op de computer:

* [B1A_MooiPlotten.py](B1A_MooiPlotten.py)

* [B1_DatasetGenerator.py](B1_DatasetGenerator.py)

* [InlevertemplateBlok1.docx](InlevertemplateBlok1.docx)

Paar testjes [1] (InleverTemplateBlok1.pdf)


Lees het theorie blok ['Data visueel weergeven'](/blok-1/theorie-data-visueel-weergeven) en zorg dat je op alle punten let.<br>
Verander eerst in B1A_MooiPlotten.py je studentnummer.<br>
Verander nu de binning en de range van de plot net zo lang tot je een goed leesbaar histogram krijgt.<br>


Kopieer nu je histogram en je code op het inlever template voor Blok1. <br>
Is je iets opgevallen aan de distributie? - Schrijf dit dan ook op.

Let op! Je mag niet de automatische binning gebruiken van matplotlib.<br>
Je moet expliciet de bin en range opties gebruiken in je code.

## Opdracht B1B - Poisson Verdeling




## Opdracht B1C - Grote Aantallen

Installeer de volgende twee files in een werkfolder op de computer:

* [B1C_GroteAantallen.py](B1C_GroteAantallen.py)

Zorg dat dit bestand in dezelfde folder staat als de B1_DatasetGenerator.py file die je in opgave B1A al hebt gebruikt.


We voeren een experiment uit waarbij we zo goed mogelijk een meting willen doen van een of andere grootheid.
De waarnemingen die we doen varieren, we kunnen het niet exact meten of de onderliggende distributie heeft een onzekerheid.
De gemeten waarden zijn hierdoor Normaal ofwel Gaussisch verdeeld. 

Door het experiment een paar keer te herhalen kunnen we verbeteren.
We doen eerst een enkele meting. Hiervan kunnen we eigenlijk niet bepalen hoe representatief deze meting is. 
We doen daarom nog een meting. Nu kunnen we de resultaten van de twee metingen te combineren kunnen we voor het eerst een schatting doen van de onzekerheid op de gemeten waardes.


We herhalen het experiment daarom nog een paar keer en elke keer kijken we naar het gemiddelde van de metingen die we hebben gedaan.
Uiteindelijke kunnen we een de distributie van de metingen bekijken en bepalen wat de standaard deviatie is van de verdeling.
We nemen deze standaard deviatie als een maat voor de nauwkeurigheid van een enkele meting.

Doordat we nu eigenlijk heel veel metingen hebben genomen is de nauwkeurigheid op het gemiddelde, en zo de nauwkeurigheid van de grootheid die we wilden bepalen een heel stuk verbeterd.


De wet van de grote getallen zegt dat als we een verdeling hebben van random (stochastische) waardes, en deze verdeling een mathematisch goed gedefinieerd gemiddelde heeft, dat het gemiddelde van een steeds grotere dataset uiteindelijk convergeert. Dit betekend dus dat als de dataset aan de voorwaarde voldoet, we een steeds nauwkeuriger beeld hebben van wat het gemiddelde van de data is.


We gaan dit nu simuleren om een gevoel te krijgen hoe dit werkt. 


* In B1C_GroteAantallen.py bestand wordt de DatasetGenerator aangeroepen die een dataset voor je aanmaakt. (met ds.DataSetGroteAantallen() )
     * Laat zien dat de waardes in de dataset een Normaal verdeling volgen. 
     * Reken het gemiddelde en de standaard deviatie uit van de dataset. Gebruik hiervoor geen standaardfuncties, graag de formules coderen.
     * Representeer de dataset in een histogram. Zorg dat het histogram er netjes uitziet.

* We gaan nu simuleren dat we steeds meer datapunten hebben in onze dataset. We willen weten wat het gemiddelde is na $1, 2, 3 ... n$ metingen?
Hoe verandert het gevonden gemiddelde?
Zorg nu dat de code in het 'berekenGemiddelde' correct werkt. Als dit werkt zorg dan dat de code over de gehele dataset draait (en niet alleen over de eerste 4 punten).
  * Plot in een grafiek het gevonden gemiddelde versus het aantal waardes waarover dit gemiddelde is bepaald.

* Vergelijk je resultaten van de histogram en je grafiek. Is dit wat je verwacht hebt? 


Zorg dat je je histogram en je grafiek er goed uitzien. Volg de aanwijzingen in het blok ['Data visueel weergeven'](/blok-1/theorie-data-visueel-weergeven) en zorg dat je op alle punten let.<br>

Voeg je resultaten toe aan je inlever document.



## Opgave B1D - Plaatjes Verzamelen

Een bekende Nederlandse supermarkt geeft gratis kaartjes weg. Per 10 euro aan boodschappen krijg je 4 plaatjes.
Per pakje van 4 kaartjes zitten vier willekeurige plaatjes. De plaatjes komen dus niet in vaste combinaties per pakje voor. 
Er bestaan 160 identieke plaatjes.

Je probeert het boek compleet te krijgen.

Ga ervan uit dat de kansdichtheidsverdeling uniform is. Dus dat elk plaatje even veel kans heeft om in jouw pakje te zitten.


* Bereken de kans dat je een specifiek plaatje aantreft in je pakje.
  * Doe dit eerst met de aanname dat de vier plaatjes in je pakje eventueel ook dezelfde plaatjes kunnen zijn.
  * Bereken nu de kans als je ervanuit gaat dat per pakje je per definitie vier verschillende plaatjes kunt verwachten.
* Schrijf nu een simulatie waarbij je 1000 keer een pakje opent. Het pakje heeft vier verschillende plaatjes.
  * Maak een histogram die voor alle plaatjes het aantal getrokken kaartjes weergeeft. Ziet de distributie eruit zoals je verwacht had? Tip: Controlleer je resultaat door veel meer pakjes te openen en te controleren of je de verwachte distributie terug krijgt.
* Nu willen we weten hoeveel pakjes we gemiddeld nodig hebben om ons boek compleet te krijgen.
  * Schrijf eerst een functie die 1 vol boek simuleert, dus die door blijft gaan met pakjes openen tot het boek vol is. De functie hoort het aantal pakjes terug te geven.
  * Roep deze functie nu 10000 keer aan en maak een histogram met de resultaten (aan pakjes nodig).
  * Bereken uit dit histogram het gemiddelde aantal pakjes dat nodig is. 


Voeg je resultaten toe aan je inlever document