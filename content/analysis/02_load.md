Load
=======================

I den här rapporten så skall jag jämföra 3 olika hemsidors laddningstid och eventuellt ge förslag på hur dom hade kunnat optimera sina hemsidor så dom laddar fortare.

Urval
-----------------------

Jag har valt att jämföra Surfline.com, Arbetsformedlingen.se och Smhi.se. Jag valde dessa 3 hemsidor för att det är hemsidor som jag använder mig utav och så vill jag även göra denna rapporten på hemsidor som inte liknar varanndra, i just den här rapporten så finner jag det intressantare.

Surfline.com är en community för surfare där man kan hitta allt från surf rapporter till alla möjliga artiklar som kan vara intressant om man surfar.

Arbetsformedlingen.se som är en svensk myndighetssida som fungerar som en plattform för folk som söker arbete och arbetsgivare. Jag tror att det är en hemsida som många är bekanta med i Sverige.

Smhi.se är Sveriges nationella meteorologiska institut som är en hemsida som tillhandahåller information om bl.a. vädret, främst i Sverige. Även detta en hemsida som jag tror många har besökt ett x antal gånger.

Metod
-----------------------

För att göra denna undersökningen så kommer jag att använda mig utav Pagespeed insights som är en hemsida som ger betyg på ens hemsida prestandaoptimering och ger en även förslag på vad som kan förbättras.

Google chrome kommer jag att använda som webbläsare när jag gör den här undersökningen. I devtools så kommer jag att jämföra laddningsvärderna från respektive hemsida.

Resultat
-----------------------
En snapshot från Surflines hemsida:

![snapshot](%base_url%/image/surfline.jpg "surfline"){.surflinebild}

Jag börjar med att välja ut 3 sidor i surfline som jag gör testen på, dessa sidor kommer jag att utgå ifrån när jag gör testerna.

Url,1:https://www.surfline.com/surf-reports-forecasts-cams

Url,2:https://www.surfline.com/surf-news

Url,3:https://www.surfline.com/travel

Jag börjar med att testa sidorna i pagespeed. Resultat från pagespeed:

Från första sidan: mobile, desktop

![snapshot](%base_url%/image/firsturlsurflinemobile.jpg "surfline"){.pagespeed}
![snapshot](%base_url%/image/firsturlsurflinedesktop.jpg "surfline"){.pagespeed}

Från andra sidan: mobile, desktop

![snapshot](%base_url%/image/2urlsurflinemobile.jpg "surfline"){.pagespeed}
![snapshot](%base_url%/image/2urlsurflinedesktop.jpg "surfline"){.pagespeed}

Från tredje sidan: mobile, desktop

![snapshot](%base_url%/image/3urlsurflinemobile.jpg "surfline"){.pagespeed}
![snapshot](%base_url%/image/3urlsurflinedesktop.jpg "surfline"){.pagespeed}

När jag går igenom resultaten ifrån pagespeed så kan jag se att Surfline hade kunnat optimera sin hemsida genom att ta bort mycket oanvänd javascript från sidan.

Längre ner på sidan syns resultaten från mina tester med devtools.

En snapshot från Arbetsförmedlingens hemsida:

![snapshot](%base_url%/image/ams.jpg "ams"){.surflinebild}

Jag kommer att göra undersökningen på dessa tre sidor:

Url,1: https://arbetsformedlingen.se/platsbanken/

Url,2: https://arbetsformedlingen.se/for-arbetssokande/mina-sidor

Url,3: https://arbetsformedlingen.se/for-arbetssokande/arbetslos---vad-hander-nu/skriv-in-dig

Resultat från sidornas pagespeed test:

Från första sidan: mobile, desktop

![snapshot](%base_url%/image/1amsmobile.jpg "ams"){.pagespeed}
![snapshot](%base_url%/image/1amsdesktop.jpg "ams"){.pagespeed}

Från andra sidan: mobile, desktop

![snapshot](%base_url%/image/2amsmobile.jpg "ams"){.pagespeed}
![snapshot](%base_url%/image/2amsdesktop.jpg "ams"){.pagespeed}

