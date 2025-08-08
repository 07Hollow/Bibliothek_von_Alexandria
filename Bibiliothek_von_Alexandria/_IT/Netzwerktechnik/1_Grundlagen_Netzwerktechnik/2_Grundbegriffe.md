>**Das wichtigste auf einen Blick:**
>#### Netzwerke und ihre Typen
>- **LAN (Local Area Network)**: Lokales Netzwerk, oft in begrenzten geografischen Bereichen (z.B. Bürogebäude).
>- **WAN (Wide Area Network)**: Weitverkehrsnetzwerk, verbindet kleinere Netzwerke zu einem großen Netzwerk.
>
>#### Netzwerkkomponenten
>- **Node**: Allgemeiner Begriff für ein Gerät im Netzwerk, z.B. Host, Client oder Server.
>- **Link**: Physikalische Verbindung zwischen Nodes.
>- **Site**: Netzwerk und die daran angeschlossenen Nodes unter gemeinsamer Verwaltung.
>- **Host**: Node ohne Router-Eigenschaft, Endgerät wie Client oder Server.
>- **Knoten**: Verzweigungspunkt in einem Netzwerk, z.B. Router oder Switch.
>- **Client**: Endgerät oder Software, die Dienste/Daten anfordert.
>- **Server**: Computer, der Dienste/Daten bereitstellt und Zugriffsrechte verwaltet.
>- **Router**: Node, der Datenpakete weiterleitet.
>- **Gateway**: Schnittstelle zwischen inkompatiblen Netzwerken, wandelt Datenformate um.
>- **Bridge**: Verbindet zwei Teilnetze auf Schicht 1 und 2 des OSI-Modells.
>- **Switch**: Netzwerkgerät, das Verbindungen basierend auf Adressen schaltet.
>
>#### Netzwerkkonzepte und Technologien
>- **Routing**: Prozess der Wegfindung für Datenpakete im Netzwerk.
>- **IP-Routing**: Routing von IP-Paketen basierend auf der Zieladresse.
>- **Subnetz**: LAN-Segment mit gemeinsamem IP-Adresspräfix, durch Router getrennt.
>- **Switching**: Schalten von Verbindungen basierend auf Adressen, konstanter Pfad für Datenpakete.
>- **Protokoll**: Regelwerk für den Datenaustausch zwischen Systemen, z.B. TCP/IP, HTTP.
>- **ISO/OSI-7-Schichtenmodell**: Referenzmodell mit sieben Schichten für Netzwerkkommunikation.
>
>#### Datenübertragung
>- **Datenpaket**: Übertragungseinheit im Netzwerk, enthält Daten sowie Sender- und Empfängeradresse.
>- **Frame**: Logischer Rahmen für einen Bit-Strom, enthält Protokoll- und Ethernet-Header.
>- **Datagramm**: In sich geschlossene Übertragungseinheit auf IP-Ebene.
>- **Datenstrom (Stream)**: Logisch zusammenhängende Datenpakete, die über ein Netzwerk übertragen werden.
>- **Port**: Logische Adresse, die die Zuordnung zwischen Protokoll und Anwendung definiert.
>- **Unidirektionale Kommunikation**: Kommunikation in eine Richtung.
>- **Bidirektionale Kommunikation**: Kommunikation in beide Richtungen, entweder Halbduplex oder Vollduplex.
>
>#### Adressierungsarten
>- **Unicast**: Übertragung von einem Host zu einem anderen Host.
>- **Multicast**: Übertragung von einem Host an mehrere Hosts.
>- **Broadcast**: Übertragung von einem Host an alle anderen Hosts.
>- **Anycast**: Übertragung von einem Host an einen Host aus einer Gruppe.
>
>#### Netzwerkkonzepte
>- **Tunneling**: Einbettung eines Protokoll-Frames in ein anderes Protokoll.
>- **Masquerading**: Verbergen mehrerer interner IP-Adressen hinter einer externen IP-Adresse mittels NAT.
>- **Bonding**: Zusammenschaltung mehrerer Leitungen zu einer logischen Leitung.
>
>#### Netzwerkstrukturen und -kabel
>- **Topologie**: Struktur des Netzwerks, z.B. Bus, Ring, Stern.
>- **Backbone**: Hauptübertragungsstrecke, verbindet Netzknoten.
>- **Leitungen und Kabel**: Leitungen sind sichtbar, Kabel werden im Boden oder auf See verlegt.

