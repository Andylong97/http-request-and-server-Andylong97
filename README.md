Innlevering #1: HTTP Server
===========================

Oppgaven:
---------

Nesten alle utviklere jobber med HTTP til daglig.Den mest brukte versjonen av HTTP er definert i [RFC 7230](https://tools.ietf.org/html/rfc7230) mm. For at dere skal bli kjent med protokollen g�r innlevering #1 ut p� � lage en minimal implementasjon av protokollen.

Serveren skal bruke parametre fra requesten og svare tilsvarende. Dere kan benytte tjesten [URL Echo](http://ivanzuzak.info/urlecho/) som mal.

HTTP er definert som en request/response protokoll. Det vil si at en klient (typisk en nettleser) oppretter en forbindelse til en server og sender en request. Serveren svarer med en response. B�de requesten og responsen er tekst som sendes over nettverket. En typisk utveksling kan se slik ut (fra [RFC 7230](https://tools.ietf.org/html/rfc7230#section-2.1)):

Client request:

     GET /hello.txt HTTP/1.1
     User-Agent: curl/7.16.3 libcurl/7.16.3 OpenSSL/0.9.7l zlib/1.2.3
     Host: www.example.com
     Accept-Language: en, mi


Server response:

     HTTP/1.1 200 OK
     Date: Mon, 27 Jul 2009 12:28:53 GMT
     Server: Apache
     Last-Modified: Wed, 22 Jul 2009 19:15:56 GMT
     ETag: "34aa387-d-1568eb00"
     Accept-Ranges: bytes
     Content-Length: 51
     Vary: Accept-Encoding
     Content-Type: text/plain

     Hello World! My payload includes a trailing CRLF.  


Innleveringen:
--------------

Dere skal levere inn oppgaven i GitHub og jobbe parvis. Dersom du �nsker � v�re med � p�virke hvem du skal jobbe med, s� kan du [fylle ut dette sp�rreskjema](https://docs.google.com/forms/d/1ao3Is3_Or_Tku_77ZDjdr-Sr1O-0Ag7fsljYjKh7rFQ/prefill). Dere kan velge nye grupper til neste innlevering.

I tillegg til koden i GitHub skal dere ta opp en video p� 3-8 minutter der dere parprogrammerer litt kode. Screencast-o-matic anbefales som verkt�y for video-opptaket, men andre verkt�y kan benyttes. En lenke til videoen skal leveres � ikke videoen selv. Husk � �pne for tilgang til videoen (�unlisted� i Youtube).


Innholdet i oppgaven er definert i form at et sett med [GitHub issues](https://github.com/jhannes-playpen/innlevering-1-http/issues). Det er lurt � kopiere disse issues til deres eget kopi av prosjektet.




Vurderingskriterier:
--------------------

* Koden m� kompilerer og serveren m� la seg starte.
* README.md m� beskrive hvordan man starter opp serveren
* Det b�r v�re god testdekning p� koden
* Serveren b�r ikke krasje/falle ned av seg selv
* Klienten b�r koble seg fra korrekt
* Prosjektet b�r v�re dokumentert i form av README.md som ogs� b�r inneholde:
  * Hvordan man tester l�sningen
  * Kommentarer p� eget resultat. Hva kunne v�rt gjort bedre?
  * Eventuelle sp�rsm�l dere trenger svar p� for � komme videre.
* Koden b�r kunne h�ndtere funksjonalitet:
  * Forskjellige status codes
  * Forskjellige HTTP headere
  * Forskjellige HTTP bodies





