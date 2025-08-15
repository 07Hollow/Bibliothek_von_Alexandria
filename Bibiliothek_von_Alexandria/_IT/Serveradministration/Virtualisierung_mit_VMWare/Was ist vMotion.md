#vMotion #Virtualisierung #Server #Cloud-Computing #Shared-Storage #VM 

#virtuelle_Maschinen #iSCI #SAN #NFS #ESXi #iSCI-SAN #NAS #Network-Attached_Storage #Storage-Attached-Network #RDM #Raw-Device-Mapping #IP-Stack

Eine der wichtigsten Funktionen in der Virtualisierung ist das unterbrechnungslose Verschieben von laufender virtueller Maschinen von einem Server auf einen anderen. Im Cloud-Computing bildet das die Grundlage aller Betriebsmodelle. 

# Shared Storage
Das verlagern von Workloads auf einen anderen ESXi-Host, funktioniert nur dann, wenn die virtuellen Disks der VM während des Umzugs für Quell- und Ziel-Host zugreifbar sind. Die verknüpfte virtuelle Festplatte verbleibt nämlich im selben Verzeichnis des Speichers, den beide Hosts gemeinsam verwenden.

Das setzt neben einem Cluster-fähigen Dateisystem ein Shared Storage voraus. Dies kann ein Fibre-Channel- bzw. iSCSI-SAN oder ein NAS mit NFS sein. Auch vSAN kommt dafür in Frage.

vMotion überträgt den gesamten Zustand der virtuellen Maschine auf den neuen Host (Arbeits­speicher, CPU-Register, Netzwerk­verbindungen). Anschließend nimmt die virtuelle Maschine ihre Aktivität wieder auf.

# Voraussetzung für das Netzwerk 
Die wichtigste Voraussetzung ist das vCenter, welches vorhanden sein muss. 
Außerdem braucht man ein vMotion-Netzwerk, bei dem das Service-Tag für vMotion gesetzt ist. Dieses benötigt je einen VMKernel-Adapter pro Host im gleichen Layer-2-Segment bzw. VLAN und im gleichen Layer-3-Subnetz.

Das vMotion-Netzwerk existiert dann neben anderen System-Traffic-relevanten VM-Kernel-Adaptern, wie Management, IP-Storage oder vSAN sowie dem VM-Traffic.

Bezüglich der Portgruppe gibt es zusätzliche Voraussetzungen für das VM-Netzwerk. In der Vergangen­heit musste diese auf dem Quell- und Ziel-Host mit identischem Namen existieren. Inzwischen kann der Nutzer im vMotion-Dialog aber das Zielnetzwerk auch auswählen.

Darüber hinaus verfügt ab vSphere 6.x jeder Host über einen zweiten TCP/IP-Stack, der für die Migration von vSphere vMotion vorgesehen ist.

Eine zusätzliche Voraussetzung für vMotion besteht darin, dass eine VM keine aktive Verbindung zu einem internen virtuellen Switch hat. Die Migration einer solchen virtuellen Maschine führt zu einem Fehler.

Ferner darf keine CPU-Affinität für den virtuellen Prozessor konfiguriert sein. Auch sollte die VM mit keinem virtuellen Gerät wie einer CD/DVD oder einem Disketten­laufwerk verbunden sein, auf dem ein lokales Image gemountet ist.

Kann der Ziel-Host nicht auf die Auslagerungs­datei der VM zugreifen, dann muss vSphere vMotion in der Lage sein, für den Ziel-Host eine neue zu erstellen, bevor die Migration startet. Wird Raw Device Mapping (RDM) verwendet, dann muss der Ziel-Host auf die RDM-Datei und die LUN, der diese Festplatte zugeordnet ist, zugreifen können.

Auch sind so genannte Monster-VMs (sehr viele vCPUs, virtuelle Festplatten mit mehr als 2TB) für vMotion in der Regel problematisch.

Es gilt zudem, dass pro angeschlossenem VMFS-, VVOL, VSAN- oder NFS-Datenspeicher maximal 128 gleichzeitige Migrationen durch vSphere vMotion möglich sind. Es bedarf mindestens eines 1-GBit-Ethernet-Adapters für das vMotion-Netzwerk (nicht das VM-Netzwerk). Damit sind maximal 4 gleichzeitige vMotion-Vorgänge möglich, 10  GBit/s erlauben bis 8 gleichzeitige Migrationen.

![[../../../IMG/IMG_IT/zweiter_IP-Stack_vMotion.png]]
*optionaler zweiter TCPIP-Stack für den vMotion-Traffic kann die VM-Migration beschleunigen.*

Jeder aktive vMotion-Prozess erfordert einen Mindest­durchsatz von 250 MBit/s auf dem Netzwerk. Um vMotion eine bessere Leistung zu ermöglichen, weist man dem vMotion-Netzwerk in einem Multi-NIC-Setup am besten zwei Portgruppen zu.

Schließlich erfordert vMotion auf dem Quell- und Ziel-Host kompatible CPUs, die Funktions­sätze der Prozessoren beider Server müssen kompatibel sein. Die lizenz­seitigen Voraus­setzungen für vMotion sind schnell geklärt: Man braucht mindestens vSphere Essentials Plus.

> Weiterführende Links:
> [VMware vMotion: Funktionsweise und Voraussetzungen | WindowsPro](https://www.windowspro.de/thomas-drilling/vmware-vmotion-funktionsweise-voraussetzungen)

---

![[../../../Template/© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]