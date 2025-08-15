Unter einer Netzwerk-Topologie versteht man die typische Anordnung und physikalische Verbindung von Geräten in einem Netzwerk. Geräte sind Hosts, wie Clients und Server, die das Netzwerk aktiv nutzen. Dazu zählen auch Netzwerkkomponenten wie Switches und Router, die eine Verteilfunktion haben und dafür sorgen, dass alle Netzwerkteilnehmer miteinander eine logische Verbindung eingehen können. Die Netzwerk-Topologie bestimmt dabei die einzusetzenden Komponenten sowie die Zugriffsmethoden auf das Übertragungsmedium.

Die im Folgenden beschriebenen Netzwerk-Topologien beziehen sich auf paketvermittelnde Netzwerke.

- Point-to-Point (PtP) / Punkt-zu-Punkt
- Point-to-Multipoint (PtMP) / Punkt-zu-Mehrpunkt
- Line / Chain / Linie
- Bus
- Ring
- Star / Stern
- Tree / Baum
- Mesh / Vermascht Topologie
- Fully Connected / Vollvermaschte Topologie
- Fabric / Gewebe

---

# Point-to-Point (PtP) / Punkt-zu-Punkt

![[../../../IMG/IMG_IT/point-to-point.png]]

Bei einer Punkt-zu-Punkt-Topologie besteht nur zwischen zwei [Hosts] bzw. Geräten eine einfache und direkte physikalische Verbindung. Diese Geräte können diese Verbindung für ihre gegenseitige Kommunikation nutzen. In einer[ Adhoc-Umgebung] finden die Hosts meist spontan zusammen und kooperieren nicht zwangsläufig dauerhaft miteinander. In einer Netzwerk-Umgebung besteht die physikalische Verbindung und die darauf aufsetzende logische Verbindung in der Regel dauerhaft. Die Punkt-zu-Punkt-Topologie darf nicht mit der [Peer-to-Peer-Architektur] (P2P) verwechselt werden.

Das [Point-to-Point Protocol] (PPP) ist ein Protokoll für die Kommunikation zwischen zwei Computern über eine serielle Schnittstelle. Üblicherweise verbindet sich ein Computer über eine Telefonleitung mit einem [Server]. Zum Beispiel könnte ein Internet-Provider eine PPP-Verbindung anbieten, sodass dessen Server auf persönliche Anfragen reagiert, diese an das Internet weiterleitet und anschließend die angeforderten Informationen an den Benutzer zurückleitet.

PPP verwendet das [Internetprotokoll] (IP), kann aber auch andere Protokolle verwenden. Es wird manchmal als Teil des [TCP/IP-Protokolls] angesehen und fungiert bezogen auf das [OSI-Referenzmodell] als Dienst der zweiten Schicht (Datenverbindungsschicht). Im Wesentlichen bündelt es die TCP/IP-Pakete des Computers und leitet diese an den Server weiter, von wo sie dann ins Internet gesendet werden.

PPP ist ein Full-Duplex-Protokoll, das mit einer Vielzahl unterschiedlicher physikalischer Medien genutzt werden kann, wie Twisted-Pair-Kabel, Lichtwellenleiter oder Satellitenübertragungen. Es verwendet eine Abwandlung des [High-Level Data Link Control] (HDLC) für die Kapselung von [Datenpaketen].

[P2P - Topologie]

---

# Point-to-Multipoint (PtMP) / Punkt-zu-Mehrpunkt

![[../../../IMG/IMG_IT/point-to-multipoint.png]]

Bei einer Punkt-zu-Mehrpunkt-Topologie besteht das Netzwerk aus mehreren Hosts, die sich eine Leitung zum Zentralsystem teilen. Die Kommunikation zwischen den Hosts erfolgt in alle Richtungen, in denen eine Verbindung besteht. Das bedeutet, dass jeder Teilnehmer bis zum Verzweigungspunkt sein eigenes Übertragungsmedium haben kann.

