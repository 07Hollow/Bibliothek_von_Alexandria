| WPAN                                  | Bluetooth                                          | ZigBee                          | EnOcean                    | Z-Wave            | UWB                      |
| ------------------------------------- | -------------------------------------------------- | ------------------------------- | -------------------------- | ----------------- | ------------------------ |
| Standard                              | IEEE 802.15.1                                      | IEEE 802.15.4                   | proprietär                 | proprietär        | (IEEE 802.15.3a)         |
| Topologie                             | AdHoc-Netz                                         | Vermaschtes Netz                | Vermaschtes Netz           | Vermaschtes Netz  | Punkt-zu-Punkt           |
| max. Übertragungs-<br>geschwindigkeit | 700 kBit/s                                         | 20 / 40 / 250 kBit/s            | 120 kBit/s                 | 9,6 kBit/s        | 110 / 480 MBit/s         |
| max. Reichweite                       | 10 / 30 / 100 m                                    | 50 m                            | 30 m                       | 20 m              | >3 / <3 m                |
| max. Anzahl der Stationen             | 8                                                  | 65.536                          | 7 (je Bridge)              | 323               | 127 (je Host)            |
| Frequenzen                            | 2,402 bis 2,480 GHz                                | 864,2 MHz  <br>2,4 GHz (Europa) | 868,3 MHz                  | 864,2 MHz         | 3,1 ... 10,6 GHz (UWB)   |
| Anwendungen                           | Datei-Download  <br>Maus, Tastatur  <br>Handy-Sync | Steuerung  <br>Automation       | Steuerung  <br>Sensornetze | Gebäudeautomation | Multimedia (Audio/Video) |

---

WPANs (Wireless Personal Area Networks) bieten einige spezifische Vorteile gegenüber WLANs, insbesondere in kleineren Umgebungen. Durch die Beschränkung auf einen kleineren Raum sind Störungen durch externe Sender weniger wahrscheinlich, was zu einer verbesserten Zuverlässigkeit führt. Zudem ermöglicht die geringere Sendeleistung eine Energieersparnis und verlängerte Akkulaufzeiten, beispielsweise bei Notebooks.

Die Datenübertragungsraten in WPANs sind im Vergleich zu WLANs typischerweise geringer. Zum Beispiel bietet das VFIR-IrDA eine maximale Übertragungsrate von 16 Mbit/s, FIR-IrDA erreicht 4 Mbit/s und Bluetooth bis zu 3 Mbit/s. Im Gegensatz dazu kann WLAN nach dem IEEE 802.11g-Standard Übertragungsraten von bis zu 54 Mbit/s erreichen.

WPANs unterstützen üblicherweise nur Point-to-Point- oder gelegentlich Point-to-Multipoint-Verbindungen. Multipoint-to-Multipoint-Verbindungen sind in den Standards nicht vorgesehen.

Typische Anwendungen für WPANs umfassen die Ad-hoc-Vernetzung von Geräten wie PDAs, Konsolen, Druckern, Notebooks, Netbooks und Mobiltelefonen. Beispiele hierfür sind der Austausch von Visitenkarten nach dem vCard-Standard und die Synchronisation von Kalendereinträgen zur Terminabstimmung. Es besteht jedoch das Risiko von Sicherheitslücken wie Snarfing, wenn Informationen unzureichend geschützt sind.

Für den Aufbau von Netzwerken nach dem ISO-OSI-Modell verwenden WPANs oft eine emulierte serielle Schnittstelle und implementieren einen geeigneten Protokollstapel wie SLIP oder PPP. Im Gegensatz dazu folgen WLANs der Struktur des IEEE 802 und unterscheiden sich nur in den unteren beiden Schichten des OSI-Modells.

Bluetooth bietet zusätzlich einen Audio-Modus, der für Freisprecheinrichtungen und Headsets genutzt wird, während IrDA den IrDA-CONTROL-Standard für Anwendungen wie Fernbedienungen unterstützt. Funkmäuse und -tastaturen können theoretisch über Bluetooth oder IrDA angebunden werden, sind aber häufiger mit proprietären Protokollen verbunden.

---

![[../../../Template/© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2024 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]