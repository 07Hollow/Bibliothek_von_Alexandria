Netzwerke werden oft nach ihrer räumlichen und geografischen Ausdehnung klassifiziert. Ein LAN (Local Area Network) ist typischerweise ein lokales Netzwerk, das mehrere Computer und Peripheriegeräte innerhalb eines Gebäudes verbindet. Allerdings kann ein LAN auch größere Dimensionen annehmen und wird oft als solches bezeichnet, wenn es privat und nicht öffentlich betrieben wird, selbst wenn es nicht lokal begrenzt ist. Die Teilnehmerzahl in einem LAN ist ebenfalls nicht auf wenige beschränkt; es kann Hunderte oder sogar Tausende von Hosts umfassen, wie es beispielsweise in einem großen Unternehmensnetzwerk der Fall sein kann.

---

# Einfaches Lokales Netzwerk

![[../../../IMG/IMG_IT/einfaches_Lokales_netzwerk.png]]

Ein einfaches Netzwerk besteht aus mindestens zwei Computersystemen, die über eine Direktverbindung (Crossoverkabel) oder ein Kopplungselement (Hub oder Switch) verbunden sind. Sobald mehr als zwei Computersysteme beteiligt sind, ist ein zentrales Kopplungselement erforderlich. Ein solches Kopplungselement, wie etwa ein Switch, stellt die physikalische und logische Verbindung zwischen den Computersystemen sicher.

---

# Ein lokales Netzwerk mit Internet-Zugang 

![[../../../IMG/IMG_IT/lokales_Netzwerk_mit_Internet-Zugang.png]]
_(Bild ohne Print-Server)_

Ein lokales Netzwerk mit Internet-Zugang besteht in der Regel aus einem Switch und einem Router. Der Switch fungiert als Kopplungselement innerhalb des LANs, während der Router den Internet-Zugang ermöglicht und ebenfalls an den Switch angeschlossen ist. Dadurch erhalten alle Teilnehmer im Netzwerk gleichzeitig Zugriff auf das Internet. In kleinen LANs sind Switch und Router oft in einem Gerät kombiniert.

Ein zusätzlicher Print-Server ermöglicht die gemeinsame Nutzung eines Druckers, sodass alle Teilnehmer im Netzwerk darauf drucken können. Der Print-Server kann ein eigenständiges Gerät sein oder im Drucker bzw. in einem Multifunktionsgerät, das Router, Switch und Print-Server integriert, enthalten sein. Solche Geräte sind im Privatbereich und in kleinen Büros üblich.

---

# Lokales Funknetzwerk / Wireless Local Area Network (WLAN)

![[../../../IMG/IMG_IT/WLAN.png]]

Anstelle kabelbasierter Verbindungen kann auch der freie Raum per Funk als Übertragungsstrecke genutzt werden. Ein Wireless LAN (WLAN) ist ein lokales Netzwerk, das einen Wireless Access Point (WAP) als Basisstation und Computersysteme mit eingebauten WLAN-Adaptern (Netzwerkkarten mit Antenne) umfasst. Alle Hosts, die sich in Reichweite der Funksignale befinden, haben Zugang zum Netzwerk. Router und Wireless Access Point sind oft in einem Multifunktionsgerät kombiniert, das als WLAN-Router bezeichnet wird. Diese Geräte werden im Privatbereich und in kleinen Büros eingesetzt.

[[6_WLAN|WLAN]]
[[.\Informatik\Netzwerktechnik\2_Übertragungstechnik\20_IEEE_802_11]]20_IEEE_802_11|IEEE 802.11]]

# Netzwerk-Komponenten in einem LAN

- [[38_Repeater|Repeater / Hub]]
- [[40_Medienkonverter|Medienkonverter]]
- [[41_Bridge|Bridge]]
- [[42_Switch|Switch]]
- [[46_Router|Router]]
- [[49_Gateway|Gateway]]
- [[50_Server|Server]]
- [[52_Proxy|Proxy]]
- [[51_Printserver|Printserver]]

---

# Übertragungssystem für lokale Netzwerke

Für die Vernetzung von lokalen Netzwerken gab es von verschiedenen Herstellern unterschiedliche und inkompatible Techniken. Dabei hat sich gezeigt, dass diese herstellerspezifische Übertragungssysteme aufgrund ihrer Abhängigkeit von einem Hersteller kaum zukunftsträchtig waren und deshalb Techniken für offene, heterogene Netze weichen mussten.

