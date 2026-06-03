
# imcm-mitschrift-1bhk-2

Das ist die README.md-Datei. md steht für Markdown. Markdown ist eine im Internet weit verbreitete Auszeichnungsspraceh(*Markup-Language*)
- Hypertext Markup Language (HTML)
- Extensible Markup Language (XML)
- Yet Another Markup Language (YAML, YML)

## Playlist zur Funktionsweise des Internets 

### Teil 1 - What is the Internet?
- wurde in den 1970er-Jahren erfunden
- Motivation: Schaffung eines dezentralen Netzwerks, das auch nach einem Atomschlag noch funktioniert (Kontext des kalten Krieges)
- Funktionsweise: Paketvermittlung (*Packet Switching*) - jedes Datenpaket sucht eine eigene Route durch das Netzwerk  
- Internet: das Netz der Netze - besteht aus vielen kleinen Netzen unterschiedlicher Internetanbieter (*Internet Service Provider - ISP*, z.B.: A1, Magenta, Salzburger AG, ...)


### Teil 2 - The Internet: Wires, Cables & Wifi

Informationen werden im Internet als Bits übertragen. Bits haben zwei Werte: 0 oder 1. 8 Bits ergeben 1 Byte. Mit einem Byte kann man 256 verschiedene Werte speichern (2^8 = 2 * 2 * 2 * 2 * 2 * 2 * 2 * 2).

Bits können über verschiedene Übertragungsmedien zwischen Computern versendet werden. Die Anzahl der übertragenen Bits pro Sekunde wird als Bandbreite bezeichnet - z.B.: 300MBits/s -> 300 Millionen Bitkönnen pro Sekunde über diese Leitung laufen.

1. Kupfer / Elektrizität
    - billig
    - einfach in der Verarbeitung
    - weit verbreitet
    - hohe Verlust über lange Distanzen (hunderte Meter)

2. Glasfaser / Licht 
    - schnelle Übertragung
    - verlustfrei
    - geeignet für Ozeankabel
    - teuer und Schwierig in der Verarbeitung

3. Funk / Radiowellen
    - hohe Verluste über Distanzen 
    - hoher Komfort, Internet überall
    - hohe Verluste über Distanzen
4. Daten, die über das Internet versendet werden, werden in Pakete aufgeteilt 
    - Pakete sind in der Regel rund 1500 Byte groß (=1.5 KB). das heißt, ein 10MB großes Foto würde in etwa 6667 Pakete aufgeteilt werden.(10MB = 10.000 KB = 10.000.000 Byte / 1500 Byte = 6667 Pakete)
    - Pakete können unterschiedliche Routen durch das Internet nehmen. Die Routenplanung erfolgt durch das Internet nehmen. Die Routenplanung
    erfolgt durch spezielle Computer sogenannten Router. Router entscheiden welchen Weg ein Paket durch das Internet nimmt. Die Entscheidung basiert auf verschiedene Faktoren, wie z.B. der akutellen Auslastung der Verbindung und der Entfernung zum Ziel.
    - jedes Paket enthält die IP-Adresse der Quelle und das Zieles sowie die Reihenfolge der Pakete(damit sie am Ziel wieder korrekt zusammengesetz werden können) 
    - am Ziel wird die Vollständigkeit der Pakete durch das *Transmission Control Protocol* (TCP) ünerprüft. Wenn Pakete verloren gehen, fordert TCP die erneute Übertragung an.
    - TCP und IP bilden gemeinsam die Basis für die Funktionsweise des Internets - man spricht auch vom TCP/IP-Modell

    ### Teil 3 - The Internet: HTTP and HTML

    - das *Hypertext Transfer Protocol* (HTTP) ist das Protokoll, das für dir Übertragung von Websiten verwendet wird
    - der Ablauf ist immer derselbe: 
    1. der Web-Client (Browser) schickt eine 
    HTTP-Anfrage (*Request*) an den Web-Server
    2. der Web-Server übernimmt die Anfrage, bearbeitet sie und schickt eine 
    HTTP-Antwort (*Response*) zurück an den Client. Dabei versieht er die Antwort mit einem [HTTP-Statuscode]
(https://de.wikipedia.org/wiki/HTTP-Statuscode). Diese sind in verschiedenen Klassen eingeteilt.
>[!NOTE]
>#### HTTP-Statuscode-Klassen
>
> - **1xx** - die Anfrage dauert nochan
> - **2xx** - die Anfrage war erfolgreich
> - **3xx** - Weiter- oder Umleitung
> - **4xx** - Clientfehler (z.B. 404- Not Found)
> - **5xx** - Serverfehler

- Daten (Websiten,Bilder,Videos usw...)  werden mittels GET-Anfragen angefordert  
- User-Input (Texteingaben,Dateinuploads, ...) werden mittels POST - Anfragen verschlüsselt übermittelt
- GET und POST sind sogenannte
**HTTP-Methoden**. Es gibt noch weitere Methoden, die wir erst später lernen.
- HTTP-Anfragen und Antworten können auch **Cookies** enthalten. Das sind kleine Textdateien, die aus Schüssel-Wert-Paaren (*key-value-pairs*) bestehen. Ist ein Cookie einmal gesetzt, wird es mit jeder Anfrage mitgesendet. So kann der Webserver einzelne User wiederkennen bzw. identifizieren.