Eine Punkt-zu-Mehrpunkt-Topologie ist eine Form der Stern-Topologie. Ein zentrales Netzwerkgerät verbindet sich einzeln mit weiteren Netzwerkgeräten. Diese angebundenen Geräte sind nicht untereinander verbunden, sondern kommunizieren ausschließlich über das zentrale Netzwerkgerät.

Dabei gibt es eine zentrale Basis und mehrere Stationen. Jede Verbindung von der Basis zu einer einzelnen Station kann als Punkt-zu-Punkt-Verbindung betrachtet werden. Alle verbundenen Stationen teilen sich die verfügbare Bandbreite der Basis. Hinzu kommt ein Overhead durch die Abstimmung von Sendezeitfenstern zwischen den beteiligten Geräten, die länger als im lokalen WLAN sind, da die Abstände und Laufzeiten zwischen den Geräten größer sind. Wie die Stationen um die Basis positioniert sind, hängt von der Antennencharakteristik der Basis ab, da sie die Stationen „hören“ muss. Die Antennen der Stationen können gerichteter sein als die der Basis.

---

# Line / Chain / Linien-Topologie (Linientechnik)

![[../../../IMG/IMG_IT/linien-topologie.png]]

In einer Linien-Topologie sind mehrere Hosts nacheinander in Reihe geschaltet, wobei die beiden Enden der Linie jeweils mit einem Gerät abgeschlossen sind. Entfernt man einen beliebigen Host, führt dies zu einer Unterbrechung der Linie und somit zum Ausfall des Netzwerks. Die entstandene Lücke muss überbrückt oder an der Stelle neu verkabelt werden, was eine Neuordnung der Verkabelung zwischen allen Geräten in Abhängigkeit vom Übertragungsmedium zur Folge hat.

Diese Linien-Topologie wird auch als Daisy-Chain-Konfiguration bezeichnet und findet häufig in der Automatisierungs- und Sicherheitstechnik Anwendung.

Es ist wichtig zu beachten, dass die Linien-Topologie oft mit der Bus-Topologie vermischt wird. Während bei der physikalischen Verkabelung keine Unterscheidung vorgenommen wird, unterscheiden sich die darauf aufbauende Übertragungslogik und das Zugriffsverfahren erheblich.

---

# Bus / Bus-Topologie

![[../../../IMG/IMG_IT/Bus-topologie.png]]

Bei einer Bus-Topologie sind alle Geräte direkt mit demselben Übertragungsmedium, dem Bussystem, verbunden. Dies bedeutet, dass alle Hosts Zugriff auf die Signale haben, die über den Bus übertragen werden.

Um Störungen und Probleme auf der Leitung zu vermeiden und die physikalischen Eigenschaften zu verbessern, sind die beiden Kabelenden mit einem Abschlusswiderstand versehen. Es gibt keine zentrale Netzwerkkomponente, die die Abläufe auf dem Bus regelt. Stattdessen übernimmt ein Zugriffsverfahren die Steuerung der Ablaufprozesse auf dem Bus, an dessen Regeln sich alle Hosts halten. Das Datenprotokoll gibt die Befehle vor, während der Bus selbst nur ein passives Übertragungsmedium darstellt.

---

# Ring / Ring-Topologie

![[../../../IMG/IMG_IT/Ring-Topologie.png]]

In einer Ring-Topologie sind alle Geräte über eine geschlossene Kabelstrecke ringförmig miteinander verbunden. An jedem Host kommt ein Kabel an und geht wieder ab.

Typischerweise ist in der Ring-Topologie keine aktive Netzwerk-Komponente erforderlich. Die Steuerung und der Zugriff auf das Übertragungsmedium werden durch ein Datenprotokoll geregelt, an das sich alle Stationen halten.

Ein Ring-Manager ist jedoch oft vorteilhaft. Dieser ermöglicht den Betrieb eines doppelten Rings, sodass die Ring-Topologie bei einer Unterbrechung an einer Stelle in eine Bus-Topologie umschalten kann.

