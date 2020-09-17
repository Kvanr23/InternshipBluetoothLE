# InternshipBluetoothLE
Repository for everything about the internship, including issues and bugs


## Assignment Description
Crownstone

Crownstone, gevestigd in Rotterdam, Stationsplein 45 d1.118, https://crownstone.rocks, is fabrikant van slimme stekkers en connectoren (kroonsteentjes). Een Crownstone product is een 16A schakelaar, LED dimmer, vermogensmeter, soft-fuse, standby-killer en aanwezigheidssensor ineen. Unique selling point is de positiebepaling binnenshuis van smartphones en wearables dat het mogelijk maakt om volledig automatisch te reageren op de aanwezigheid, binnenkomst, of vertrek van een persoon. Direct kunnen lichten worden aangezet of energieverbruikende apparaten uitgezet. 

Onderwerp - Bluetooth Library

De Crownstone hardware kan worden bediend vanaf een smartphone. Echter, het gebruik van enkel een smartphone betekent: (1) niet schakelen op afstand, (2) geen continue opslag van het energieverbruik, en (3) lange round-trips via het internet. Hiervoor brengt Crownstone in 2020 een hub op de markt. De hub kan gebruik maken van een Crownstone USB stick om met Bluetooth Low Energy (Bluetooth LE) de Crownstones aan te sturen. 

Crownstone wil ook directe ondersteuning van Bluetooth LE aanbieden. Hiervoor moet een library worden ontwikkeld die geschikt is voor de Crownstone zelf en voor typische platformen die met home automation software (zoals Home Assistant) worden gebruikt. 

Wij willen graag een robuuste Bluetooth LE library voor Crownstones. We vermoeden dat de bluez libraries zelf robuust zijn en dat door het gebruik maken van een stabiele C library veel problematiek rondom het missen van notificaties, het niet kunnen verbinden, etc. wegvalt. 

Onderdelen van deze opdracht:

Het uitzoeken van het beste ontwerp voor de library, waaronder:
- bluez kernel/user space code, zie http://www.bluez.org/development/lists/
- stabiele C libraries, zie https://people.csail.mit.edu/albert/bluez-intro/c404.html
- python libraries, pybluez, bluepy, python-bluezero
- crownstone bluetooth lib
- Het volledig implementeren van de oplossing. 
  dit betreft het implementeren van de code in een nieuwe C library, of
  het forken van een bestaande python lib en deze grondig verbeteren;
  het schrijven van de wrappers om bovenstaande code aan te roepen.

- Het analyseren van de robuustheid van de library:
  + het meten van het aantal gedropte packets;
  + het meten van het aantal mislukte pogingen om een connectie te maken;
  
Het uiterst zorgvuldig documenteren van het gebruik van de code. Dit betreft duidelijk aangeven welke versie van bluez wordt ondersteund en alle noodzakelijke details rondom deployment op home automation platformen.

Eindresultaat:
Een robuuste Bluetooth LE library om Crownstones aan te spreken.

Benodigde ervaring:
 - Kennis en interesse in C/C++.
 - Kennis van Python.
 - Interesse in bluetooth en kennis over basis aspecten van het protocol.
 - In staat om technisch in het Engels te communiceren met domeinexperts.
 
 
