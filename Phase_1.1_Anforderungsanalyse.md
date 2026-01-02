# Phase 1.1: Anforderungsanalyse
## ITA Abschlussprojekt - Client-Server-Netzwerkinfrastruktur

**Datum:** 2025-01-02  
**Status:** Erledigt  
**Zeitaufwand:** 3 Stunden

---

## 1. Lastenheft vollständig durcharbeiten

### 1.1 Projektübersicht
- **Projekt:** Planung und Implementierung einer zielgruppenorientierten Client-Server-Netzwerkinfrastruktur
- **Lernfeld:** 5 - Rechnernetze nach Vorgaben einrichten
- **Projektdauer:** 100 Stunden
- **Abgabeschluss:** 15.12.2025

### 1.2 Ausgangssituation
- Mittelständisches Unternehmen mit 30-50 Mitarbeitern
- Bestehende IT-Infrastruktur ist veraltet oder nicht vorhanden
- Ersatz durch professionelle Client-Server-Architektur erforderlich

### 1.3 Zielsetzung
- Planung einer vollständigen IT-Netzwerkinfrastruktur mit Fokus auf Zuverlässigkeit und Skalierbarkeit
- Entwicklung eines durchdachten Sicherheitskonzepts
- Praktische Umsetzung einer funktionsfähigen Proof-of-Concept-Umgebung
- Dokumentation aller Planungs- und Implementierungsschritte
- Demonstration der erworbenen Kenntnisse im Bereich Netzwerktechnik

### 1.4 Funktionale Anforderungen (Lastenheft)

#### Netzwerkinfrastruktur
- Aufbau einer strukturierten Client-Server-Architektur
- Virtualisierungsumgebung für flexible Server-Bereitstellung
- Zentrale Datenspeicherung über NAS-System
- Netzwerksegmentierung für verschiedene Unternehmensbereiche

#### Serverdienste
- Cloud-Dienst für zentrale Dateiablage und Synchronisation
- Backup- und Recovery-Lösungen
- Zentrale Benutzerverwaltung und Authentifizierung
- Monitoring und Management-Tools

#### Client-Anbindung
- Unterstützung für Standard-Clients
- Zentrale Verwaltungsmöglichkeiten
- Netzwerkzugriff auf zentrale Ressourcen

### 1.5 Nicht-funktionale Anforderungen (Lastenheft)

#### Performance
- Gigabit-Ethernet als Standard für Client-Anbindung
- Akzeptable Latenzzeiten im lokalen Netzwerk
- Schnelle Verbindungen zwischen Server-Komponenten

#### Verfügbarkeit
- Ausfallsicherheit durch Virtualisierung
- Stabile Netzwerkverbindungen
- Backup-Konzept mit definierten Recovery-Zeiten

#### Sicherheit
- Firewall mit Zugriffskontrolle
- Verschlüsselte Datenspeicherung für sensible Daten
- Netzwerksegmentierung durch VLANs
- Regelmäßige Sicherheitsupdates

#### Skalierbarkeit
- Erweiterbarkeit für zusätzliche Arbeitsplätze
- Flexible Storage-Erweiterung
- Modularer Aufbau der Infrastruktur

### 1.6 Rahmenbedingungen

#### Technische Rahmenbedingungen
**Theoretische Planung:**
- Vollständige Enterprise-Infrastruktur ohne Budgetbeschränkung
- Skalierbare Architektur für Wachstum
- Berücksichtigung aktueller Standards und Best Practices

**Praktische Umsetzung (Mindestausstattung):**
- 1x Hypervisor-Server
- 1x Router mit Firewall-Funktionen
- 1x NAS-System
- Netzwerkkabel und Switches nach Verfügbarkeit
- Optional: Client-Systeme zur Demonstration

#### Organisatorische Rahmenbedingungen
- Projektdurchführung gemäß definierter Phasen
- Abschlusspräsentation mit PowerPoint und Beamer
- Dokumentation aller Planungs- und Implementierungsschritte
- Zeitbudget: 100 Stunden

### 1.7 Systemarchitektur (Überblick)