Die Ring-Topologie zeichnet sich durch eine geschlossene Kabelstrecke aus, bei der die Netzwerk-Teilnehmer über einen durchgehenden Kabelring miteinander verbunden sind. Dies bedeutet, dass an jedem Host ein Kabel ankommt und ein Kabel abgeht. Die Steuerung und der Zugriff auf das Übertragungsmedium werden durch ein Protokoll geregelt, an das sich alle Stationen halten.

Ein Ring-Manager kann sinnvoll sein, da er bei einer Unterbrechung des Rings den Betrieb auf eine Bus-Topologie umschalten kann. Diese Redundanz ist besonders wichtig in Produktionsumgebungen, die auf hohe Verfügbarkeit angewiesen sind.

---

# Star / Stern-Topologie

![[../../../IMG/IMG_IT/Stern-Topologie.png]]

In der Stern-Topologie ist eine zentrale Netzwerk-Komponente vorhanden, die eine physikalische Verbindung zu allen Hosts unterhält. Jeder Host ist über eine separate Leitung mit dieser zentralen Netzwerk-Komponente verbunden, die typischerweise ein Hub oder Switch ist. Diese Komponente übernimmt die Verteilung der Datenpakete, indem sie die Pakete empfängt und an ihre Ziele weiterleitet.

Die Datenbelastung auf der zentralen Verteilerkomponente kann hoch sein, da alle Daten und Verbindungen über sie laufen. Das Netzwerk ermöglicht es, Hosts jederzeit hinzuzufügen oder zu entfernen, ohne den Betrieb des Netzwerks zu beeinträchtigen.

Eine Stern-Bus-Struktur kombiniert die Eigenschaften der Stern- und der Bus-Topologie. Die Stationen sind über eine Sternstruktur mit einem Hub verbunden, während mehrere Switche über eine Busleitung miteinander verbunden sind.

Die Stern-Topologie funktioniert ähnlich wie die Punkt-zu-Mehrpunkt-Topologie, jedoch mit dem Unterschied, dass alle Hosts eine direkte Leitung zur zentralen Netzwerk-Komponente haben. Diese zentrale Komponente, meist ein Hub oder Switch, empfängt Daten und leitet sie gezielt weiter.

Obwohl die Datenbelastung im Zentrum hoch sein kann, beeinflusst das Hinzufügen oder Entfernen von Hosts den Netzwerkbetrieb nicht.

---

# Tree / Baum-Topologie

![[../../../IMG/IMG_IT/Baum-Topologie.png]]

Die Baum-Topologie stellt eine erweiterte Form der Stern-Topologie dar und wird häufig in größeren lokalen Netzwerken eingesetzt, insbesondere wenn mehrere Topologien miteinander kombiniert werden. Typischerweise bildet ein übergeordnetes Netzwerk-Element wie ein Router den Ausgangspunkt, von dem aus sich ein Stamm mit vielen Verzweigungen bildet. Diese Struktur ähnelt einem Baum, daher der Name Baum-Topologie.

In der Baum-Topologie gibt es eine klare Hierarchie, wobei das übergeordnete Netzwerk-Element die Wurzel darstellt und die Verzweigungen zu den einzelnen Netzwerkgeräten führen. Dies ermöglicht eine effiziente Organisation und Verwaltung des Netzwerks, da Daten über den Baum verteilt und geroutet werden können, wodurch die Belastung auf einzelne Teile des Netzwerks reduziert wird.

---

# Mesh / Maschen-Topologie

![[../../../IMG/IMG_IT/Mesh-Topologie.png]]

Bei der Maschen-Topologie, auch vermaschte Topologie genannt, handelt es sich um ein dezentrales Netzwerk, bei dem alle Netzwerkknoten willkürlich miteinander verbunden sind. Es gibt keine festen hierarchischen Strukturen, und nicht jeder Host ist direkt mit jedem anderen Host verbunden. Der Vorteil dieser Topologie liegt in der erhöhten Robustheit und Zuverlässigkeit des Netzwerks:

