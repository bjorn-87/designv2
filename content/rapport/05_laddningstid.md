---
---
Laddningstid Kmom5
=========================

I denna rapport har jag undersökt och dokumenterat laddningstiden för tre banker som finns i Sverige.

Urval
-----------------------

I Föregående rapporten om färgval och typsnitt så valde jag mellan banker eller E-handelsföretag.
Valet blev E-handelsföretag i den rapporten så då beslutade jag mig för att undersöka banker i denna rapport.

Valet hamnade på Nordea, Handelsbanken och swedbank då de var första bankerna som jag kom att tänka på.


Metod
-----------------------
Verktygen jag använt mig av är:

* Google Chrome
* [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* Devtools nätverkstest i chrome
* Google spreadsheets kalkylark

Började med att kolla sidornas prestanda i PageSpeed Insights och dokumenterade resultatet i ett kalkylark i google spreadsheets.
Efter det dokumenterade jag laddningstid, antal resurser och sidornas totala storlek med hjälp av devtools i Chrome.

Resultat
-----------------------
Resultaten finns dokumenterade i [Google spreadsheets](https://docs.google.com/spreadsheets/d/1cZ9frsecPxn3ipQTgv3oWlOsdXm_KT0Dh63dm20mGUY/edit?usp=sharing)  
######[Nordea](https://www.nordea.se)

Nordea var näst snabbaste sidan, både i pagespeed Insights och i mina egna tester.
Fick i Genomsnitt 90 poäng på Dator och 51 på mobil.
Genomsnittliga laddningstiden mätt i Devtools var 1.96s på dator och 5.6s på mobil.

[FIGURE src="image/nordeaStart.png?w=350" class="bank" caption="Bild på nordeas startsida"]

Några förslag på förbättringar var:

* Minifiera CSS.
* Ta bort oanvänd CSS.
* Skicka bilder i modernare format.
* Ta bort resurser som blockerar renderingen.



######[Handelsbanken](https://www.handelsbanken.se/sv/)

Handelsbanken var snabbast och fick bäst betyg i PageSpeed Insights både på dator och mobil.
Men var inte snabbast i mina egna tester.
Fick i genomsnitt 94 poäng på dator och 56 poäng på mobil.
Genomsnittliga laddningstiden mätt i Devtools var 2.35s på dator och 2.36s på mobil.

[FIGURE src="image/handelsbankenStart.png?w=350" class="bank" caption="Bild på Handelsbankens startsida"]

Förbättringsförslagen för Handelsbanken var liknande för alla tre sidor jag testade, vilka var:

* Skicka bilder i modernare format.
* Använd bilder med rätt storlek.
* Koda bilder effektivt.

######[Swedbank](https://www.swedbank.se/)

Swedbank fick sämst betyg enligt PageSpeed Insights men var snabbast enligt mina tester.
Fick i genomsnitt 79 poäng på dator och 29 poäng på mobil.
Genomsnittliga laddningstiden mätt i Devtools var 1.49s på dator och 1.58s på mobil.

[FIGURE src="image/swedbankStart.png?w=350" class="bank" caption="Bild på Swedbanks startsida"]

Några av förbättringsförslagen för Swedbank var:

* Aktivera textkomprimering.
* Ta bort resurser som blockerar renderingen.
* Ta bort oanvänd CSS.
* Skicka bilder i modernare format.
* Använd bilder mer rätt storlek.

Analys
-----------------------

Ingen av dessa sidor hade bra värden på mobil testerna. Vilket troligtvis beror på att de har fokuserat på Datorformatet och utvecklat appar till mobilerna.  
Gemensamt för alla tre var att de alla hade förbättringsförslag som innefattar bilderna på deras sidor, antingen att skicka dem i modernare format eller att använda bilder i rätt storlekar. Andra återkommande förbättringsförslag är att ta bort oanvänd CSS och minifiera CSS.
Det var intressant att se att Swedbank som jag upplevde som snabbast fick sämst betyg i PageSpeed insights.
När jag upptäckte detta så gjorde jag om mätningarna och såg då att det beror på att de hade längst fördröjning på "Tid till interaktivt tillstånd" vilket betyder att sidan verkat laddat in men försöker man göra något så händer inget.  
Det var även intressant att se att trots att Nordea använder sig av fler bilder än Handelsbanken så är totala storleken som laddas in mindre och deras sida laddas snabbare i mina tester med Devtools.

Av den anledningen vinner Nordea mitt test och rangordningen blir följande:

1. Nordea
2. Handelsbanken
3. Swedbank

Jag skulle säga att personligen så går min gräns vid 3 sekunder. Allt efter det känns långsamt.
Baserat på det så klarar alla dessa testet och känns rätt så snabba att klicka sig runt på.

Referenser
-----------------------

* [Nordea](https://www.komplett.se/)
* [Handelsbanken](https://www.netonnet.se/)
* [Swedbank](https://www.colorzilla.com/)
* [Full Page Screen Capture](https://gofullpage.com/)
* [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)

Övrigt
-----------------------

Denna rapport är skriven av Björn Olsson 2019-12-11.