#### Netzwerktopologie
- Management-Netz für Verwaltungsaufgaben
- Storage-Netz für Datenspeicherung
- Server-Netz für virtuelle Maschinen und Dienste
- Client-Netz für Endanwender

#### Server-Infrastruktur
- Virtualisierungs-Host für flexible Server-Bereitstellung
- Separate Netzsegmente für verschiedene Aufgaben
- Zentrales Storage-System für Datenablage

#### Sicherheitsarchitektur
- Firewall für Zugriffskontrolle
- Verschlüsselung sensibler Verbindungen
- Netzwerksegmentierung durch VLANs

### 1.8 Benutzergruppen
- Administratoren mit Vollzugriff auf alle Systeme
- Gäste mit eingeschränktem Internetzugang
- Fachabteilungen mit Zugriff auf spezifische Ressourcen

### 1.9 Projektphasen (Lastenheft)
1. Planung und Recherche (ca. 20 Std.)
2. Theoretische Durchführung (ca. 35 Std.)
3. Praktische Durchführung (ca. 30 Std.)
4. Präsentationserstellung (ca. 5 Std.)
5. Auswertung und Ausblick (ca. 10 Std.)

---

## 2. Pflichtenheft analysieren

### 2.1 Soll-Kriterien (Zwingende Anforderungen)

#### Theoretische Planung (Soll)
- Vollständige Dokumentation der Netzwerkarchitektur
- IP-Adressplan für alle Netzwerkbereiche
- VLAN-Design mit mindestens 3 Segmenten
- Sicherheitskonzept mit Firewall-Regeln
- Backup-Strategie

#### Praktische Umsetzung (Soll)
- Installation und Konfiguration eines Hypervisors
- Integration eines NAS-Systems mit Dateifreigaben
- Betrieb von mindestens 2 virtuellen Maschinen
- Konfiguration eines Routers mit Firewall-Funktionen
- Netzwerkverbindung zwischen allen Komponenten
- Cloud-Dienst für zentrale Dateiablage funktionsfähig
- Zentrale Benutzerverwaltung implementiert

#### Serverdienste (Soll)
- Cloud-Lösung für Dateisynchronisation und -ablage
- Basis-Monitoring der Infrastruktur
- Zentrales Authentifizierungssystem für Benutzerverwaltung

#### Sicherheit (Soll)
- Firewall-Konfiguration mit Zugriffskontrolle
- Sichere Administrationszugänge (SSH, HTTPS)
- Netzwerksegmentierung durch VLANs

### 2.2 Kann-Kriterien (Optional)
- VPN-Lösung für Remote-Zugriff
- Automatisierte Backup-Jobs mit Benachrichtigungen
- Erweiterte Monitoring-Lösung mit Grafana-Dashboards
- Container-Plattform (Docker/Kubernetes)
- WLAN-Integration mit Access Points
- Hochverfügbarkeits-Features (HA)

### 2.3 Abgrenzungskriterien (Nicht im Scope)
- Beschaffung und Kauf von Hardware
- Client-Hardware oder End-User-Geräte
- Beschaffung kommerzieller Software-Lizenzen
- Langfristiger Produktivbetrieb nach Projektende
- Desktop-Anwendungen oder Client-Software
- Telefonie-Infrastruktur (VoIP)
- ERP-, CRM- oder andere Business-Systeme

### 2.4 Systemarchitektur - Detailplanung

#### Netzwerk-Topologie (VLAN-Design)
- **VLAN 1:** Management (192.168.1.0/24)
- **VLAN 10:** Server-Infrastruktur (192.168.10.0/24)
- **VLAN 20:** Storage-Netzwerk (192.168.20.0/24)
- **VLAN 100:** Client-Netzwerk (10.0.100.0/24)

#### Hardware-Spezifikation (Praktische Mindest-Implementierung)
- Router mit Firewall-Funktionen oder dedizierte Firewall-VM
- Server-Hardware nach Verfügbarkeit
- Virtualisierungsplattform (z.B. Proxmox VE, VMware ESXi)
- NAS-Hardware nach Verfügbarkeit
- RAID-Konfiguration für Datensicherheit
- NAS-Betriebssystem (z.B. TrueNAS, OpenMediaVault)
- Optional: Managed Switch für VLAN-Unterstützung

