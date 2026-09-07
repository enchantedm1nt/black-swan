+++
date = '2026-09-07T21:21:38+02:00'
draft = false
title = 'Weet de HvA wanneer je dood gaat?'
toc = false
tags = ["privacy"]
+++

Als je denkt dat een hogeschool slechts je tentamenresultaten en naam bijhoudt, dan heb je het toch echt bij het verkeerde eind. In deze blog geef ik een inkijkje in de data die de HvA van je verzamelt (en daarmee vermoedelijk een hoop andere educatieve instanties) op basis van documenten opgevraagd via een AVG-verzoek dat ik eerder dit jaar heb gedaan. Uit die documenten blijkt dat de HvA een indrukwekkende hoeveelheid data over je verzamelt, van je digitale voetafdruk tot een heuse overlijdensdatum voor het geval je bezwijkt onder de studiedruk.

## Van wie ben je, en wanneer ga je dood?
Al meteen in SIS wordt het interessant. Als student ken je dit misschien als website waar je cijfers op staan en je je studiezaken volgt, maar voor de HvA is het zowat een administratieve levenslijn. Behalve de verwachte zaken zoals je roepnaam, adres en studentnummer, wordt ook een hoop bureaucratisch pessimisme je kant op geslingerd. Het attribuut `usr_udf_DateDeath` is namelijk standaard aanwezig. De HvA merkt zelf vrij nuchter op dat het "niet erg waarschijnlijk is dat dit in een 'Nieuwe Student' situatie geleverd wordt", maar hij staat er wel lekker in.

Daarnaast wemelt het van de dubbele logica. Neem de e-mailadressen: een gotspe aan beslisbomen probeert je AMC-, privé- of home-e-mail uit Studielink te vissen om je maar te kunnen bereiken. Vervolgens geeft de HvA wel weer aan dat hun eigen logica door slordige AD-provisioning soms volkomen overbodig is.

## Brightspace en het internet. Alles wordt gemonitord.
Niet alleen 'simpele' administratieve gegevens zijn een gek rommeltje, ook je dagelijkse activiteit door de digitale leeromgeving (DLO/Brightspace) en het HvA-netwerk wordt minutieus bijgehouden.

Om te beginnen met Brightspace: niet alleen je cijfers en ingeleverde werken worden opgeslagen, maar ook je complete login-geschiedenis (wanneer/waar heb je ingelogd?), je IP-adres, pagina's die je hebt bezocht binnen Brightspace en eventuele discussiebijdragen.

Maak je gebruik van EduVPN of de wifi op de HvA? Dan wordt je gebruikers-ID, besturingssysteem en exacte verbindingstijden bijgehouden. Klinkt niet heel spectaculair, maar met wat kunst- en vliegwerk valt daar prima uit af te leiden wanneer je precies op de HvA bent geweest, als je wifi permanent aanstaat. Deze gegevens worden een jaar lang bewaard voor "troubleshooten en security incidenten". Bij de EduVPN geldt ook dat je netwerkverkeer niet wordt opgeslagen, maar wel onderhevig is aan netwerksensoren, firewalls en Netflow-analyses. Prima om je IP mee te verbergen, maar ik zou 'm niet als volwaardige VPN inzetten.

## Juridische rookgordijnen.
Zoals iedere instantie moet de HvA volgens de Algemene Verordening Gegevensbescherming (hierna: AVG) per stukje data kunnen uitleggen waarom ze dat gegeven bewaren, en voor hoe lang. Het valt daarbij op dat de beschrijvingen erg vaag kunnen zijn en breed leunen op algemene juridische prietpraat zoals het "algemeen belang" en "gerechtvaardigd belang". Daarmee timmeren ze op papier alles dicht, terwijl de praktijk waarschijnlijk heel anders loopt. Zo valt het op dat bij enkele attributen treffend wordt opgemerkt dat data "voorlopig niet leverbaar en dus ook geen waarde" bevat, of dat een specifieke notificatiestructuur "nog ter discussie" staat.
