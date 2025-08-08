>**Das wichtigste auf einen Blick:**
>- **Netzwerk**: Physikalische und logische Verbindung mehrerer Computersysteme.
>- **Protokolle**: Regeln für Kommunikation zwischen Systemen.
>- **Schichtenmodell**: Aufteilung der Kommunikation in Schichten (z.B. OSI-Modell).
>- **Verbindungsarten**: Verbindungsorientiert vs. verbindungslos.
>- **Peer-to-Peer-Netzwerke**: Gleichberechtigte Teilnehmer ohne zentralen Verwalter.
>- **LAN, WAN, GAN**: Unterschiedliche Netzwerkausmaße und -typen.
>- **Sicherheit**: Bedeutung von Sicherheitsmaßnahmen bei globaler Vernetzung.
>- **Ressourcennutzung**: Gemeinsame Nutzung von Hardware und Diensten.

<br>

Ein Netzwerk ist die physische und logische Verbindung mehrerer Computersysteme. Es basiert auf Übertragungstechniken, Protokollen und Systemen, die die Kommunikation zwischen den Netzwerkteilnehmern ermöglichen. Ein einfaches Netzwerk besteht aus zwei Computern, die über ein Kabel verbunden sind und dadurch ihre Ressourcen wie Rechenleistung, Speicher, Programme, Daten, Drucker und andere Peripheriegeräte gemeinsam nutzen können. Ein netzwerkfähiges Betriebssystem stellt diese Ressourcen den Benutzern auf der Anwendungsebene zur Verfügung.

Daraus ergeben sich mehrere Vorteile gegenüber unvernetzten Computern:

- Gemeinsame Nutzung von Datenbeständen
- Zugriff auf verfügbare Ressourcen
- Teilen von Rechenleistung und Speicherkapazität
- Zentrale Steuerung von Programmen und Daten
- Durchsetzung von Berechtigungen und Zuständigkeiten
- Gewährleistung von Datenschutz und Datensicherheit

Zu Beginn der Computergeschichte waren Peripheriegeräte und Speicher sehr teuer. Die erste Möglichkeit, Peripheriegeräte gemeinsam zu nutzen, waren manuelle Umschaltboxen, mit denen mehrere Computer einen Drucker teilen konnten. Welcher Computer den Drucker nutzen konnte, wurde über die Umschaltbox bestimmt. Allerdings hatten Umschaltboxen den Nachteil, dass Computer und Peripheriegeräte aufgrund der begrenzten Kabellänge relativ nah beieinander stehen mussten.

Der Bedarf, Daten zwischen mehreren Computern auszutauschen und Ressourcen zu teilen, führte schließlich zur Vernetzung von Computern.

---

# Netzwerk-Dimensionen: LAN, WAN und GAN

Bestimmte Netzwerktechniken unterliegen Beschränkungen, die insbesondere die Reichweite und geografische Ausdehnung des Netzwerks begrenzt. Hierbei unterscheidet man zwischen verschiedenen Netzwerk-Dimensionen für die es unterschiedliche Netzwerktechniken gibt.

- [[7_WPAN|PAN]] - Personal Area Network, z. B. Bluetooth
- [[5_LAN|LAN]] - Local Area Network, z. B. Ethernet und WLAN
- [[MAN]] - Metropolitan Area Network: regionales Netz
- [[8_WAN|WAN]] - Wide Area Network: öffentliches Netz, z. B. DSL und Mobilfunk
- [[GAN]] - Global Area Network: globales Netz, z. B. das Internet

![[../../../IMG/IMG_IT/Netzwerk_Dimensionen.png]]

Normalerweise findet ein Austausch zwischen verschiedenen Netzwerken statt. Das bedeutet, dass ein Teilnehmer eines LANs oft auch Zugang zu einem WAN oder einem GAN hat. Eine exakte Abgrenzung zwischen diesen Netzwerkdimensionen ist nicht immer möglich, weshalb häufig eine grobe Einteilung vorgenommen wird. Üblicherweise unterscheidet man zwischen LAN und WAN, wobei es Techniken und Protokolle gibt, die in beiden Netzwerktypen eingesetzt werden können.

Warum vernetzen wir Computersysteme zu einem LAN? Um gemeinsame Ressourcen zu nutzen, wie beispielsweise Internetzugang, Drucker, Speicher, Rechenleistung, Dienste und Anwendungen.