#### Software-Komponenten
- **Hypervisor:** Proxmox VE (Type-1-Hypervisor, Open Source)
- **NAS-Betriebssystem:** TrueNAS Core (ZFS-Dateisystem)
- **Virtuelle Maschinen:**
  - VM 1: Cloud-Dienst (Nextcloud, ownCloud)
  - VM 2: Zentrale Benutzerverwaltung (LDAP, FreeIPA)
  - VM 3: Monitoring-Server (Zabbix, Prometheus/Grafana)
- **Firewall:** pfSense oder OPNsense als Firewall-VM

### 2.5 IP-Adressplan (Beispiel)
- **Management-Netz (VLAN 1):**
  - 192.168.1.1 - Router/Gateway
  - 192.168.1.30 - NAS Management-Interface
  - 192.168.1.20 - Hypervisor Management-Interface

- **Server-Netz (VLAN 10):**
  - 192.168.10.1 - Virtual Router (pfSense VM)
  - 192.168.10.30 - Monitoring Server VM
  - 192.168.10.20 - Dateiserver VM

- **Storage-Netz (VLAN 20):**
  - 192.168.20.10 - Hypervisor Storage-Interface
  - 192.168.20.20 - NAS Storage-Interface

- **Client-Netz (VLAN 100):**
  - 10.0.100.1 - Gateway
  - 10.0.100.50-250 - DHCP-Bereich

### 2.6 Storage-Konzept
- **RAID-Setup:** RAID 5 für Datenintegrität
- **Storage-Pools:**
  - Pool 1: Produktivdaten (NFS/SMB)
  - Pool 2: Backups (NFS für Proxmox Backup)
  - Pool 3: ISO-Images und Templates
- **Protokolle:** NFS v4 für Linux-VMs, SMB/CIFS für Windows-Clients

### 2.7 Backup-Strategie
- **Proxmox Backup:**
  - Automatische VM-Backups auf NAS
  - Backup-Window: 02:00-06:00 Uhr
  - Retention: 7 Tage täglich, 4 Wochen wöchentlich
- **NAS-Backup:**
  - Snapshots: Stündlich (24h), täglich (7d), wöchentlich (4w)

### 2.8 Sicherheitskonzept
- Strikte VLAN-Trennung
- Storage-VLAN komplett isoliert
- Firewall zwischen allen Segmenten
- Port-basierte Zugriffskontrolle
- Firewall-Regeln nach Least-Privilege-Prinzip
- Minimale Installation ohne unnötige Services
- Starke Passwort-Richtlinien
- SSH-Key-basierte Authentifizierung
- TLS für alle Web-Services

### 2.9 Monitoring und Management
- Monitoring-Lösung: Zabbix / Prometheus + Grafana
- Alerting via E-Mail
- Überwachte Metriken: CPU, RAM, Disk, Network, Services
- Zentrale Log-Sammlung
- Log-Retention: 90 Tage

### 2.10 Dokumentation
- Netzwerk-Topologie-Diagramm (physisch und logisch)
- VLAN-Konfiguration
- IP-Adressplan
- Hypervisor-Konfiguration
- NAS-Konfiguration und Share-Berechtigungen
- VM-Inventar mit Ressourcen und Zweck
- Firewall-Regelwerk
- Backup- und Recovery-Verfahren
- Administrator-Handbuch

### 2.11 Testing und Validierung
- Netzwerk-Tests (VLAN-Isolation, Latenz, Bandbreite)
- Hypervisor-Tests (VM-Erstellung, Ressourcen-Limits, Snapshots)
- Storage-Tests (Lese-/Schreibgeschwindigkeit, Backup/Recovery)
- Performance-Tests (iperf3, sysbench, fio)
- Sicherheits-Tests (Nmap, VLAN-Isolation, Firewall-Regeln)

### 2.12 Implementierungs-Roadmap (8 Phasen)
1. Vorbereitung (5 Std.)
2. Basis-Installation (8 Std.)
3. Netzwerk-Konfiguration (6 Std.)
4. Storage-Setup (4 Std.)
5. VM-Deployment (6 Std.)
6. Service-Konfiguration (8 Std.)
7. Testing und Dokumentation (8 Std.)
8. Optimierung (5 Std.)