---

# LAN und WAN
Netzwerke werden grundsätzlich in ihrer geografischen Ausdehnung differenziert.
Die Abkürzung **LAN** steht für **L**ocal **A**rea **N**etwork. Damit wird wird ein lokales begrenztes Netzwerk bezeichnet, welches aber je nach Organisationsgröße auch mehrere Tausend Teilnehmer umfassen kann. 
WAN steht für **W**ide **A**rea **N**etwork. Gemeint ist damit ein Zusammenschluss kleinere Netzwerke zu einem großen Netzwerk. 
Das LAN ist über einen Router mit dem WAN verbunden. So gelangt man in der Regel ins Internet.

- [[5_LAN|LAN]]
- [[8_WAN|WAN]]

---

# Node 
Node ist ein Überbegriff für eine physikalische Komponente innerhalb eines Netzwerkes. Ein Node ist ein Gerät, welches an einem oder auch mehreren Netzwerken angeschlossen ist und über mehrere Schnittstellen verfügt. 
Verallgemeinert ist ein Node ein Host, ein Client oder ein Server.

---

# Link
Ein physikalisches Netzwerk wird manchmal auch als Link (=Verbindung) bezeichnet. Zu diesem physikalischen Netzwerk gehören alle Nodes, die am selben Link angeschlossen sind.

ggf. noch was aus dem Buch

---

# Site
Ein Netzwerk und die daran angeschlossenen Nodes bilden eine Site. Dafür stehen sie auch unter einer gemeinsamen und zusammenhängenden Verwaltung. Da eine Site oft nur das Lokale Netzwerk einschließt, wird dann eher der Begriff LAN verwendet

---

# Host 
Ein Host ist ein Node ohne Router-Eigenschaften. Typisch wird ein Client oder Server als Host bezeichnet.

---

# Knoten
Allgemein formuliert ist ein Knoten ein Verzweigungspunkt in einem Kommunikationsnetzwerk, an dem mehrere Verbindungen zusammenlaufen. Knoten sind im Telefonnetz die Vermittlungsstellen oder auch Telefonanlagen. In einem IP-Netzwerk sind Router und in einem Ethernet-Netzwerk sind Switche die Knoten.  
Zugangspunkte zu einem Netzwerk, z. B. WLAN-Access-Points, werden häufig auch als Knoten bezeichnet.

---

# Client 
Ein Client ist ein Endgerät oder auch eine Software-Komponente, die von einer zentralen Stelle Dienste oder Daten anfordert oder über einen zentralen Zugang am Netzwerk teilnimmt. Der Client ist als Teil der Client-Server-Architektur in größere Zahl in allen Netzwerken zu finden.  
Typische Hardware-Clients sind PCs, Smartphones, Tablets und Notebooks. Auf diesen laufen dann mehrere Software-Clients für unterschiedliche Dienste. WWW, E-Mail, Messaging, usw.

- [[32_Client-Server-Architektur|Client-Server-Architektur]]

---

# Server
Einfach gesagt ist ein Server ein Computer, welcher Speicher, Daten, Dienste und Rechenleistung in einem Netzwerk zur Verfügung stellt und Zugriffsrechte verwaltet. Über einen Software-Client können Nutzer Dienste und Anwendungen über das Netzwerk anfordern. 

- [[50_Server|Server]]

---

# Router 
Ein Router ist ein Node, mit Routing Funktion. Sprich er leitet (routet) die Pakete, die nicht an ihn selbst gerichtet sind, an die entsprechende Stelle weiter. In einem dezentralen Netzwerk entscheidet der Router bei jedem eingehendem Paket erneut, welchen Weg das Paket geht. 

[[46_Router|Router]]

---

# Routing 
Die Art und Weise, wie Datenpakete in einem dezentralen Netzwerk oder IP-Netzwerk verarbeitet werden, bezeichnet man als Routing. Man könnte Routing auch als Wegfindung bezeichnen. Dabei wird der Weg zum Ziel anhand mehrerer Kriterien (metric) ermittelt. Je mehr Kriterien berücksichtigt werden müssen, desto genauer und gezielter ist der Weg zum Ziel. Aber desto (zeit-)aufwendiger ist die Bestimmung oder Berechnung des Wegs.  
In der Regel ist das maßgebliche Kriterium die Zieladresse und damit der kürzeste bzw. schnellste Weg zum Ziel. In gewisser Weise suchen sich die Datenpakete ihren Weg zum Empfänger selber. Beim Routing geht darum den optimalen Weg vom Sender zum Empfänger zu finden.  
Das maßgebliche Hilfsmittel beim Routing ist die Routing-Tabelle, in der mögliche Routen festgelegt sind.

