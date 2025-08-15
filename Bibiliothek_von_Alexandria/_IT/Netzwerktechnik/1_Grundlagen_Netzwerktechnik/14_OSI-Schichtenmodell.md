>**Das wichtigste au einen Blick:**
><table>
>	<tr>
>		<th  style="vertical-align: middle; text-align: center;">OSI</th>
>		<th  style="vertical-align: middle; text-align: center;">Einordnung</th>
>		<th  style="vertical-align: middle; text-align: center;">DoD</th>
>		<th  style="vertical-align: middle; text-align: center;">Protokolle</th>
>		<th  style="vertical-align: middle; text-align: center;">Einheiten</th>
>		<th  style="vertical-align: middle; text-align: center;">Behandlung</th>
>		<th  style="vertical-align: middle; text-align: center;">Komponenten</th>
>	</tr>
>	<tr>
>		<td  style="vertical-align: middle; text-align: center;">Anwendung</td>
>		<td  rowspan="3" style="vertical-align: middle; text-align: center;">anwendungs-<br>bezogen</td>
>		<td rowspan="3" style="vertical-align: middle; text-align: center;">Anwendung</td>
>		<td rowspan="3" style="vertical-align: middle; text-align: center;">DNS <br>HTTP<br>SMTP<br>IMAP</td>
>		<td rowspan="3" style="vertical-align: middle; text-align: center;">Daten</td>
>		<td  style="vertical-align: middle; text-align: center;">Kapselung</td>
>		<td rowspan="4" style="vertical-align: middle; text-align: center;">Gateway<br>Server<br>Proxy</td>
>	</tr>
>	<tr>
>		<td  style="vertical-align: middle; text-align: center;">Darstellung</td>
>		<td  style="vertical-align: middle; text-align: center;">Codec<br>Dateiformat</td>
>	</tr>
>	<tr>
>		<td  style="vertical-align: middle; text-align: center;">Kommunikation</td>
>		<td  style="vertical-align: middle; text-align: center;">Verschlüsselung</td>
>	</tr>
>	<tr>
>		<td style="vertical-align: middle; text-align: center;">Transport</td>
>		<td rowspan="4"  style="vertical-align: middle; text-align: center;">übertragungs-<br>bezogene und<br>transport-<br>orientiert</td>
>		<td  style="vertical-align: middle; text-align: center;">Transport</td>
>		<td  style="vertical-align: middle; text-align: center;">TCP<br>UDP</td>
>		<td  style="vertical-align: middle; text-align: center;">Segment (TCP)<br>Datagram (UPD)</td>
>		<td></td>
>	</tr>
>	<tr>
>		<td  style="vertical-align: middle; text-align: center;">Vermittlung</td>
>		<td  style="vertical-align: middle; text-align: center;">Internet</td>
>		<td  style="vertical-align: middle; text-align: center;">IPv4<br>IPv6</td>
>		<td  style="vertical-align: middle; text-align: center;">Datagram</td>
>		<td></td>
>		<td  style="vertical-align: middle; text-align: center;">Router<br>L3-Switch</td>
>	</tr>
>	<tr>
>		<td style="vertical-align: middle; text-align: center;">Sicherung</td>
>		<td rowspan="2" style="vertical-align: middle; text-align: center;">Netzzugang</td>
>		<td rowspan="2" style="vertical-align: middle; text-align: center;">Ethernet<br>WLAN</td>
>		<td rowspan="2" style="vertical-align: middle; text-align: center;">Rahmen<br>Frame<br>Bit<br>Symbol</td>
>		<td></td>
>		<td  style="vertical-align: middle; text-align: center;">Switch<br>Bridge</td>
>	</tr>
>	<td  style="vertical-align: middle; text-align: center;">Bitübertragung</td>
>	<td></td>
>	<td  style="vertical-align: middle; text-align: center;">Hub<br>Repeater</td>
></table>

---