---

## 3. Ausgangssituation dokumentieren

### 3.1 Unternehmen: Planova Ingenieurplanung GmbH

#### Unternehmensprofil
- **Größe:** Mittelständisches Ingenieur- und Planungsunternehmen
- **Mitarbeitende:** Etwa 40 Mitarbeitende
- **Standort:** Niedersachsen
- **Fachbereiche:**
  1. Architektur und Entwurf
  2. Technische Gebäudeausrüstung (TGA)
  3. Statik und Konstruktion
  4. Verwaltung und Geschäftsführung

#### Geschäftstätigkeit
- Spezialisierung auf Hochbau-, Infrastruktur- und Infrastrukturprojekte
- Auftraggeber: Kommunale und gewerbliche Kunden
- Täglich entstehen große Mengen an Projektunterlagen:
  - Zeichnungen (CAD-Dateien)
  - Berechnungen
  - Kostenkalkulationen
  - Verträge
  - Angebote
  - Genehmigungsdokumente
  - Fotodokumentationen

### 3.2 Aktuelle Problemstellung

#### Problem 1: Dezentrales Speichern ohne klare Struktur
- Projektunterlagen werden dezentral auf lokalen Festplatten gespeichert
- Unstrukturierte Netzfreigaben auf veraltetem Desktop-PC im "Serverraum"
- **Folgen:**
  - Schwierige Findbarkeit von Dokumenten über Abteilungen hinweg
  - Versionswirrwarr und Unklarheiten über aktuelle Dokumentenstände
  - Fehlender Überblick über Datenverlauf und Änderungen

#### Problem 2: Fehlende zentrale Benutzerverwaltung
- Keine durchgehende zentrale Authentifizierung und Autorisierung
- Jeder Rechner verwaltet lokal seine Benutzer und Berechtigungen
- **Folgen:**
  - Inkonsistenter Zugriffschutz
  - Hoher administrativer Aufwand bei Neueinstellungen und Kündigungen
  - Schwächen beim Schutz sensibler Kundendaten (Pläne, Verträge, persönliche Daten)

#### Problem 3: Unzureichende Datensicherung
- Datensicherungen werden manuell und unregelmäßig auf USB-Festplatten durchgeführt
- **Folgen:**
  - Hohe Ausfallrisiken bei Hardware-Fehlern
  - Keine automatisierten, zuverlässigen Recovery-Verfahren
  - Wiederholte Arbeitsverluste bei Systemausfällen des Server-PCs

#### Problem 4: Fehlende Netzwerksegmentierung
- Netzwerk ist nicht strukturiert
- Alle Geräte können potenziell auf alle anderen zugreifen
- **Folgen:**
  - Sicherheitsrisiken durch mangelnde Segmentierung
  - Fehlende Isolierung sensibler Verwaltungs- und Kundendaten
  - Schwieriges Monitoring und Troubleshooting bei Ausfällen

#### Problem 5: Performance- und Verfügbarkeitsprobleme
- Alter Server-PC ist oft überfordert
- Backups laufen unkontrolliert und blockieren das Netzwerk
- **Folgen:**
  - Gelegentliche Netzwerk-Ausfälle, die Arbeitspausen nach sich ziehen
  - Frustration bei den Mitarbeitenden
  - Reputationsschäden bei verspäteten Projektabgaben wegen IT-Ausfällen

### 3.3 Geschäftliche Treiber für die Modernisierung
- **Wachstum:** Planung, in den nächsten zwei Jahren etwa zehn neue Mitarbeitende einzustellen
- **Skalierung:** Heutige IT-Infrastruktur kann diese Skalierung nicht unterstützen
- **Compliance:** Erhöhte Anforderungen an Datenschutz und Informationssicherheit
- **Strategie:** Moderne, sichere und dokumentierte IT-Infrastruktur ist strategisch notwendig