[[47_Routing|Routing]]
[[|IP-Routing]]

---

# Subnetz
Netzwerk Buch
# Gateway
Ein Gateway ist eine Hardware oder Software oder eine Kombination daraus, die eine Schnittstelle zwischen zwei inkompatiblen Netzwerken darstellt. Das Gateway kümmert sich darum, dass die Form und Adressierung der Daten in das jeweilige andere Format oder Protokoll des anderen Netzes konvertiert werden.

[[49_Gateway|Gateway]]

---

# Bridge
Eine Bridge oder Netzwerkbrücke verbindet zwei Teilnetze, die auf den Schichten 1 und 2 des OSI-Schichtenmodells arbeiten. Für die Hosts im Netzwerk ist die Bridge transparent und bleibt für sie unsichtbar.

Bridges waren ursprünglich dazu gedacht, verschiedene LAN-Arten miteinander zu verbinden, zum Beispiel ein Ethernet- und ein Token-Ring-LAN. Sie spielte eine entscheidende Rolle bei der Verwaltung größerer lokaler Netzwerke, indem sie die Segmentierung unterstützte, um die Größe der Kollisionsdomänen zu begrenzen und das Risiko von Schleifenbildung zu minimieren.
Auf Grund der Unterschiede zwischen den LANs hat dies niemlas gut funktioniert. Verschiedene Rahmenformen erfordern Kopieren und Neuformatierungen, was CPU-Zeit in Anspruch nimmt, eine neue Prüfsumme nötig macht und möglicherweise unentdeckte Fehler aufgrund von defekten Bits im Speicher der Bridge einführt 

Bridges bieten deutlich bessere Performanz als Hubs und die Isolation den Bridge-Ports bedeutet auch, dass Eingabeleitungen mit unterschiedlichen Geschwindigkeiten laufen können, möglicherweise sogar mit sogar mit unterschiedlichen Netztypen.

Ein Switch kann auch als Multiport-Bridge betrachtet werden.

---

# Switching
Beim Switching werden Verbindungen in einem Netzwerk basierend auf Adressen hergestellt. In einem geswitchten Netzwerk wird üblicherweise der Empfängeradresse folgend ein fester Pfad mit definierter Bandbreite bestimmt, über den Datenpakete geleitet werden. Sobald ein Datenpaket gesendet wird, ist der Weg durch das Netzwerk bereits vorherbestimmt.

---

# Protokoll 
In der Netzwerktechnik bezeichnet ein Protokoll den Ablauf einer Kommunikation zwischen zwei Systemen. Diese Protokolle sind üblicherweise einer spezifischen Schicht des OSI-Schichtenmodells zugeordnet.

[[31_Protokolle|Protokolle]]

---

# Domäne
Eine Domäne bezieht sich in der Netzwerktechnik auf ein logisches Subnetz, einen Namensbereich oder ein Objekt, das die höchste Ebene eines Verwaltungsbereichs darstellt. Beispielsweise in einem Unternehmensnetzwerk könnte "firma.local" eine Domäne sein, die alle Computer und Benutzerkonten des Unternehmens umfasst. Insbesondere im Zusammenhang mit Verzeichnisdiensten wie Active Directory und großen lokalen Netzwerken wird häufig von einer Domäne gesprochen.

[[./|Verzeichnisdienste]]

---

# Ressourcen
In der Netzwerktechnik spricht man häufig von Ressourcen. Damit sind in erster Linie Speicherplätze gemeint, auf denen Daten abgelegt werden können. Darüber hinaus zählen auch Drucker, Server und andere Netzwerkgeräte dazu, die zentrale Dienste innerhalb eines Netzwerks bereitstellen.

---