Warum verbinden wir uns mit einem WAN? Um Dienste von anderen zu nutzen oder eigene Dienste anzubieten, wie beispielsweise Datenverarbeitung und Informationsaustausch.

Warum verbinden wir uns mit einem GAN? Um an weltweit verfügbaren Kommunikationsanwendungen teilzunehmen, wie Internet, Telefonie, Messaging und E-Mail.

---

# Protokolle in der Netzwerktechnik
In der Netzwerktechnik regeln Protokolle die Kommunikation zwischen Systemen. Netzwerkprotokolle sind Sammlungen von Regeln, die festlegen, wie die Kommunikation zwischen zwei oder mehr Systemen abläuft. Sie definieren, wie die Verbindung hergestellt wird, wie und welche Informationen ausgetauscht werden, und wie die Kommunikation beendet wird. Während einer Sitzung werden nicht nur Daten ausgetauscht, sondern auch Protokollinformationen, die vom Empfänger verarbeitet werden.

Typischerweise wird die Kommunikation nicht von einem einzigen Protokoll gesteuert, sondern von mehreren Protokollen, die spezifische Aufgaben übernehmen. Diese Protokolle werden nach einem Schichtenmodell organisiert, wobei jedes Protokoll einer bestimmten Schicht zugeordnet ist.

[[31_Protokolle|Protokolle]]

---

# Schichtenmodelle 
Da ein Netzwerk möglichst universell sein soll, sodass es von mehreren Teilnehmern und Anwendungen gleichzeitig genutzt werden kann, ist die Netzwerkkommunikation in Schichten aufgeteilt. Jede Schicht hat eine spezifische Aufgabe und löst ein bestimmtes Teilproblem der Kommunikation. Dabei müssen Sender und Empfänger das gleiche Schichtenmodell verwenden.

Es existieren verschiedene Schichtenmodelle, die sich in der Anzahl der Schichten und der damit verbundenen Verdichtung der Aufgaben unterscheiden.

[[12_Schichtenmodelle|Schichtenmodelle]]
[[13_DoD-Schichtenmodell|DoD-Schichtenmodell]]
[[14_OSI-Schichtenmodell|OSI-Schichtenmodell]]

---

# Datenübertragung
Die Kommunikation kann grundsätzlich auf zwei Arten erfolgen: verbindungsorientiert oder verbindungslos.

Bei der verbindungsorientierten Datenübertragung wird vor dem Datenaustausch eine logische Verbindung hergestellt. Diese Verbindung bleibt während der gesamten Übertragung aufrechterhalten und wird erst durch einen Verbindungsabbau beendet.

Bei der verbindungslosen Kommunikation hingegen wird keine logische und somit auch keine dauerhafte Verbindung aufgebaut. Die Daten werden in kleine Einheiten aufgeteilt, und jede Einheit wird als abgeschlossener Vorgang übertragen. Diese Übertragungseinheiten werden je nach Technik allgemein als Pakete oder Datenpakete bezeichnet. Die Protokolle und OSI-Schichten verwenden oft spezifische Begriffe für diese Einheiten, die jedoch meist dasselbe bedeuten.

| OSI-Schicht    | Typ (Deutsch)       | Typ (Englisch) |
|:-------------- |:------------------- |:-------------- |
| Alle Schichten | Paket/Datenpaket    | Packet         |
| Anwendung      | Nachricht           | Message        |
| Transport      | Segment             | Segment        |
| Vermittlung    | Datagramm           | Datagramm      |
| Sicherung      | Rahmen              | Frame          |
| Bitübertragung | Bitfolge / Bitstrom | Bitstream      |

Ganz allgemein spricht man von Datenpaketen oder nur Paketen. Nimmt man es ganz genau, dann spricht man bei IPv4 von Datagrammen (RFC 891) und bei IPv6 von Paketen (RFC 2460) und bei TCP ist es das Segment.

---

# Netzwerk-Adressen
Innerhalb eines Netzwerks werden spezielle Netzwerk-Adressen verwendet, um Sender und Empfänger eines Datenpakets oder einer Nachricht zu adressieren. Diese Netzwerk-Adressen unterscheiden sich anhand ihrer Funktion, Anwendungen und Protokoll-Schicht. Das bedeutet, dass eine Kommunikation auf jeder OSI-Schicht mit eigenen Adressen arbeitet.

#### Adressen und ihre Funktionen in verschiedenen OSI-Schichten:

1. **Physikalische Schicht (Layer 1)**:
    
    - Keine spezifischen Adressen, sondern physikalische Merkmale wie Signalstärke und Modulationstechniken.
2. **Sicherungsschicht (Layer 2)**:
    
    - **MAC-Adressen (Media Access Control)**: Eindeutige physische Adressen, die Netzwerkkarten zugewiesen werden und zur Identifikation von Geräten innerhalb eines lokalen Netzwerks dienen.
3. **Netzwerkschicht (Layer 3)**:
    
    - **IP-Adressen (Internet Protocol)**: Logische Adressen, die zur Identifikation und Lokalisierung von Geräten im Netzwerk verwendet werden. Unterscheidung zwischen IPv4 (z.B., 192.168.1.1) und IPv6 (z.B., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
    - **Subnetzmasken und Gateway-Adressen**: Ergänzen IP-Adressen zur Definition von Netzwerken und zur Bestimmung von Standard-Routen.
4. **Transportschicht (Layer 4)**:
    
    - **Port-Nummern**: Spezifische Kommunikationsendpunkte innerhalb eines Geräts. Werden verwendet, um Daten an die richtigen Anwendungen zu leiten (z.B., Port 80 für HTTP, Port 443 für HTTPS).
5. **Sitzungsschicht (Layer 5)**:
    
    - **Sitzungs-IDs**: Identifikatoren, die Sitzungen zwischen Endpunkten verwalten und synchronisieren.
6. **Darstellungsschicht (Layer 6)**:
    
    - **Keine spezifischen Adressen**: Diese Schicht kümmert sich um die Syntax und Semantik der Informationen, z.B. durch Datenkompression und -verschlüsselung.
7. **Anwendungsschicht (Layer 7)**:
    
    - **URL und URN (Uniform Resource Locator/Name)**: Adressen, die zur Identifikation von Ressourcen im Internet verwendet werden (z.B., [https://www.example.com](https://www.example.com)).
    - **E-Mail-Adressen**: Verwendet in Anwendungen wie E-Mail-Protokollen (SMTP, IMAP).

Internet-Adressen ist ein Überbegriff für Netzwerk-Adressen, die im Internet verwendet werden.

Der Aufbau von Netzwerk-Adressen ist meistens hierarchisch. Das bedeutet, für die einzelnen Bestandteile einer Netzwerk-Adresse gibt es verschiedene verantwortliche Stellen. So stellt man sicher, dass Adressen eindeutig sind und deren Zuteilung nicht zu sehr zentralistisch ist.

[[4_Anwendungen_und_Dienste/1_Netzwerk-Adressen|Netzwerk-Adressen]]

---

# Ein einfaches Netzwerk: Peer-to-Peer

![[../../../IMG/IMG_IT/P2P_Netzwerk.png]]

In einem Peer-to-Peer-Netzwerk sind alle angeschlossenen Computer gleichberechtigt und stellen einander ihre Ressourcen zur Verfügung. Solche Netzwerke eignen sich für bis zu 10 Stationen, da es bei mehr Teilnehmern schnell unübersichtlich wird. Diese Netzwerke sind relativ schnell und kostengünstig aufzubauen, wobei die Teilnehmer möglichst nah beieinander stehen sollten.

Es gibt keinen zentralen Netzwerkverwalter; jeder Teilnehmer ist für seinen eigenen Computer verantwortlich. Daher muss jeder selbst entscheiden, welche Ressourcen er freigibt und die Datensicherung eigenständig durchführen.

---

# Sicherheit in Netzwerken
Die zunehmende globale und lokale Vernetzung hat die Bedeutung der Computersicherheit und Netzwerksicherheit stark erhöht. Früher waren viele Netzwerke isoliert und ohne Verbindung nach außen, während heutzutage praktisch jedes Netzwerk mit dem Internet verbunden ist. Dadurch ist es möglich, dass Personen aus aller Welt, unabhängig von ihren Absichten, eine Verbindung zu jedem Netzwerk herstellen können.

- [[|Grundlagen der Netzwerk-Sicherheit]]
- [[|Sicherheitsrisiken und Sicherheitslücken in der Netzwerktechnik]]
- [[|Wie sicher ist ...?]]
- [[|Sicherheitskonzepte in der Informations- und Netzwerktechnik]]
- [[|Kryptografie]]
- [[|Authentifizierung im Netzwerk]]
- [[|Verschlüsselung]]

---

# TCP/IP
TCP/IP ist eine Protokoll-Familie, die für die Vermittlung und den Transport von Datenpaketen in dezentral organisierten Netzwerken verwendet wird, sowohl in LANs (Local Area Networks) als auch in WANs (Wide Area Networks). Die zentrale Aufgabe von TCP/IP ist es, sicherzustellen, dass Datenpakete innerhalb des Netzwerks korrekt beim Empfänger ankommen. Dafür stellt TCP/IP die folgenden zentralen Funktionen bereit:

- **Adressierung**: Jedes Gerät in einem TCP/IP-Netzwerk erhält eine eindeutige IP-Adresse, die zur Identifizierung und Lokalisierung verwendet wird.
    
- **Routing**: TCP/IP ermöglicht die Weiterleitung von Datenpaketen durch verschiedene Netzwerke, um den Weg vom Sender zum Empfänger zu finden.
    
- **Fragmentierung und Reassemblierung**: TCP/IP kann große Datenpakete in kleinere Einheiten fragmentieren, die über das Netzwerk übertragen werden können, und sie am Ziel wieder reassemblieren.
    
- **Zuverlässigkeit**: Durch das TCP-Protokoll (Transmission Control Protocol) gewährleistet TCP/IP eine zuverlässige Übertragung von Datenpaketen durch Bestätigungen und erneute Übertragungen bei Bedarf.
    
- **Verbindungsaufbau und -abbau**: TCP/IP unterstützt den Aufbau und Abbau von Verbindungen zwischen Sender und Empfänger, um Daten in beide Richtungen sicher zu übertragen.
    
- **Protokollierung und Fehlererkennung**: TCP/IP überwacht den Datenfluss, erkennt Fehler und korrigiert sie gegebenenfalls durch Mechanismen wie Prüfsummen und Sequenznummern.

- [[|TCP/IP]]
- [[|IPv4]]
- [[|IPv6]]
- [[|TCP]]

---

# Ethernet und WLAN

Ethernet ist eine Familie von Netzwerktechniken, die vorwiegend in lokalen Netzwerken (LAN), aber auch zum Verbinden großer Netzwerke zum Einsatz kommt (WAN). Ethernet wird in der Regel als Synonym für ein lokales Netzwerk verstanden. Im Prinzip werden heute fast alle Vernetzungen im LAN und WAN mit Ethernet-Technik realisiert.

Wireless LAN, kurz WLAN, ist die allgemeine Bezeichnung für ein schnurloses lokales Netzwerk (Wireless Local Area Network). IEEE 802.11 ist ein Standard für eine technische Lösung, die den Aufbau eines Wireless LAN ermöglicht. IEEE 802.11 fand schnell Akzeptanz bei Herstellern und Konsumenten. Deshalb ist es die am weitesten verbreitete drahtlose Technik für ein WLAN.

- [[|IEEE 802.3 / Ethernet]]
- [[|IEEE 802.11 / WLAN]]

---

# Virtualisierung im Netzwerk

Typischerweise versteht man unter Virtualisierung den Parallelbetrieb von Betriebssystemen auf einer Hardware. Doch auch in der Netzwerktechnik wird virtualisiert. So lassen sich auf einer Netzwerk-Infrastruktur, bestehend aus Verteilkomponenten und Übertragungswegen, mehrere logisch voneinander getrennte Netzwerke betreiben.

- [[61_Virtualisierung_im_Netzwerk|Virtualisierung im Netzwerk]]
- [[|NFV ]]

---

# Cloud Computing
**Cloud Computing**, auch bekannt als Cloud IT, umfasst Anwendungen, Daten, Speicherplatz und Rechenleistung, die aus einem virtuellen Rechenzentrum, der sogenannten Cloud, bereitgestellt werden. Der Begriff "Cloud" wird verwendet, weil das virtuelle Rechenzentrum aus einem Netzwerk von zusammengeschalteten Computern (Grid) besteht und die Ressourcen nicht von einem spezifischen Computer, sondern von dieser Wolke aus vielen Computern bereitgestellt werden. Dadurch ist keine Anwendung mehr fest einem Server zugeordnet. Die Ressourcen sind dynamisch und können bedarfsweise abgerufen werden.

- [[60_Cloud_Computing|Cloud Computing]]
- [[65_Serverless_Computing|Serverless Computing]]
- [[66_Fass|FaaS]]

---

![[© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten..md]]