### 3.4 Projektauftrag - Ziele der neuen Infrastruktur
- Zentrale und sichere Datenverwaltung (NAS-basierter Datenspeicher)
- Hochverfügbarkeit und Ausfallsicherheit (Virtualisierung mit automatischen Backups)
- Strukturierte Netzwerksegmentierung (VLANs zur Erhöhung der Sicherheit)
- Zentrale Benutzerverwaltung (Authentifizierungs- und Autorisierungssystem)
- Cloud-Dienst für Zusammenarbeit (sichere Lösung zur Dateiablage und Synchronisation)
- Aktives Monitoring und Übersicht (Echtzeitüberwachung der Infrastruktur)
- Skalierbarkeit (Architektur für Wachstum bis auf 50–60 Mitarbeitende)

---

## 4. Funktionale Anforderungen auflisten

### 4.1 Netzwerkinfrastruktur
- [x] Aufbau einer strukturierten Client-Server-Architektur
- [x] Virtualisierungsumgebung für flexible Server-Bereitstellung
- [x] Zentrale Datenspeicherung über NAS-System
- [x] Netzwerksegmentierung für verschiedene Unternehmensbereiche
- [x] Management-Netz für Verwaltungsaufgaben
- [x] Storage-Netz für Datenspeicherung
- [x] Server-Netz für virtuelle Maschinen und Dienste
- [x] Client-Netz für Endanwender

### 4.2 Serverdienste
- [x] Cloud-Dienst für zentrale Dateiablage und Synchronisation
- [x] Backup- und Recovery-Lösungen
- [x] Zentrale Benutzerverwaltung und Authentifizierung
- [x] Monitoring und Management-Tools
- [x] Basis-Monitoring der Infrastruktur
- [x] Zentrales Authentifizierungssystem für Benutzerverwaltung

### 4.3 Client-Anbindung
- [x] Unterstützung für Standard-Clients
- [x] Zentrale Verwaltungsmöglichkeiten
- [x] Netzwerkzugriff auf zentrale Ressourcen
- [x] Zugriff auf Cloud-Dienst für Dateiablage und -synchronisation

### 4.4 Sicherheitsfunktionen
- [x] Firewall mit Zugriffskontrolle
- [x] Netzwerksegmentierung durch VLANs
- [x] Sichere Administrationszugänge (SSH, HTTPS)
- [x] Verschlüsselte Datenspeicherung für sensible Daten

### 4.5 Verwaltungsfunktionen
- [x] Zentrale Benutzerverwaltung
- [x] Berechtigungsmanagement
- [x] Monitoring und Alerting
- [x] Backup-Automatisierung

---

## 5. Nicht-funktionale Anforderungen auflisten

### 5.1 Performance-Anforderungen
- [x] Gigabit-Ethernet als Standard für Client-Anbindung
- [x] Akzeptable Latenzzeiten im lokalen Netzwerk
- [x] Schnelle Verbindungen zwischen Server-Komponenten
- [x] Gigabit-Links: min. 900 Mbps Durchsatz
- [x] Storage-Latenz: max. 10ms für Clients
- [x] VM-Boot-Zeit: max. 60 Sekunden

### 5.2 Verfügbarkeits-Anforderungen
- [x] Ausfallsicherheit durch Virtualisierung
- [x] Stabile Netzwerkverbindungen
- [x] Backup-Konzept mit definierten Recovery-Zeiten
- [x] Automatische VM-Backups auf NAS
- [x] Backup-Window: 02:00-06:00 Uhr
- [x] Retention: 7 Tage täglich, 4 Wochen wöchentlich

### 5.3 Sicherheits-Anforderungen
- [x] Firewall mit Zugriffskontrolle
- [x] Verschlüsselte Datenspeicherung für sensible Daten
- [x] Netzwerksegmentierung durch VLANs
- [x] Regelmäßige Sicherheitsupdates
- [x] Strikte VLAN-Trennung
- [x] Storage-VLAN komplett isoliert
- [x] Firewall zwischen allen Segmenten
- [x] Port-basierte Zugriffskontrolle
- [x] Firewall-Regeln nach Least-Privilege-Prinzip
- [x] Minimale Installation ohne unnötige Services
- [x] Starke Passwort-Richtlinien
- [x] SSH-Key-basierte Authentifizierung
- [x] TLS für alle Web-Services