In der Computer- und Netzwerktechnik haben sich Schichtenmodelle etabliert, um komplexe Vorgänge in einzelne Schritte zu gliedern. Jeder Schritt oder jede Aufgabe wird dabei als Schicht übereinander dargestellt. Das OSI-Schichtenmodell ist ein solches Referenzmodell für herstellerunabhängige Kommunikationssysteme und dient als Design-Grundlage für Kommunikationsprotokolle und Computernetze.

Entwickelt von der Internationalen Organisation für Normung ([ISO]), steht OSI für Open System Interconnection (Offenes System für Kommunikationsverbindungen). Das Modell besteht aus 7 Schichten und ist feiner und detaillierter gegliedert als das DoD-Schichtenmodell. Jede Schicht im OSI-Modell definiert spezifische Aufgaben und Funktionen für die Kommunikation zwischen zwei Systemen. Es gibt Verfahren und Protokolle, die diese Aufgaben erfüllen und der übergeordneten Schicht bestimmte Dienstleistungen bereitstellen.

Bei der Kommunikation zwischen zwei Systemen durchläuft der Datenfluss alle 7 Schichten des OSI-Modells mindestens zweimal - einmal beim Sender und einmal beim Empfänger. Dieses Modell wird häufig zur Veranschaulichung der Kommunikationsabläufe verwendet, obwohl das DoD-Schichtenmodell, insbesondere in Verbindung mit der TCP/IP-Protokollfamilie, näher an der praktischen Realität des Internets liegt.

---

# Protokolle im OSI-Schichtenmodell
[Protokolle] sind eine Sammlung von Regeln zur Kommunikation, die auf einer bestimmten Schicht des OSI-Schichtenmodells definiert sind. Jedes Protokoll innerhalb einer Schicht ist weitgehend transparent gegenüber den Protokollen der über- und untergeordneten Schichten. Dies bedeutet, dass die Verhaltensweise eines Protokolls sich ähnlich verhält, als würde es direkt mit dem entsprechenden Protokoll auf der gegenüberliegenden Seite kommunizieren.

Die Übergänge zwischen den Schichten werden als Schnittstellen bezeichnet und sind entscheidend für die Kommunikation zwischen den Protokollen. Manche Protokolle sind speziell für bestimmte Anwendungen entwickelt worden und können sich über mehrere Schichten erstrecken, um mehrere Aufgaben abzudecken. In solchen Fällen kann es vorkommen, dass bestimmte Aufgaben in mehreren Schichten ausgeführt werden müssen, was die Komplexität der Kommunikation erhöht.

---

# 1. Bitübertragungsschicht / Physical Layer
Die Bitübertragungsschicht ist fundamental für die Kommunikation in Netzwerken, da sie die Schnittstelle zum physikalischen Übertragungsmedium bildet. Hier werden die elektrischen, mechanischen und funktionalen Details festgelegt, die für die Übertragung von Bitfolgen über das Medium erforderlich sind. 

Die Protokolle dieser Schicht variieren je nach dem spezifischen Übertragungsmedium und den verwendeten Übertragungsverfahren. Dabei ist es wichtig zu betonen, dass das Übertragungsmedium selbst nicht direkt Teil der Bitübertragungsschicht ist, sondern als externes Element betrachtet wird, das durch die Schnittstelle der Schicht 1 bedient wird.

---

# 2. Sicherungsschicht / Data Link Layer
Die Sicherungsschicht spielt eine entscheidende Rolle bei der Gewährleistung einer stabilen und zuverlässigen Verbindung zwischen einem Endgerät und dem physischen Übertragungsmedium. Ihre Hauptaufgaben umfassen die Fehlererkennung, Fehlerbehebung und die Kontrolle des [Datenflusses], um eine fehlerfreie [Datenübertragung] zu gewährleisten und [Datenverluste] zu minimieren.

Ein zentraler Aspekt der Sicherungsschicht ist die Verwaltung logischer Verbindungen mittels [Datenpaketen]. Hier werden Datenpakete mit einer [physikalischen Adresse] versehen, um sicherzustellen, dass sie korrekt über das Medium gesendet und empfangen werden können. Zudem implementiert diese Schicht elementare Mechanismen zur Fehlererkennung, wie etwa [Prüfsummen] oder [CRC] (Cyclic Redundancy Check), die sicherstellen, dass die übertragenen Daten korrekt angekommen sind und ggf. fehlerhaft empfangene Datenpakete erneut angefordert werden können.