- [SNA von IBM](https://www.bsi.bund.de/DE/Themen/Oeffentliche-Verwaltung/Zulassung/SINA/sina_node.html)
- [DECnet von Digital Equipment](https://de.wikipedia.org/wiki/DECnet)
- [[.\|IPX/SPX von Novell]]

Irgendwann in den 1990er Jahren hat sich Ethernet gegenüber anderen herstellerspezifischen Vernetzungstechniken durchgesetzt. Insbesondere der einfache und kostengünstige Aufbau eines Ethernet-Netzwerks sorgte für die rasche Verbreitung auf der ganzen Welt. Im Prinzip werden heute fast alle Vernetzungen im LAN und auch im WAN auf Basis der IEEE-802-Spezifikationen realisiert.

- [[.\|IEEE 802]]
- [[.\|IEEE 802.3 / Ethernet]]
- [[.\|IEEE 802.11 / WLAN / Wi-Fi]]

---

# Software Defined Networking (SDN)

Software Defined Networking, kurz SDN, umfasst Netzwerk-Komponenten, deren Funktionen individuell programmierbar sind. Diese Technologie ermöglicht es, die Kontrolle über das Netzwerk zentralisiert auszuüben und somit eine übergeordnete Steuerung aller Netzwerk-Komponenten zu gewährleisten. SDN trennt traditionell integrierte Netzwerkfunktionen in zwei Hauptebenen: die Kontrollebene (Control Plane), die die Netzwerkentscheidungen trifft, und die Weiterleitungsebene (Data Plane), die den Datenverkehr entsprechend dieser Entscheidungen weiterleitet. Durch diese Architektur bietet SDN eine verbesserte Flexibilität, Skalierbarkeit und Verwaltbarkeit von Netzwerken im Vergleich zu herkömmlichen Netzwerkarchitekturen.

[[62_SDN|SDN]]

---

# Grenzen zwischen LAN und WAN

Heutzutage macht eine klare Trennung zwischen LAN (Local Area Network) und WAN (Wide Area Network) kaum noch Sinn. Dies liegt hauptsächlich daran, dass viele Ressourcen wie Daten und Dienste nicht mehr ausschließlich im lokalen Netzwerk vorhanden sind, sondern oft extern in Rechenzentren oder in der Cloud gespeichert werden.

Durch die zunehmende Mobilität der Anwender und die Verbreitung von Home Office ist es sinnvoll geworden, Rechenleistung und Datenspeicher zentral zu verwalten und unabhängig von Zeit und Standort bereitzustellen oder abrufen zu können.

Lokale Netzwerke fungieren heutzutage oft nur noch als Zugangspunkte oder Zugangsnetze zum Internet, über die Anwendungen und Dienste in der Cloud zugänglich sind. Sie dienen somit als Schnittstelle zwischen den Endgeräten der Nutzer und den externen Ressourcen, die in der Cloud gehostet werden.

---

# Aktuelle Vernetzungstechniken im Vergleich

| Vernetzungstechnik | Reichweite              | Bandbreite (brutto) | Stream (netto) | Datenrate (netto) |
| :----------------- | :---------------------- | :------------------ | :------------- | :---------------- |
| HomePlug AV        | Wohnung/Einfamilienhaus | 200 MBit/s          | -              | ca. 8 MByte/s     |
| HomePlug AV2       | Wohnung/Einfamilienhaus | 500 MBit/s          | -              | ca. 20 MByte/s    |
| Bluetooth          | Zimmer/Wohnung          | 3 MBit/s            | -              | ca. 2 MByte/s     |
| WLAN IEEE 802.11n  | typ. 20 m               | 600 MBit/s          | 100 MBit/s     | ca. 35 MByte/s    |
| WLAN IEEE 802.11ac | typ. 20 m               | 6.900 MBit/s        | 400 MBit/s     | ca. 50 MByte/s    |
| WLAN IEEE 802.11ax | typ. 20 m               | 9.600 MBit/s        | 500 MBit/s     | -                 |
| Fast-Ethernet      | 100 m                   | 100 MBit/s          | 94 MBit/s      | ca. 10 MByte/s    |
| Gigabit-Ethernet   | 100 m                   | 1.000 MBit/s        | 940 MBit/s     | ca. 100 MByte/s   |
| Gigabit-Ethernet   | 100 m                   | 2.500 MBit/s        | 2.400 MBit/s   | -                 |
| Gigabit-Ethernet   | 100 m                   | 5.000 MBit/s        | 4.000 MBit/s   | -                 |
| Gigabit-Ethernet   | 100 m                   | 10.000 MBit/s       | 6.000 MBit/s   | -                 |

Die tatsächliche Datenrate wird von verschiedenen Faktoren beeinflusst. Optimale Bedingungen sowohl bei der physikalischen Übertragung als auch bei der logischen Kommunikation sind entscheidend. Dies gilt insbesondere für Funkübertragungen, bei denen solche Bedingungen schwer zu realisieren sind.

[[.\|Home-Plug-Powerline]]
[[.\|Bluetooth]]
[[.\|Wi-Fi 4 / IEEE 802.11n / WLAN mit 150 MBit]]
[[.\|Wi-Fi 5 / IEEE 802.11ac / Gigabit-WLAN]]
[[.\|Wi-Fi 6 / IEEE 802.11ax / High Efficiency WLAN]]
[[.\|Wi-Fi 7 / IEEE 802.11be / Extremely High Throughput]]
[[.\|Fast-Ethernet / IEEE 802.3u]]
[[.\|Gigabit-Ethernet / IEEE 802.3ab]]

---

# Sicherheit und Bedrohungslage

In herkömmlichen Netzwerken besteht eine erhebliche Gefahr durch Systeme, die unbekannte Schwachstellen aufweisen und durch menschliches Fehlverhalten kompromittiert werden können. Ein typisches Szenario ist das Öffnen eines infizierten E-Mail-Anhangs oder die Installation einer Software aus einer unsicheren Quelle.

Ein einziger technischer oder menschlicher Fehler kann ausreichen, um einem Angreifer den initialen Zugriff auf das interne Netzwerk zu ermöglichen. Vom kompromittierten System aus kann der Angreifer dann Schadcode auf andere Systeme im Netzwerk verbreiten. Dies geschieht oft, weil die Systeme und Nutzer innerhalb des Netzwerks einander vertrauen und Sicherheitsmaßnahmen teilweise oder vollständig umgangen werden.

Die Bedrohungslage zeigt deutlich, dass interne Systeme oft unzureichend geschützt sind und daher nicht bedingungslos vertrauenswürdig sein können. Es ist daher unerlässlich, dass nicht nur externe Bedrohungen, sondern auch potenziell gefährliche interne Systeme abgesichert werden müssen.

---

![[../../../Template/© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]