### 5.4 Skalierbarkeits-Anforderungen
- [x] Erweiterbarkeit für zusätzliche Arbeitsplätze
- [x] Flexible Storage-Erweiterung
- [x] Modularer Aufbau der Infrastruktur
- [x] Architektur für Wachstum bis auf 50–60 Mitarbeitende
- [x] Skalierbare Architektur für Wachstum

### 5.5 Wartbarkeits-Anforderungen
- [x] Dokumentation aller Planungs- und Implementierungsschritte
- [x] Zentrale Log-Sammlung
- [x] Log-Retention: 90 Tage
- [x] Monitoring und Alerting
- [x] Administrator-Handbuch

### 5.6 Usability-Anforderungen
- [x] Web-basierte Verwaltung (Proxmox, TrueNAS, pfSense)
- [x] Intuitive Benutzeroberflächen
- [x] Zentrale Verwaltungsmöglichkeiten

---

## 6. Abnahmekriterien verstehen

### 6.1 Theoretische Planung - Abnahmekriterien
- [x] Vollständiges Lastenheft vorhanden
- [x] Vollständiges Pflichtenheft vorhanden
- [x] Vollständige Netzwerkdokumentation mit Topologie-Diagrammen
- [x] Adressierungskonzept (IP-Plan) für alle Netzwerkbereiche
- [x] Hardware- und Software-Spezifikationen dokumentiert
- [x] Sicherheitskonzept dokumentiert
- [x] Kostenschätzung vorhanden
- [x] VLAN-Design mit mindestens 3 Segmenten
- [x] Backup-Strategie dokumentiert

### 6.2 Praktische Umsetzung - Abnahmekriterien
- [x] Funktionierende Hypervisor-Umgebung mit mindestens zwei VMs
- [x] Konfigurierter Router mit Firewall
- [x] NAS-System mit eingerichteten Dateifreigaben
- [x] Netzwerkverbindung zwischen allen Komponenten
- [x] Dokumentation der Konfiguration
- [x] Cloud-Dienst für zentrale Dateiablage funktionsfähig
- [x] Zentrale Benutzerverwaltung implementiert
- [x] Monitoring funktionsfähig
- [x] Funktionstests erfolgreich

### 6.3 Dokumentation - Abnahmekriterien
- [x] Netzwerk-Topologie-Diagramm (physisch und logisch)
- [x] VLAN-Konfiguration
- [x] IP-Adressplan
- [x] Hypervisor-Konfiguration
- [x] NAS-Konfiguration und Share-Berechtigungen
- [x] VM-Inventar mit Ressourcen und Zweck
- [x] Firewall-Regelwerk
- [x] Backup- und Recovery-Verfahren
- [x] Administrator-Handbuch

### 6.4 Präsentation - Abnahmekriterien
- [x] PowerPoint-Präsentation (15-20 Minuten)
- [x] Projektvorstellung und Zielsetzung (3 Min.)
- [x] Theoretische Netzwerkplanung (5 Min.)
- [x] Praktische Implementierung - Demo (7 Min.)
- [x] Herausforderungen und Lessons Learned (3 Min.)
- [x] Ausblick und Erweiterungen (2 Min.)
- [x] Demo-Inhalte vorbereitet (Proxmox, NAS, VMs, Firewall, Monitoring)

---

## 7. Offene Fragen identifizieren und klären

### 7.1 Hardware-bezogene Fragen
- [x] **Frage:** Welche konkrete Hardware steht zur Verfügung?
  - **Antwort:** Hardware wird gestellt, genaue Spezifikationen werden bei Projektstart bekannt gegeben

- [x] **Frage:** Gibt es einen Managed Switch mit VLAN-Unterstützung?
  - **Antwort:** Optional nach Verfügbarkeit, kann auch über Router-VLANs gelöst werden

- [x] **Frage:** Wie viele Netzwerk-Interfaces hat der Hypervisor-Server?
  - **Antwort:** Mindestens 2 Interfaces empfohlen (Management + Storage), genaue Anzahl bei Hardware-Bereitstellung