---

# 3. Vermittlungsschicht / Network Layer
Die Vermittlungsschicht (auch als Netzwerkschicht bekannt) spielt eine zentrale Rolle bei der Steuerung der Kommunikation zwischen Endgeräten in einem Netzwerk. Unabhängig vom spezifischen [Übertragungsmedium] und der [Netzwerktopologie] koordiniert diese Schicht die zeitlich und logisch getrennte Übertragung von Daten zwischen verschiedenen Endpunkten.

Ein wesentliches Merkmal der Vermittlungsschicht ist die Einführung der[logischen Adressierung] der Endgeräte. Diese Adressen dienen dazu, die Identität der Empfängergeräte auf einem Netzwerk zu definieren. Die logische Adressierung ist eng mit dem Routingprozess verbunden, der die Wegfindung von einem Sender zu einem Empfänger innerhalb des Netzwerks ermöglicht. 

[Routing] bezeichnet dabei den Prozess, bei dem Netzwerkpakete über verschiedene Netzwerke hinweg geleitet werden, basierend auf den Zieladressen in den Paketen. Dieser Vorgang umfasst die Auswahl der optimalen Route sowie die Weiterleitung der Pakete über Zwischenstationen ([Router]), um sicherzustellen, dass sie ihr Ziel erreichen.

Zusätzlich zur Routingfunktion übernimmt die Vermittlungsschicht auch Aufgaben der Datenflusskontrolle, um sicherzustellen, dass die Datenübertragung effizient und ohne Überlastung der Netzwerkressourcen erfolgt. Diese Schicht spielt somit eine entscheidende Rolle für die Verwaltung der Netzwerkkommunikation und trägt maßgeblich zur Zuverlässigkeit und Effizienz von Datenübertragungen bei.

---

# 4. Transportschicht / Transport Layer
Die Transportschicht fungiert als Bindeglied zwischen den transportorientierten und anwendungsorientierten Schichten eines Netzwerks. Ihre Hauptaufgabe besteht darin, die Kommunikation zwischen Anwendungen auf unterschiedlichen Endgeräten zu unterstützen, indem sie den zuverlässigen Transport von Datenpaketen über logische Ende-zu-Ende-Verbindungen ermöglicht.

Diese Schicht ist für die Segmentierung und Wiederzusammenstellung von Datenpaketen verantwortlich, die von den Anwendungen gesendet und empfangen werden. Sie bietet Mechanismen zur Fehlererkennung und -korrektur sowie zur Datenflusskontrolle, um sicherzustellen, dass die übertragenen Datenpakete zuverlässig und in der richtigen Reihenfolge ankommen.

Ein wichtiger Aspekt der Transportschicht ist die Identifizierung der Kommunikationsendpunkte, die durch sogenannte [Ports] definiert werden. Diese Ports ermöglichen es mehreren Anwendungen, gleichzeitig auf einem Gerät zu kommunizieren, indem sie eindeutige Kennungen für den Datenaustausch bereitstellen.

Zu den bekannten Protokollen der Transportschicht gehören [TCP] (Transmission Control Protocol) und [UDP] (User Datagram Protocol). TCP bietet eine verbindungsorientierte Kommunikation mit hoher Zuverlässigkeit und Gewährleistung der [Datenintegrität], während UDP eine verbindungslose Kommunikation bietet, die weniger [Overhead] erzeugt und für Anwendungen geeignet ist, bei denen ein schneller Datenaustausch wichtiger ist als die Zuverlässigkeit.

---

# 5. Kommunikationsschicht / Session Layer
Die Kommunikationsschicht, auch bekannt als Sitzungsschicht oder Prozess-zu-Prozess-Schicht, spielt eine zentrale Rolle bei der Organisation und Verwaltung von Verbindungen zwischen Endsystemen in einem Netzwerk. Sie stellt Steuerungs- und Kontrollmechanismen bereit, die die Einrichtung, Verwaltung und Beendigung von Kommunikationsverbindungen sowie den Datenaustausch zwischen Anwendungen ermöglichen.

