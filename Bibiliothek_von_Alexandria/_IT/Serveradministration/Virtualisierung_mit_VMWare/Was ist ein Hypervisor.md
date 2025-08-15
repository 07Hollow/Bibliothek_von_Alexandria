#Hypervisor #VM #Betriebssystem #OS #Komponenten #Ressourcen #virtuelle_Maschinen 

#Virtualisierung
# Überblick 
Ein Hypervisor verwaltet die Ressourcen eines Computers und weist diese dann virtuellen Maschinen neu zu.

Ein Hypervisor ist wie eine Art Aufsichtsperson, die sich darum kümmert, dass jede VM ihre Komponente bekommt. 

Bei Verwendung als Hypervisor wird die physische Hardware als Host bezeichnet. Die vielen VMs, die seine Ressourcen nutzen, sind Guests.

# Wie funktioniert ein Hypervisor
Hypervisoren benötigen zur Ausführung der VMs einige Komponenten auf Betriebssystemebene, zum Beispiel einen Speichermanager, Prozessplaner, Input/Output-Stack (I/O), Gerätetreiber, Sicherheitsmanager, Netzwerk-Stack und mehr.

Der Hypervisor stellt den einzelnen virtuellen Maschinen die zugewiesenen Ressourcen zur Verfügung und verwaltet die Planung der VM-Ressourcen im Verhältnis zu den physischen Ressourcen. Die physische Hardware übernimmt nach wie vor die Ausführung, das heißt die CPU führt nach wie vor CPU-Befehle aus, wie sie beispielsweise von den VMs angefordert werden, während der Hypervisor die Planung übernimmt.

Mehrere unterschiedliche Betriebssysteme können nebeneinander ausgeführt werden und sich dieselben virtualisierten Hardwareressourcen mit einem Hypervisor teilen. Dies ist ein zentraler Vorteil der Virtualisierung. Ohne Virtualisierung können Sie nur ein Betriebssystem auf der Hardware ausführen.

# Hypervisor Typ 1 und Typ 2
Es gibt zwei verschiedene Typen von Hypervisoren. Diese sind vom Typ 1 und Typ 2.

Was die Hypervisor gemeinsam haben, ist, dass sie die VMs voneinander Isolieren. Das erhöht die Sicherheit und sorgt dafür, dass sich die VMs nicht untereinander beeinflussen. 

Im großen und Ganzen unterscheiden sich die Hypervisor darin, dass der Typ ein im Gegensatz zum Typ 2 kein darunterliegendes System erfordert. 

**Hypervisor Typ 1:** Dieser wird auch Bare-Metal-Hypervisor genannt, da dieser direkt auf der physischen Hardware läuft und kein darunterliegendes Betriebssysteme erfordert. Der Vorteil ist eine leistungsstarke und Effiziente Lösung für die Virtualisierung.

**Hypervisor Typ 2:** Auch unter dem Namen Hosted Hypervisor bekannt ist eine Virtualisierungstechnologie, welche als Anwendung auf einem bereits vorhandenen OS, dem Host-OS läuft. Vorteile sind eine unkompliziertere Einrichtung, da bereits bestehende Treiber und Dienste genutzt werden, von denen der Hypervisor profitiert. Nachteil ist natürlich eine Leistungseinbußung im Vergleich zum Typ 1, da Hypervisor sich die Ressourcen mit dem Host-OS teilt. 

# Hypervisor im Vergleich 
| Hypervisor            | Typ | Vorteile                                                                                                                                                                                                                                                                                                                                             | Website                                                                                                                         |
| --------------------- | --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| VMWare vSphere (ESXi) | 1   | Hohe Verfügbarkeit und Leistungsfähigkeit<br>Unterschiedliche Lizenzoptionen<br>Unterstützt viele Betriebssysteme<br>Umfangreiches Management und viele Konfigurationsmöglichkeiten<br>Gute Integration in Cloud-Umgebungen                                                                                                                          | [VMware vSphere](https://www.vmware.com/products/cloud-infrastructure/vsphere?pubDate=20250802)                                 |
| Microsoft Hyper-V     | 1   | Nahtlose Integration in Windows-Umgebungen<br>Erweiterte Sicherheitsfunktionen wie Shielded VMs<br>Unterstützt viele Betriebssysteme<br>Hohe Skalierbarkeit und Flexibilität, besonders in privaten Clouds                                                                                                                                           | [Hyper-V Technologieübersicht](https://learn.microsoft.com/de-de/windows-server/virtualization/hyper-v/overview?pivots=windows) |
| Citrix                | 1   | Erweiterte Funktionen wie XenServer Conversion Manager und Memory Optimization, die die Handhabung und Verfügbarkeit verbessern<br>Gut für Anwendungs- und Desktopvirtualisierung geeignet, insbesondere durch die Integration in bestehende Citrix-Produkte wie Citrix Virtual Apps and Desktops, was die Verwaltung und Bereitstellung erleichtert | [Download Citrix Hypervisor - Citrix](https://www.citrix.com/downloads/citrix-hypervisor/)                                      |
| KVM                   | 1   | Hohe Effizienz durch Integration im Linux Kernel<br>Ideal für Cloud-Umgebungen<br>Multiplattform-Support                                                                                                                                                                                                                                             | [KVM hypervisor: a beginners’ guide](https://ubuntu.com/blog/kvm-hyphervisor)                                                   |
| Proxmox               | 1   | Open-Source<br>flexible Lizenzmodelle<br>Zentrale Verwaltung<br>Hohe Flexibilität<br>Skalierbar<br>Snapshotfunktionen                                                                                                                                                                                                                                | [Proxmox - Open-Source Server Solutions](https://www.proxmox.com/de/)                                                           |
| PowerVM               |     |                                                                                                                                                                                                                                                                                                                                                      |                                                                                                                                 |
| Oracle VM             |     |                                                                                                                                                                                                                                                                                                                                                      |                                                                                                                                 |
| Qemu                      |     |                                                                                                                                                                                                                                                                                                                                                      |                                                                                                                                 |

[💬1 - Welche Hypervisoren gibt es und welcher Hypervisor ist der beste?](https://serverhero.de/wissen/vergleich-hypervisor-vmware-hyper-v)

> Weiterführende Links:
> [Was ist ein Hypervisor? Funktion, Vorteile, Typ 1 und 2](https://www.redhat.com/de/topics/virtualization/what-is-a-hypervisor)
> [Hypervisor Typ 1 und 2: Das sind die Unterschiede - IONOS](https://www.ionos.de/digitalguide/server/knowhow/hypervisor-typ-1-vs-2/)

---

![[../../../Template/© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.|© 2025 Bibliothek von Alexandria. Alle Rechte vorbehalten.]]