Från tredje sidan: mobile, desktop

![snapshot](%base_url%/image/3amsmobile.jpg "ams"){.pagespeed}
![snapshot](%base_url%/image/3amsdesktop.jpg "ams"){.pagespeed}

När jag analyserar resultaten från pagespeed så får jag som förslag "Eliminate render-blocking resources". För att förbättra arbetsförmedlingens sida så skulle jag se över deras css-filer och även javascript-filer, komprimera dessa filer så gott det går.

Längre ner på sidan syns resultaten från mina tester med devtools.

En snapshot från Smhi:s hemsida:

![snapshot](%base_url%/image/smhi.jpg "smhi"){.surflinebild}

Jag kommer att göra undersökningen på dessa tre sidor:

Url,1: https://www.smhi.se/q/Varberg/2664996

Url,2: https://www.smhi.se/vader/prognoser/ortsprognoser/q/Stockholm/2673730

Url,3: https://www.smhi.se/kunskapsbanken/klimat

Resultat från sidornas pagespeed test:

Från första sidan: mobile, desktop

![snapshot](%base_url%/image/1smhimobile.jpg "smhi"){.pagespeed}
![snapshot](%base_url%/image/1smhidesktop.jpg "smhi"){.pagespeed}

Från andra sidan: mobile, desktop

![snapshot](%base_url%/image/2smhimobile.jpg "smhi"){.pagespeed}
![snapshot](%base_url%/image/2smhidesktop.jpg "smhi"){.pagespeed}

Från tredje sidan: mobile, desktop

![snapshot](%base_url%/image/3smhimobile.jpg "smhi"){.pagespeed}
![snapshot](%base_url%/image/3smhidesktop.jpg "smhi"){.pagespeed}

När jag går igenom resultaten från pagespeed så får jag som förslag "Reduce unused JavaScript" för att förbättra smhis hemsida.

resultat från mina mätningar med devtools:

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTf6muDKRSACBB6FRMeRr_RzXr_a0FzSsdYSCQKFEqqNqcUJfNSZcgr19lSA__x6FSqaM-mFaloTbYY/pubhtml?widget=true&amp;headers=false"></iframe>

Notera tiden i Surflines test där jag har satt tiden till 1 min på grund av att laddningstiden hela tiden fortsatte.

Analys
-----------------------

När jag skall sammanfatta mina resultat från testerna jag har gjort så kan jag se att sidorna som jag har testat har fått liknande förbättringsförslag från pagespeed. Verktyget har gett analysen att samtliga sidor kan förbättra både sin användning av javascript och även CSS. Minska oanvänd javascript och CSS verkar vara något som många sidor därför borde ta en extra titt på för att förbättra laddningstiden.

Vinnare i testet.
-----------------------

För att utse en vinnare i mitt test så kommer jag endast att addera sidornas resultat. Summering av sidornas poäng ifrån pagespeed:

1.Surfline.com totalt 252p

2.Smhi.se totalt 216p

3.Arbetsformedlingen.se totalt 206p

Vinnaren, hemsidan som fick flest poäng var surfline. Lite förvånad är jag över resultatet då deras sida inte slutade ladda när jag testade sidorna i devtools men däremot så har dom en mycket mer dynamisk sida så jag antar att dom har gjort ett bättre jobb med att komprimera deras filer.

Gräns för absolut laddningstid
-----------------------

Jag tycker att en laddningstid runt 10 sekunder är en godkänd laddningstid för en sida, inte för långsamt men endå så att man hade kunnat förbättra något. En bra laddningstid skulle nog ligga runt 5 sek och om det är över 15 sek så bör man se över ens filer som sidan innehåller. Överlag så tycker jag att sidorna jag testade hade kunnat bli lite bättre men endå att dom klarade sig bra. Surfline var lite svårt att göra testet på eftersom att sidan hela tiden fortsatte att laddas.

Övrigt
-----------------------

Lucas Danielsson Valladares