Diese Schicht ist dafür verantwortlich, dass verschiedene Prozesse auf unterschiedlichen Geräten miteinander kommunizieren können, indem sie eine strukturierte Art und Weise bereitstellt, wie diese Prozesse miteinander interagieren können. Sie koordiniert die Sitzungen, überwacht den Dialog und stellt sicher, dass die Datenübertragung zwischen den Anwendungen effizient und zuverlässig erfolgt.

Zu den Aufgaben der Kommunikationsschicht gehört es auch, die Interaktion zwischen den Anwendungen zu verwalten, unabhängig davon, ob diese Anwendungen auf demselben Rechner oder auf unterschiedlichen Endgeräten innerhalb des Netzwerks ausgeführt werden. Sie ermöglicht es den Anwendungen, synchronisiert zu kommunizieren, Datenströme zu steuern und Sicherheitsmechanismen für die Datenübertragung zu implementieren.

Ein Beispiel für Protokolle auf dieser Schicht sind das [Session Initiation Protocol] (SIP) und das [Remote Procedure Call] (RPC), die beide dafür entwickelt wurden, um die Interaktion zwischen Anwendungen über Netzwerkgrenzen hinweg zu erleichtern und sicherzustellen.

---

# 6. Darstellungsschicht / Presentation Layer
Die Darstellungsschicht, auch als Presentation Layer bekannt, spielt eine zentrale Rolle bei der Umwandlung von Daten in verschiedene [Codecs] und Formate. Sie stellt sicher, dass die Daten von der Anwendungsschicht in ein geeignetes Format umgewandelt werden, das für die Übertragung über das Netzwerk geeignet ist, und umgekehrt.

Diese Schicht kümmert sich um die Syntax und Semantik der übertragenen Informationen, wobei sie keine Kenntnis über die eigentlichen Inhalte oder Anwendungen hat, sondern nur darüber, wie die Daten dargestellt und interpretiert werden sollen. Zu ihren Aufgaben gehört die Kodierung der Daten in ein allgemein verständliches Format, das von der darunterliegenden Kommunikationsschicht transportiert werden kann.

Ein wichtiges Merkmal der Darstellungsschicht ist die Möglichkeit, Daten in Standardformate umzuwandeln, die unabhängig von den spezifischen Systemen oder Anwendungen sind, die die Daten erzeugt oder empfangen. Dies erleichtert die Interoperabilität zwischen verschiedenen Systemen und Netzwerken, da die Darstellungsschicht sicherstellt, dass die Daten bei der Übertragung korrekt interpretiert und verarbeitet werden können.

Beispiele für Funktionen der Darstellungsschicht sind die Datenkompression, [Verschlüsselung], Formatierung und die Kodierung in spezifische [Datentypen] oder Codierungen wie [ASCII], [Unicode] oder [Binärformate]. Durch diese Prozesse wird sichergestellt, dass die Daten effizient und sicher übertragen werden können, unabhängig von den spezifischen technischen Details der übertragenden und empfangenden Systeme.

---

# 7. Anwendungsschicht / Application Layer
Die Anwendungsschicht ist die oberste Schicht im OSI-Schichtenmodell und stellt eine direkte Schnittstelle für Anwendungen und Dienste bereit. Sie ermöglicht es den Benutzern, auf Netzwerkdienste zuzugreifen und sie zu nutzen. Hier finden die Dateneingabe und -ausgabe statt, wobei die Anwendungen direkt mit den unteren Schichten kommunizieren, um Daten zu senden oder zu empfangen.

Diese Schicht bietet eine Vielzahl von Diensten und Funktionen für verschiedene Anwendungen. Dazu gehören typischerweise Anwendungen wie Webbrowser, E-Mail-Clients, Dateiübertragungsprogramme, Streaming-Anwendungen und vieles mehr. Die Anwendungsschicht stellt die notwendigen Mittel bereit, damit Anwendungen über das Netzwerk miteinander kommunizieren können, unabhängig von den zugrunde liegenden Details der Netzwerkinfrastruktur.

