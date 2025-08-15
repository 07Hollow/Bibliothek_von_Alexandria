Schichtmodelle sind essenziell, um komplexe Netzwerke besser zu verstehen und zu verwalten. Sie bieten eine klare Struktur, die es ermöglicht, Netzwerkfunktionen, [Protokolle] und Dienste in sinnvolle Abschnitte zu gliedern.

Diese Modelle werden von verschiedenen Organisationen wie der „International Organization for Standardization“ ([ISO]) und der „Internet Engineering Task Force“ ([IETF]) entwickelt und gepflegt. Die bekanntesten Schichtmodelle sind das [OSI-Modell] und das [TCP/IP-Modell], die beide essentiell für die Netzwerkkommunikation sind.

In der Computer- und Netzwerktechnik werden komplexe Kommunikationsvorgänge zwischen Teilnehmern in einzelne Schichten unterteilt. Jede Schicht hat spezifische Aufgaben und Funktionen, die durch Verfahren und Protokolle erfüllt werden. Diese Schichten arbeiten zusammen, um eine effiziente Kommunikation zwischen Systemen zu ermöglichen.

Ein gängiges Beispiel zur Veranschaulichung eines Schichtenmodells ist das Gespräch zwischen Personen, die unterschiedliche Sprachen sprechen. Sie benötigen einen Dolmetscher, um miteinander zu kommunizieren. In einem offenen Schichtenmodell entsprechen die Dolmetscher den Protokollen der verschiedenen Schichten, die sich darauf einigen, wie die Kommunikation erfolgen soll. Der Übertragungsweg könnte dabei eine technische Einrichtung wie Telefon, Fax oder E-Mail sein.

---

# Proprietäre Systeme vs Offene Systeme 

Proprietäre Systeme zeichnen sich dadurch aus, dass Übertragungsweg, Protokolle und Anwendungen von einem einzigen Hersteller stammen. Dies führt in der Regel dazu, dass Details über das System schwer zugänglich sind und das System insgesamt wenig flexibel und transparent ist. Der Anwender ist stark an den Hersteller gebunden, insbesondere wenn es um Problemlösungen, Erweiterungen oder Ersatz geht.

Im Gegensatz dazu sind offene Systeme charakterisiert durch genormte, spezifizierte und offengelegte Übertragungswege, Protokolle und Anwendungen. Dies ermöglicht es jedem, Teile zu nutzen und eigene Implementierungen zu entwickeln. Diese offenen Systeme sind darauf ausgelegt, dass Produkte und Lösungen verschiedener Hersteller miteinander arbeiten können und im besten Fall austauschbar sind. Dies fördert Interoperabilität und Wettbewerb auf dem Markt.

---

# Nachteile von Schichtenmodellen
In einem paketvermittelnden Netzwerk wird bei jeder Schicht, die ein [Datenpaket] durchläuft, ein [Header] hinzugefügt. Dieser Header enthält Informationen, die für die Verarbeitung innerhalb derselben Schicht beim Empfänger entscheidend sind. Jeder Header vergrößert das ursprüngliche Datenpaket um einige Bytes.

Jede Schicht hat [Schnittstellen] zur darüber- oder darunterliegenden Schicht. In einem strengen Schichtenmodell findet keine Verarbeitung über die Grenzen einer Schicht hinaus statt. Im Gegensatz zu hochintegrierten Systemen sind Kommunikationssysteme, die auf Schichtenmodellen basieren, nicht primär auf hohe Geschwindigkeit oder Leistung ausgelegt. Vielmehr geht es um hohe Flexibilität, um Implementierungen der Schichten einfach anpassen und austauschen zu können.

---

# Schichtenmodelle in der Netzwerktechnik

|     |             DoD-Schichtenmodell              |    OSI-Schichtenmodell    |     |
| :-: | :------------------------------------------: | :-----------------------: | :-: |
| 4.  |   Anwendungsschicht  <br>Application Layer   |     Anwendungsschicht     | 7.  |
| 4.  |   Anwendungsschicht  <br>Application Layer   |    Darstellungsschicht    | 6.  |
| 4.  |   Anwendungsschicht  <br>Application Layer   | Kommunikationsschicht<br> | 5.  |
| 3.  |    Transportschicht  <br>Transport Layer     |     Transportschicht      | 4.  |
| 2.  |     Internetschicht  <br>Internet Layer      |    Vermittlungsschicht    | 3.  |
| 1.  | Netzzugangsschicht  <br>Network Access Layer |     Sicherungsschicht     | 2.  |
| 1.  | Netzzugangsschicht  <br>Network Access Layer |  Bitübertragungsschicht   | 1.  |

[DoD-Schichtenmodell]
[OSI-Schichtenmodell]

---

![[../../../Template/© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]