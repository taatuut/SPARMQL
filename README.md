# SPARMQL

Emil  5:45 PM
Ik moet toch nog een side projectje starten: SPARMQL, volgens mij als ik json sem-achtige triples in MongoDB gooi en ze dan met compound indexes spo, pos en osp indexeer, MQL2SPARQL laagje maak, dan moet ik toch een heel eind komen...

Geert  5:58 PM
Hehe.. parsen van de query en de functies zijn ook een struikelblok..

Emil  5:59 PM
Hehe... daarom poneer ik het idee hier ook even..
6:00
En ik moet even nadenken wat ik me nog herinner van John Snelson zijn presentaties over de Triple Index, der zat nog een vierde component in de index, waarvan het an sich ook jammer was dat je die niet zelf in de triple (quad) kon adresseren.
6:01
Oh ja, voor de graph/name Collection, en daar zat beperking dat er triple maar bij een graph kan.
6:02
Maar je kan natuurlijk zelfde triple ook met meerdere graph labels inserten als je dat vierde veld in het document opneemt, en dan de indexen daarmee uitbreidt

Geert  6:02 PM
Dan kun jij dus beter doen...

Emil  6:02 PM
nog ff nadenken over bitemporal meteen

Geert  6:03 PM
Context van triples kwam van collection
6:03
Graph dus

Emil  6:03 PM
ja precies, maar dat werkt niet op vergelijkbare manier in MongoDB want daar is Collection 'fysieke scheiding'

Geert  6:03 PM
Bitemp moet kunnen, maar het afdwingen is lastiger..
6:04
Ja, zonde dat mongo die keuze gemaakt heeft. Erg beperkend..
6:04
Maar met extra veldje ben je er weer

Emil  6:05 PM
Ja de collection als label(s) in MarkLogic is wel lekker
6:05
precies

Geert  6:05 PM
Al eens envelope toegepast in mongo?

Emil  6:05 PM
nee, zou dat nuttige toevoeging zijn voor dit concept?
New

Geert  6:06 PM
Met zorba kun je trouwens xqy op mobgo doen dacht ik
6:06
Collection en timestamps in header
6:07
Triples in triples.. :sunglasses:

Emil  6:07 PM
Hop de repo is er https://github.com/taatuut/SPARMQL

Geert  6:07 PM
Lol
