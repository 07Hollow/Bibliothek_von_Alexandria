Das DoD Internet Architecture Model (auch bekannt als TCP/IP Model) ist eine Schichtenarchitektur für Netzwerkprotokolle, die Ende der 1960er Jahre von der [DARPA](https://www.darpa.mil/) für das Verteidigungsministerium der Vereinigten Staaten entwickelt wurde. Es besteht aus vier Schichten und wurde im Rahmen der [ARPANET]-Entwicklung eingeführt, um eine robuste, dezentrale Netzwerkstruktur zu schaffen. Ähnlich dem [OSI-Referenzmodell] teilt das DoD-Modell die Aufgaben der Datenübertragung in verschiedene Schichten auf und verwendet eine Reihe von Protokollen, um diese Aufgaben zu lösen. Es dient als Grundlage für das Internet, das ebenfalls aus mehreren miteinander verbundenen Schichten besteht.

---

# 1. Netzzugangsschicht (Network Access Layer) 
Diese Schicht regelt die physische Übertragung der Daten zwischen den Rechnern und Prozessen. Hier werden das Übertragungsmedium (wie Kupferkabel oder Funknetz), der [Leitungscode] (z.B. RZ-Code, NRZ-Code) und das Zugriffsprotokoll (z.B. [Ethernet], V.24) festgelegt.

---

# 2. Internetschicht (Internet Layer) 
Protokolle auf dieser Schicht ermöglichen die netzwerkweite Adressierung, unabhängig vom Übertragungsmedium. Jeder Rechner oder Netzwerkkarte wird eine [[IP|Netzwerkadresse]].

---

# 3. Transportschicht (Transport Layer)
Diese Schicht kontrolliert den Datenfluss zwischen den Anwendungen auf den verschiedenen Rechnern. Die Protokolle [TCP] (Transmission Control Protocol) und [UDP] (User Datagram Protocol) sind hierbei von Bedeutung. TCP bietet eine verbindungsorientierte, zuverlässige Datenübertragung mit Kontrollmechanismen, während UDP eine verbindungslose, weniger aufwendige Datenübertragung ohne Verbindungskontrolle ermöglicht.

---

# 4. Process-Schicht (Application Layer)
Hier werden die eigentlichen Nutzdaten der Anwendungen definiert und aufgebaut. Protokolle wie [HTTP] für Webseiten, [FTP] für Dateiübertragungen und [SMTP] für E-Mails gehören zu dieser Schicht.

---

# DoD vs. OSI
Das DoD-Schichtenmodell und das OSI-Schichtenmodell sind zwei Ansätze zur Strukturierung von Netzwerkprotokollen. Das DoD-Modell, entwickelt in den 1960er Jahren, besteht aus vier festen Schichten und bildet die Basis des Internets. Es ist weniger flexibel als das OSI-Modell, das später entwickelt wurde und sieben Schichten umfasst, die detaillierter und modularer sind. TCP/IP-Protokolle sind eng mit dem DoD-Modell verbunden, was Flexibilität bei den Anwendungen und Übertragungsmedien erlaubt, jedoch sind die Protokolle in den anderen Schichten fest vorgegeben.

---

![[../../../Template/© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]