1. **Erhöhung der Reichweite**: Durch das Netzwerk erhöht sich die Reichweite, insbesondere für Knoten, die am Rand des Netzwerks liegen.

2. **Redundanz bei Verbindungsstörungen**: Im Falle eines Verbindungsfehlers kann der Datenverkehr üblicherweise über alternative Wege fortgesetzt werden. Dies geschieht durch Routing, bei dem aktive Netzwerk-Komponenten wie Router oder Switches die Datenpakete innerhalb des Netzwerks vermitteln.

In einem lokalen Netzwerk ([LAN]) tritt die Maschen-Topologie häufig auf, wenn verschiedene Systeme und verschiedene Topologien miteinander verbunden sind und keine klare Struktur vorgegeben ist.

Ein Beispiel für eine Maschen-Topologie auf einer größeren Skala ist das Internet selbst. Es gibt keine zentrale Instanz, die die gesamte Architektur des Internets steuert. Stattdessen sind die Netzwerkknoten (wie [Server], [Router] und [Switches]) über verschiedene Pfade miteinander verbunden, wodurch eine robuste und flexible Netzwerktopologie entsteht.

---

# Fully Connected /  Vollvermaschte Topologie

![[../../../IMG/IMG_IT/Vollvermaschte-Topologie.png]]

Fully Connected oder vollständig verbunden bezeichnet eine Netzwerk-Topologie, in der jeder Host direkt mit jedem anderen Host über eine eigene physikalische Verbindung verbunden ist. Das bedeutet, dass jeder Host eine [Schnittstelle] für jede mögliche Verbindung benötigt, und es muss für jede dieser Verbindungen ein eigenes Übertragungsmedium vorhanden sein.

Diese Topologie wird auch als Vollvermaschte Topologie bezeichnet. Sie ist theoretisch perfekt, da sie optimale Redundanz und direkte Kommunikationswege zwischen allen Teilnehmern bietet. Jedoch wird Fully Connected in der Praxis nur selten angewendet, da der Aufwand für die Verkabelung und die Bereitstellung der Schnittstellen sehr hoch ist. Es ist nur dann sinnvoll, wenn eine sehr hohe Bandbreite zwischen allen Teilnehmern benötigt wird und die Anzahl der Hosts relativ gering ist.

Die Vollvermaschte Topologie ist besonders in kleinen Netzwerken oder in spezialisierten Anwendungen relevant, wo die direkte und ununterbrochene Kommunikation zwischen allen Netzwerkteilnehmern von entscheidender Bedeutung ist.

---

# Fabric / Geflecht-Topologie (Gewebe)

![[../../../IMG/IMG_IT/Geflecht-Topologie.png]]

Die Geflecht-Topologie ist eine Netzwerkstruktur, bei der alle Hosts direkt miteinander verbunden sind, ohne dass es einen zentralen Knoten gibt. Diese Topologie ist besonders für hochverfügbare verteilte Systeme geeignet und stammt ursprünglich aus der Fibre-Channel-Welt, wo sie in Speichernetzen lange Zeit eingesetzt wurde.

Früher war ein hierarchischer Aufbau und Segmentierung im Netzwerk vorherrschend, besonders im Kontext des vorwiegenden Client-Server-Datenverkehrs. Stern- oder Baum-Topologien mit zentralistischem Ansatz waren die bevorzugte Architektur für Verkabelung und Vernetzung. Heute jedoch hat sich der Datenverkehr stark verändert, mit dynamischen Inhalten und einer zunehmenden Interaktion zwischen Web-, Applikations- und Datenbank-Servern. Dadurch entstehen Datenströme mit unterschiedlichen Charakteristiken, die flexiblere und intelligenter gestaltete Netzwerk-Topologien erfordern.