Ein entscheidender Aspekt der Anwendungsschicht ist die Interoperabilität, die es ermöglicht, dass Anwendungen unterschiedlicher Hersteller und auf verschiedenen Plattformen miteinander kommunizieren können. Dies wird durch die Verwendung standardisierter Protokolle und Formate erreicht, die von der Anwendungsschicht unterstützt werden.

---

# Kurzbeschreibung des OSI-Schichtenmodells

7. Schicht / **Anwendung**: Funktionen für Anwendungen, sowie die Dateneingabe und -ausgabe.  
6. Schicht / **Darstellung**: Umwandlung der systemabhängigen Daten in ein unabhängiges Format.  
5. Schicht / **Kommunikation**: Steuerung der Verbindungen und des Datenaustauschs.  
4. Schicht / **Transport**: Zuordnung der Datenpakete zu einer Anwendung.  
3. Schicht / **Vermittlung**: Routing der Datenpakete zum nächsten Knoten.  
2. Schicht / **Sicherung**: Segmentierung der Pakete in Frames und Hinzufügen von Prüfsummen.  
1. Schicht / **Bitübertragung**: Umwandlung der [Bits] in ein zum Medium passendes Signal und physikalische Übertragung.

Hinweis: Die Endgeräte der Endsysteme und das Übertragungsmedium sind aus dem OSI-Schichtenmodell ausgeklammert. Trotzdem kann es sein, dass die Endgeräte in der Anwendungsschicht und das Übertragungsmedium in der Bitübertragungsschicht vorgegeben sind.

---

# Das OSI-Schichtenmodell in der Praxis
Das OSI-Schichtenmodell wird oft als Referenz für die Darstellung von Kommunikationsabläufen und Nachrichtenübermittlung verwendet. Allerdings spiegelt das DoD-Schichtenmodell (TCP/IP) die Realität viel genauer wider. Das Problem des OSI-Modells liegt in der schwerfälligen Standardisierungsorganisation ISO, die nicht schnell genug war, um rasch einen Rahmen für Protokolle und Übertragungssysteme in der Netzwerktechnik zu schaffen. Im Gegensatz dazu war TCP/IP frei verfügbar, funktionierte gut und verbreitete sich schnell mit zusätzlichen Protokollen. Letztlich blieb der ISO keine andere Wahl, als TCP/IP im OSI-Modell zu berücksichtigen.

Zusätzlich zu TCP/IP haben sich weitere Netzwerkprotokolle entwickelt, die jedoch größtenteils von TCP/IP verdrängt wurden. Heutzutage arbeiten fast alle Netzwerke auf Basis von TCP/IP.

In einer Tabelle werden verschiedene Protokolle, Übertragungs- und Vermittlungstechniken den Schichten des OSI-Modells zugeordnet. Da viele dieser Techniken mehrere Schichten nutzen können, ist eine vollständige und fehlerfreie Darstellung in der Tabelle nicht immer gewährleistet.

| Schicht 7 | Anwendung     | Telnet, FTP, HTTP, SMTP, NNTP                                          |
| --------- | ------------- | ---------------------------------------------------------------------- |
| Schicht 6 | Darstellung   | Telnet, FTP, HTTP, SMTP, NNTP, NetBIOS                                 |
| Schicht 5 | Kommunikation | Telnet, FTP, HTTP, SMTP, NNTP, NetBIOS, TFTP                           |
| Schicht 4 | Transport     | TCP, UDP, SPX, NetBEUI                                                 |
| Schicht 3 | Vermittlung   | IP, IPX, ICMP, T.70, T.90, X.25, NetBEUI                               |
| Schicht 2 | Sicherung     | LLC/MAC, X.75, V.120, ARP, HDLC, PPP                                   |
| Schicht 1 | Übertragung   | Ethernet, Token Ring, FDDI, V.110, X.25, Frame Relay, V.90, V.34, V.24 |

