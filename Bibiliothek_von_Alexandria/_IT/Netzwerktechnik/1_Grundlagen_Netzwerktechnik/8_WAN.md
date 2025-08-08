![[../../../IMG/IMG_IT/WAN.png]]

Ein Wide Area Network (WAN) ist ein Netzwerk, das über einen großen geografischen Bereich verteilt ist. Im Gegensatz zu lokalen Netzwerken (LANs), die eher begrenzte Gebiete abdecken und häufig innerhalb einer Organisation betrieben werden, wird ein WAN typischerweise von einem Provider oder Telekommunikationsanbieter verwaltet.

In kleinen lokalen Netzen spielt die Auslastung der Netzwerkleitungen oft eine untergeordnete Rolle. Im WAN-Bereich hingegen ist es für Netzbetreiber von großer Bedeutung, dass ihre Leitungen effizient ausgelastet sind. Ungenutzte Kapazitäten bedeuten Kosten ohne entsprechende Einnahmen. Daher sind die Anforderungen an Abrechnungsmodelle, parallele Nutzungsmöglichkeiten und Netzwerkmanagement, insbesondere im Falle von Ausfällen, besonders hoch.

Im WAN-Bereich haben sich spezifische Techniken entwickelt, die primär darauf ausgerichtet sind, LANs miteinander zu verbinden. Diese Techniken haben letztlich zur Entstehung des Internets beigetragen. Zu den klassischen Techniken in WAN-Netzwerken gehören leitungsvermittelte Verbindungen, Punkt-zu-Punkt-Verbindungen, paketorientierte Verbindungen und virtuelle private Netze (VPN).

Diese Techniken ermöglichen es, dass Unternehmen und Organisationen über große Entfernungen hinweg miteinander kommunizieren und Daten austauschen können, unabhängig davon, wo sich die jeweiligen Standorte befinden.

--- 

# MAN - Metropolitan Area Network
Eine Sonderform des Wide Area Network (WAN) ist das Metropolitan Area Network (MAN). Es handelt sich dabei um ein Netzwerk, dass sich über eine große Stadt oder eine Region erstreckt.

---

# WAN-Übertragungssysteme 
[[.\|SDH]]
[[.\|ATM]]
[[.\|FDDI]]
[[.\|RPR]]

---

# SDH/SONET
Weitverkehrsnetze in Europa werden häufig mit der Transporttechnik SDH (Synchronous Digital Hierarchy) betrieben, während in Amerika das äquivalente System SONET (Synchronous Optical Network) verwendet wird. Beide Systeme sind praktisch identisch und teilen die Bandbreite mittels Zeitmultiplexverfahren auf.

SDH und SONET bieten gleiche Geschwindigkeitsstufen an, die jedoch unterschiedlich benannt werden. Diese Technologien wurden ursprünglich entwickelt, um die Netze für den steigenden Bedarf an hohen Bandbreiten, insbesondere für die Sprachtelefonie, fit zu machen.

SDH basiert auf einer europäischen Norm und wurde entwickelt, um die ineffizienten und veralteten Systeme der Sprachtelefonie durch ein effizientes, hierarchisches System für die Datenübertragung zu ersetzen.

---

# ATM - Asynchronous Transfer Mode
ATM (Asynchronous Transfer Mode) ist in der Tat keine reine Übertragungstechnik, sondern eine Netztechnik, die ursprünglich als Basis für ein Breitband-ISDN (B-ISDN) konzipiert wurde, das auch integriertes Kabelfernsehen unterstützen sollte. Heutzutage wird die ATM-Netztechnik als Transportmedium in lokalen, öffentlichen und privaten Hochgeschwindigkeitsnetzwerken eingesetzt.

ATM wurde entwickelt, um verschiedene Arten von Diensten effizient über ein Netzwerk zu transportieren, darunter Sprache, Daten und Video. Es nutzt eine festgelegte Zellgröße von 53 Bytes, was es besonders geeignet macht für Anwendungen, die eine konstante und deterministische Datenübertragung erfordern.

Ursprünglich war ATM als die Zukunft der Netzwerktechnologie angesehen worden, hat jedoch in vielen Bereichen zugunsten anderer Technologien wie Ethernet und IP-basierten Netzwerken an Bedeutung verloren. Dennoch bleibt ATM in bestimmten Bereichen, insbesondere in spezialisierten Hochgeschwindigkeitsnetzwerken und Telekommunikationsinfrastrukturen, weiterhin relevant.

---

# FDDI - Fibre Distributed Data Interface
FDDI (Fiber Distributed Data Interface) ist ein Standard für ein Glasfaser-Datennetzwerk, der nach ISO 9314 1-3 und ANSI ASC X3T9.5 spezifiziert ist. Die Übertragungsgeschwindigkeit ist auf 100 MBit/s begrenzt, und die Netzwerktopologie ist in Form eines einfachen oder doppelten Rings angelegt.

Die maximale Ausdehnung eines FDDI-Netzwerks beträgt 200 km und es können bis zu 1000 Stationen angeschlossen werden. Aufgrund dieser Eigenschaften eignet sich FDDI besonders gut für den Aufbau eines Backbone-Netzwerks. Es ermöglicht die Vernetzung großer Netzwerke miteinander, was es ideal für den Einsatz in umfangreichen und verteilten Netzwerkumgebungen macht.

FDDI bietet eine hohe Zuverlässigkeit und Ausfallsicherheit, da Daten im Ring weitergeleitet werden können, selbst wenn eine Verbindung oder Station ausfällt. Obwohl FDDI heute nicht mehr so weit verbreitet ist wie früher, spielt es immer noch eine Rolle in spezialisierten Anwendungen, insbesondere in Umgebungen, die hohe Bandbreiten und Zuverlässigkeit erfordern.

---

# RPR - Resilient Packet Ring
RPR ist ein 10-GBit-Ethernet, das ein WAN-Interface mitbringt und zu SDH/SONET kompatibel ist.

---

# Software-Defined WAN (SD-WAN)
Ein Netzbetreiber trennt in seinem WAN die Netzsteuerung und Netzfunktionen von ihrer proprietären Hardware. Die Steuerung und Funktionen laufen dann als Software auf Standard-Hardware.

[[63_SD-WAN|SD-WAN]]

--- 

![[../../../Template/© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]