# Datenpaket
In Telekommunikations- und Computernetzwerken wie dem Internet erfolgt die Übertragung von Daten in Form einzelner Datenpakete. Dabei spielt es keine Rolle, ob es sich um Sprachdaten, Videodaten oder andere Informationen handelt. Da Daten nur selten als Ganzes in ein Paket hineinpassen, werden sie vorab in einzelne, kleinere Datenpakete zerlegt. Anschließend werden die Pakete unabhängig voneinander verschickt. Das bietet den Vorteil, dass ein Paket nicht noch einmal geschickt werden muss, falls es verloren geht.

Als Datenpaket wird somit eine **in sich geschlossene Dateneinheit** bezeichnet, welche von einem Sender an einen Empfänger übermittelt wird. Das Verfahren wird auch als **Paketvermittlung** bezeichnet. Struktur, Aufbau und Datenverschlüsselung der einzelnen Datenpakete werden durch das zugrunde liegende Netzwerkprotokoll definiert.

---

# Frame
Ein Frame ist ein logischer Rahmen, der einen Bit-Strom enthält. Frames werden von einer Netzwerkkarte oder einem Netzwerk-Interface über ein Übertragungsmedium gesendet und empfangen. Jeder Frame ist mit Daten sowie einem Protokoll-Header und einem Ethernet-Header versehen. Diese enthalten Start- und Endsequenzen, Kontrollzeichen, Adressen und Prüfsummen. Frames werden auch als Pakete bzw. Datenpakete bezeichnet. Im Zusammenhang mit Ethernet wird ein Datenpaket speziell als Frame bezeichnet.

[[./Netzwerktechnik/2_Übertragungstechniken7_Ethernet-Frame|Ethernet-Frame]]

---

# Datagram 
Ein Datagramm ist **eine in sich geschlossene, unabhängige Dateneinheit, die ohne weitere Verbindungssicherung zwischen zwei Endpunkten (Peer-to-Peer) verschickt** wird. Diese Dateneinheit enthält Informationen, die mittels eines Datagrammdienstes über ein Netzwerk transportiert werden sollen.

Ein IP-Paket, das an den Netzwerk-Adapter (NIC, Network Interface Card) übergeben wird, wird als Datagramm bezeichnet.

---

# Datenstrom / (Data)stream
Ein Datastream oder Stream ist ein Datenstrom aus logisch zusammenhängenden Datenpaketen, die über ein Netzwerk übertragen werden. Die logische Verbindung der Datenpakete erfolgt üblicherweise über die Empfänger-Adresse. Auf der IP-Ebene ist dies die IP-Adresse, während es auf der TCP- oder UDP-Ebene die Portnummer ist. Darüber hinaus können die Datenpakete auch auf der Anwendungsebene eine logische Verbindung zueinander haben.

---

# Port
In der Netzwerktechnik kann ein Port entweder eine physische Verbindung an einem Gerät wie einem Switch oder Router oder eine logische Zuordnung darstellen. Ein Beispiel für Letzteres ist der Netzwerkzugang eines WLAN-Clients über einen WLAN-Access-Point. Bei den Protokollen TCP und UDP fungiert der Port als eine Art Adresse, die die Zuordnung zwischen einem Protokoll und einer Anwendung oder einem Datenstrom ermöglicht. Sowohl logische als auch physische Ports werden oft durch eine Nummer oder Adresse identifiziert.

[[.|TCP- und UDP-Ports]]

---

# Unidirektionale Kommunikation
Unidirektional bedeutet "in eine Richtung". Bei unidirektionaler Kommunikation oder Übertragung zwischen zwei Teilnehmern steht nur ein Kanal zur Verfügung, der ausschließlich in eine Richtung genutzt werden kann. Ein Rückkanal existiert dabei nicht.

---

# Bidirektionale Kommunikation
Bidirektional bedeutet "in beide Richtungen". Bei bidirektionaler Kommunikation oder Übertragung können Signale, Daten oder Informationen in beide Richtungen fließen. Zwischen Sender und Empfänger gibt es zwei Kanäle: einen Hin- und einen Rückkanal. Diese Kanäle werden auch als Upstream und Downstream bzw. Uplink und Downlink bezeichnet. 

Bei bidirektionaler Übertragung unterscheidet man zwischen Halbduplex und Vollduplex. Bei Halbduplex kann jeweils nur ein Kommunikationspartner senden oder empfangen, während bei Vollduplex beide Kommunikationspartner gleichzeitig senden und empfangen können.