Auch wenn nur die Schichten von 1 bis 7 offiziell definiert sind, gelten steht im allgmeinen Sprachgebraucht die Schicht 0 für die Verkabelung und die Hardware. Die Schicht 8 stellt den Anwender mit seinen Anforderungen oder die Politik dar. Die Schicht 9 ist die Religion oder ein Dogma.

---

# Schichtenmodell: Datenübertragung und Adressierung

<table>
	<tr>
		<th style="vertical-align: middle; text-align: center;">Schichten</th>
		<th colspan="2" style="vertical-align: middle; text-align: center;">Datenverarbeitung und -übertragung</th>
		<th colspan="2" style="vertical-align: middle; text-align: center;">Adressierung und Verbindungsaufbau</th>
	</tr> 
	<tr>
		<td style="vertical-align: middle; text-align: center;">Anwendung OSI-Schicht 5 + 6 + 7</td>
		<td style="vertical-align: middle; text-align: center;">HTTP, FTP, IMAP, SMTP</td>
		<td style="vertical-align: middle; text-align: center;">URL: www.google.com <p style="font-size: 30px;">&#8595;</p> host / DNS  <p style="font-size: 30px;">&#8595;</p> </td>
		<td style="vertical-align: middle; text-align: center;">NetBIOS S-Name (Computername) <p style="font-size: 30px;">&#8595;</p> Imhost / WINS <p style="font-size: 30px;">&#8595;</p>
	</tr>
	<tr>
		<td style="vertical-align: middle; text-align: center;"> Übertragung OSI-Schicht 3 + 4</td>
		<td colspan="2" style="vertical-align: middle; text-align: center;">Transport: TCP / UDP (Datenpakete) <p style="font-size: 30px;">&#8595;</p> Adressierung: IP /ICMP (Adresse)  <p style="font-size: 30px;">&#8595;</p> </td>
		<td style="vertical-align: middle; text-align: center;">IP-Adresse und TCP/UDP-Port <p style="font-size: 30px;">&#8595;</p> </td>
	</tr>
	<tr>
		<td style="vertical-align: middle; text-align: center;">Netzzugang (physikalisch) OSI-Schicht 1 + 2</td>
		<td colspan="2" style="vertical-align: middle; text-align: center;">NDIS <p style="font-size: 30px;">&#8595;</p> Treiber <p style="font-size: 30px;">&#8595;</p> NIC
		<td style="vertical-align: middle; text-align: center;">ARP <p style="font-size: 30px;">&#8595;</p> MAC-Adresse <p style="font-size: 30px;">&#8595;</p> Ethernet
	</tr>
</table>

---

# Beschreibung der Datenübertragung
In den Anwendungsschichten 5, 6 und 7 sind alle Protokolle definiert, auf die Programme und Anwendungen direkt zugreifen. In der Windows-Netzwerkwelt stellt [SMB] mit [NetBIOS] die Verbindung zur Übertragungsschicht her. Wenn ein Unix-[Betriebssystem] mit Windows kommunizieren soll, wird beispielsweise der Dienst Samba genutzt, um Anwendungen die Ressourcen im Windows-Netzwerk auf dem Unix-Betriebssystem zur Verfügung zu stellen.

Die Verbindung zwischen Anwendungs- und Übertragungsschicht wird über Ports von TCP hergestellt. Anwendungen und Dienste erhalten ihre Daten über diese Ports. Der Datenstrom wird entweder vom verbindungsorientierten Transportprotokoll TCP oder vom verbindungslosen Transportprotokoll UDP in Pakete verpackt. Das Internet Protocol (IP) übernimmt die Adressierung der Pakete.

Der [Bitstrom] wird an den [NDIS] (Network Driver Interface Specification) weitergeleitet, der mit dem Gerätetreiber der Netzwerkkarte kommuniziert. Erst der Treiber sendet die Daten an die [Netzwerkkarte] (NIC). Von dort gehen die Daten auf die Reise durch das Netzwerk, wobei alle Details der physischen Verbindung über verschiedene Netzwerke hinweg behandelt werden.

Bei eingehenden Daten erfolgt der Prozess in umgekehrter Reihenfolge.

[TCP]
[UDP]
[IPv4]

---