Das Konzept der Fabric erfüllt alle wesentlichen Anforderungen an moderne Rechenzentrum-Netzwerke:
- Hohe Geschwindigkeit
- Ausfallsicherheit
- Flexibilität
- Einfaches Management

Eine Fabric weist eine Sternstruktur auf, jedoch ohne einen zentralen Knoten. Stattdessen verbindet sie die verteilten Komponenten redundant zu einer strukturiert vermaschten Topologie. Dies macht die Fabric zu einer Grundlage für hochverfügbare verteilte Systeme.

Die Fabric basiert auf Ansätzen aus der Fibre-Channel-Welt und wird als Vorbild für Ethernet im Rechenzentrum genutzt. Sie ist eine verteilte Architektur, die mehrere physische Switches zu einem großen logischen Switch zusammenfasst.

Für die Vernetzung von Gebäuden bedeutet dies den Einsatz weiterer Core-, Etagen- und Access-Switches, die über zusätzliche Verbindungen miteinander verbunden sind. Oft kommen hier Techniken wie Software Defined Networking (SDN) zum Einsatz, um die Netzwerkkonfiguration und -steuerung flexibel zu gestalten.

[SDN]

---

# Vorteile und Nachteile der Grundtopologien

| **Topologie**     | **Vorteile**                                                                      | **Nachteile**                                                                                 |
| ----------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Bus-Topologie     | - einfach installierbar<br>- kurze Leitungen                                      | - Netzausdehnung begrenzt<br>- bei Kabelbruch fällt Netz aus<br>- aufwändige Zugriffsmethoden |
| Ring-Topologie    | - verteilte Steuerung<br>- große Netzausdehnung                                   | - aufwendige Fehlersuche<br>- bei Störungen Netzausfall<br>- hoher Verkabelungsaufwand        |
| Stern-Topologie   | - einfache Vernetzung<br>- einfache Erweiterung<br>- hohe Ausfallsicherheit       | - hoher Verkabelungsaufwand<br>- Netzausfall bei Ausfall oder Überlastung des Hubs            |
| Maschen-Topologie | - dezentrale Steuerung<br>- unendliche Netzausdehnung<br>- hohe Ausfallsicherheit | - aufwendige Administration<br>- teure und hochwertige Vernetzung                             |

---

# Verkabelungsaufwand im Vergleich
Die Verkabelungsaufwände der Bus- und Ring-Topologie sind beträchtlich und sollten nicht unterschätzt werden. Obwohl die Kabelstrecken in diesen Topologien möglicherweise kürzer sind als bei der Stern-Topologie, erfordern sie oft lange und verwinkelte Kabelwege, da jeder Host direkt miteinander verbunden werden muss. Beim Umzug eines Hosts muss das Kabelziehen oft von Grund auf wiederholt werden, was zusätzlichen Aufwand bedeutet.

Im Gegensatz dazu bietet die Stern-Topologie deutliche Vorteile in der Flexibilität der Verkabelung. Zwar ist der Initielaufwand für die Verkabelung etwas höher, da jeder Host direkt mit einem zentralen Switch oder Hub verbunden wird. Jedoch ermöglicht dies eine flexible Nutzung der Kabelstrecken. Verschiedene Netzwerktechniken oder andere Anwendungen können auf denselben Kabelstrecken betrieben werden, ohne dass umfangreiche Umverkabelungen erforderlich sind.

Insgesamt bietet die Stern-Topologie daher eine praktische und flexible Lösung für Netzwerke, insbesondere wenn sich die Anforderungen an die Netzwerkarchitektur mit der Zeit ändern können.

---

# WLAN-Topologie
Eine WLAN-Topologie besteht im wesentlichen aus den drahtlosen Netzteilnehmern, die als WLAN-Clients bezeichnet werden und mindestens einer WLAN-Basisstation, die als Wireless Access Point (WAP) oder einfache nur Access Point (AP) bezeichnet wird.

[WLAN-Topologie]

--- 

![[../../../Template/© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]