---

# Unicast, Multicast, Broadcast und Anycast
- **Unicast:** Unicast-Adressen adressieren genau einen Host. Die Übertragung erfolgt von einem Host zu einem anderen Host.
- **Multicast:** Hinter einer Multicast-Adresse verbergen sich eine ganze Gruppen von Hosts. Die Übertragung erfolgt von einem Host an mehrere Hosts.
- **Broadcast:** Broadcast-Adressen adressieren alle Hosts. Die Übertragung erfolgt von einem Host an alle anderen Hosts.
- **Anycast:** Anycast-Adressen werden von mehreren Hosts in einem Netzwerk verwendet. Die Übertragung erfolgt von einem Host an einen Host aus einer Gruppe bzw. einem Verbund.

[[34_Unicast_Multicast_Broadcast_und_Anycast|Unicast, Multicast, Broadcast und Anycast]]

---

# Tunneling
Tunneling ist ein Verfahren in der Netzwerktechnik, bei dem Datenpakete über ein Netzwerk durch ein anderes transportiert werden. Ein Protokoll kapselt ein anderes, um es durch ein Netzwerk zu leiten, das es normalerweise nicht unterstützt.

---

[[|Tunneling]]
# Masquerading
Masquerading bezeichnet das Verbergen ganzer Netze hinter einer einzigen IP-Adresse.

In SOHO-Umgebungen, die nur eine IP-Adresse vom Internet-Provider erhalten, wird Masquerading oft eingesetzt. Verschiedene Endgeräte im internen Netz nutzen eine Verbindung ins Internet, wobei interne Adressen über NAT (Network Address Translation) auf eine externe Adresse gebündelt werden. Externe Geräte können die internen Rechner nicht direkt ansprechen, da nur eine IP-Adresse von außen sichtbar ist.

---

# Bonding
Beim Bonding werden mehrere physikalisch vorhandene Leitungen zu einer logischen Leitung zusammengeschaltet. In der Regel um eine höhere Geschwindigkeit zu erreichen.

---

# Topologie
Eine Topologie beschreibt die strukturelle Anordnung eines Netzwerks, indem sie festlegt, wie Geräte wie Computer und Router miteinander verbunden sind. Es gibt verschiedene Typen wie Stern, Bus, Ring und Masche, die jeweils unterschiedliche Eigenschaften in Bezug auf Kosten, Ausfallsicherheit und Erweiterbarkeit bieten.

---

# Backbone
Ein Backbone ist die zentrale Übertragungsstrecke in einem Netzwerk, die mehrere Netzknoten verbindet. Diese Knoten dienen als Zugangspunkte zum Backbone und bilden das Kernnetz oder Core Network. In umfangreicheren Netzwerken integriert der Backbone verschiedene Netzwerkstrukturen, um lokale Netze und Hochleistungssysteme miteinander zu verbinden. Der Backbone ist typischerweise redundant ausgelegt, um Ausfallsicherheit zu gewährleisten.

---

# Leitungen und Kabel
Die Begriffe Leitungen und Kabel werden oft fälschlicherweise synonym verwendet, obwohl es einen Unterschied gibt. Kabel sind spezielle Arten von Leitungen, die im Boden oder auf dem Meeresboden verlegt werden. Im Gegensatz dazu sind Leitungen allgemeinere Begriffe, die sowohl Kabel als auch andere Arten von Verbindungen umfassen, die elektrische oder elektronische Signale übertragen.

Umgangssprachlich verwenden die meisten Menschen den Begriff "Kabel", auch wenn sie eigentlich "Leitung" meinen, was technisch korrekter wäre. Diese Verwechslung ist die häufigste sprachliche Ungenauigkeit in den Bereichen Elektrotechnik und Informationstechnik, noch vor der falschen Benennung einer Glühbirne.

Der Begriff "Kabel" ist kurz und daher einfacher auszusprechen, weshalb er in vielen Kontexten verwendet wird, auch wenn er nicht ganz korrekt ist. Zum Beispiel befindet sich auf einer Kabeltrommel keine "Kabel", sondern Leitungen. Jedoch wird man in Fachgeschäften selten den Begriff "Leitungstrommel" finden. Ebenso sagt niemand "Netzwerkleitung", obwohl dies technisch korrekt wäre.

---

![[© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten..md]]