# Beschreibung des Verbindungsaufbaus
Innerhalb der Anwendungsschicht dient die [URL] (Universal Resource Locator) zur Identifikation eines Computers und der darauf ausgeführten Dienste. In Windows-Netzwerken übernimmt der NetBIOS-Name des Computers diese Aufgabe. Zur Auflösung der URL in eine [IP-Adresse] wird die Datei `hosts` verwendet, in der alle URLs und IP-Adressen aufgelistet sind. Aufgrund der Vielzahl an URLs wurde das [DNS] (Domain Name System) eingeführt, das hierarchisch aufgebaut ist. DNS-Server können unbekannte DNS-Namen bei übergeordneten DNS-Servern anfragen. Im Windows-Netzwerk wird die Datei `lmhosts` oder der [WINS]-Server (Windows Internet Name Service) zur Auflösung von NetBIOS-Namen in IP-Adressen verwendet.

Sobald die IP-Adresse in der Übertragungsschicht aufgelöst ist, wird [ARP] (Address Resolution Protocol) verwendet, um die IP-Adresse in die [MAC-Adresse] (Media Access Control) der Netzwerkkarte in der physikalischen Schicht zu übersetzen. Die MAC-Adresse ist die einzige eindeutige Adresse, mit der ein Computer im Netzwerk sicher identifiziert werden kann, da sie fest auf einer Netzwerkkarte eingestellt ist.

---

# OSI-Schichtenmodell im [ISDN]

<table>
  <tr>
    <th rowspan="2" style="vertical-align: middle; text-align: center;">OSI-Schichten</th>
    <th rowspan="2" style="vertical-align: middle; text-align: center;">ISDN-D-Kanal</th>
    <th colspan="2" style="vertical-align: middle; text-align: center;">ISDN-B-Kanal</th>
  </tr>
  <tr>
    <th style="vertical-align: middle; text-align: center;">Dienst: Sprache</th>
    <th style="vertical-align: middle; text-align: center;">Dienst: Daten</th>
  </tr>
  <tr>
    <td style="vertical-align: middle; text-align: center;">OSI-Schicht 5 + 6 + 7 Anwendung</td>
    <td></td>
    <td></td>
    <td style="vertical-align: middle; text-align: center;">Übertragung der Daten, wie in der Netzwerktechnik</td>
  </tr>
  <tr>
    <td style="vertical-align: middle; text-align: center;">OSI-Schicht 4</td>
    <td style="vertical-align: middle; text-align: center;"></td>
    <td style="vertical-align: middle; text-align: center;">Sprachcodierung (a-Law oder μ-Law)</td>
    <td style="vertical-align: middle; text-align: center;">HDLC, PPP oder Frame Relay<br>Multilink-PPP<br>X.75 und V.110</td>
  </tr>
  <tr>
    <td style="vertical-align: middle; text-align: center;">OSI-Schicht 3 Vermittlung</td>
    <td style="vertical-align: middle; text-align: center;">Signalisierung<br>Funktionen zum Auf- und Abbau von Verbindungen<br>Funktionen für ISDN-Dienstmerkmale</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align: middle; text-align: center;">OSI-Schicht 2 Sicherung</td>
    <td style="vertical-align: middle; text-align: center;">Sicherung der Übermittlung der gesamten Bitübertragungsschicht per CRC-Check<br>Endgeräteadressierung (TEI-Vergabe bei Mehrgeräteanschlüssen)</td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td rowspan="2" style="vertical-align: middle; text-align: center;">OSI-Schicht 1 Bitübertragung</td>
    <td>Übertragung der Steuerinformationen im D-Kanal (16 kBit/s)<br>Rahmenbildung auf dem S0-Bus (I.430)</td>
    <td colspan="2" style="vertical-align: middle; text-align: center;">Übertragung von je 64 kBit/s Nutzdaten (für Anwendungen oder Sprache) pro B-Kanal</td>
  </tr>
  <tr> 
	  <td colspan="3" style="vertical-align: middle; text-align: center;">Rahmenbildung auf dem S0-Bus (I.430)</td> 
</tr>
</table>

---

![[../../../Template/© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]

