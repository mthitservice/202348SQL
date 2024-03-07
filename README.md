# SQL Server Cluster Informationen
(im Rahmen einer Schulung)

## Vorbereitung
[Link zu MS Informationen](https://learn.microsoft.com/en-us/sql/database-engine/availability-groups/windows/prereqs-restrictions-recommendations-always-on-availability?view=sql-server-ver16)

### Dienstkonen vorbereiten:
[Link zu Tutorial](https://www.frankysweb.de/group-managed-service-accounts-gmsa-fuer-tasks-und-dienste/)

### Speicher:
- OS 60GB + 3 x Arbeitsspeicher frei
- Instanz mind 60 GB
- MDF mdf (DB Block)
- LOGS ldf (DB Block) 
- Temp  pro Kern (nx ndf , 1 x leere ldf ) (DB Block) - IO Höchste Arbeitslast !!!
- Backup (Archiv)
- Optional (Ext) ndf (DB Block) 

### Netzwerk:
- Client Netz
- Cluster Netz

### Nach Vorbereitung aber vor der Installation Check der Performance durch IOSIM
[Link Anleitung IO SIM] (https://learn.microsoft.com/de-de/troubleshoot/sql/tools/sqliosim-utility-simulate-activity-disk-subsystem)

### Nach Instalation - Grundlastmessung Performance Monitor
[Link zu Tutorial] (https://www.mssqltips.com/sqlservertutorial/283/performance-monitor/)


[Link zur PDF VMWare SQL Server Clustervorbereitung](https://docs.vmware.com/de/VMware-vSphere/7.0/vsphere-esxi-vcenter-server-702-setup-wsfc.pdf)

### Cluster Architekturen die möglich sind
[Link zur übersichtlichen Clusterarchitektur](https://www.sqlshack.com/an-overview-of-distributed-sql-server-always-on-availability-groups/)

### Fehlersuche
[Link zu den möglichen Problemen] (https://madafa.de/blog/troubleshooting-von-always-on-verfugbarkeitsgruppen)