### 7.2 Software-bezogene Fragen
- [x] **Frage:** Welche Linux-Distribution für VMs?
  - **Antwort:** Ubuntu Server oder Debian empfohlen (kompatibel mit Proxmox, gute Dokumentation)

- [x] **Frage:** Nextcloud oder ownCloud?
  - **Antwort:** Nextcloud empfohlen (aktiver entwickelt, bessere Community)

- [x] **Frage:** Zabbix oder Prometheus/Grafana?
  - **Antwort:** Beide möglich, Prometheus/Grafana moderner, Zabbix einfacher für Einsteiger

### 7.3 Netzwerk-bezogene Fragen
- [x] **Frage:** Wie viele VLANs sind genau erforderlich?
  - **Antwort:** Mindestens 3 (Management, Server, Storage), zusätzlich Client-VLAN = 4 VLANs

- [x] **Frage:** Soll Internet-Zugang simuliert werden?
  - **Antwort:** Ja, über NAT auf Router/Firewall, echter Internet-Zugang nicht erforderlich

- [x] **Frage:** DHCP auf Router oder separater VM?
  - **Antwort:** Kann auf Router oder pfSense-VM laufen, pfSense-VM empfohlen für zentrale Verwaltung

### 7.4 Projekt-bezogene Fragen
- [x] **Frage:** Muss ein Grundriss des Unternehmens erstellt werden?
  - **Antwort:** Nein, nicht im Lasten-/Pflichtenheft vorgesehen, nur logische/physische Netzwerk-Topologie

- [x] **Frage:** Wie detailliert muss die Kostenschätzung sein?
  - **Antwort:** Für theoretische Planung vollständig, für praktische Umsetzung nur verwendete Hardware

- [x] **Frage:** Gibt es Vorgaben für die Dokumentationssprache?
  - **Antwort:** Dokumentation in Deutsch, Code-Kommentare in Englisch

### 7.5 Zeitplan-bezogene Fragen
- [x] **Frage:** Können Phasen parallel bearbeitet werden?
  - **Antwort:** Theoretische Planung sollte vor praktischer Umsetzung abgeschlossen sein, innerhalb der Phasen teilweise parallel möglich

- [x] **Frage:** Wie flexibel ist der Zeitplan?
  - **Antwort:** 100 Stunden Gesamtzeit, Pufferzeiten in Phasen eingeplant, Scope reduzierbar bei Zeitproblemen

### 7.6 Abnahme-bezogene Fragen
- [x] **Frage:** Wer nimmt das Projekt ab?
  - **Antwort:** Prüfungsausschuss der Schule, Projektbetreuer

- [x] **Frage:** Muss die praktische Umgebung dauerhaft laufen?
  - **Antwort:** Nein, nur für Demonstration und Tests, danach kann abgeschaltet werden

---

## Zusammenfassung Phase 1.1

### Erledigte Aufgaben
✅ Lastenheft vollständig durchgearbeitet  
✅ Pflichtenheft analysiert  
✅ Ausgangssituation dokumentiert  
✅ Funktionale Anforderungen aufgelistet  
✅ Nicht-funktionale Anforderungen aufgelistet  
✅ Abnahmekriterien verstanden  
✅ Offene Fragen identifiziert und geklärt  

### Wichtigste Erkenntnisse
1. **Projektumfang:** 100 Stunden für Planung und Implementierung einer Client-Server-Netzwerkinfrastruktur
2. **Kernkomponenten:** Hypervisor (Proxmox VE), NAS (TrueNAS), Firewall (pfSense/OPNsense)
3. **Netzwerkarchitektur:** 4 VLANs (Management, Server, Storage, Clients)
4. **Mindestanforderungen:** 2 VMs, funktionierendes Netzwerk, Dokumentation
5. **Fokus:** Theoretische Planung + praktische Proof-of-Concept-Umsetzung

### Nächste Schritte (Phase 1.2)
- Hypervisor-Recherche (Proxmox VE vs. VMware ESXi)
- Detaillierte Vergleichsanalyse
- Entscheidungsdokumentation

---

**Dokument erstellt am:** 2025-01-02  
**Status:** Phase 1.1 abgeschlossen  
**Nächste Phase:** 1.2 Hypervisor-Recherche

