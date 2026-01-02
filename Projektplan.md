# Projektplan: Client-Server-Netzwerkinfrastruktur
## ITA Abschlussprojekt - Planova Ingenieurplanung GmbH

**Projektdauer:** 100 Stunden  
**Abgabeschluss:** 15.12.2025  
**Lernfeld:** 5 - Rechnernetze nach Vorgaben einrichten

---

## Übersicht

Planung und Implementierung einer Client-Server-Netzwerkinfrastruktur für ein mittelständisches Unternehmen (40 Mitarbeitende, 4 Fachabteilungen).

**Ziel:** Theoretische Gesamtplanung + praktische Proof-of-Concept-Umsetzung

---

## Projektphasen

### Phase 1: Planung und Recherche (ca. 20 Std.)

#### Aufgaben:
- [ ] Anforderungen aus Lastenheft analysieren
- [ ] Technische Recherche zu Hypervisor-Lösungen (Proxmox VE, VMware ESXi)
- [ ] NAS-Systeme vergleichen (TrueNAS, OpenMediaVault)
- [ ] Firewall-Lösungen recherchieren (pfSense, OPNsense)
- [ ] Netzwerkarchitektur-Konzepte studieren (VLAN, Routing, Security)
- [ ] Hardware-Anforderungen definieren
- [ ] Software-Lizenzen prüfen (Open Source vs. kommerziell)

#### Deliverables:
- Recherche-Dokumentation
- Technologie-Vergleich
- Hardware-Spezifikationen

---

### Phase 2: Theoretische Durchführung (ca. 35 Std.)

#### 2.1 Netzwerkarchitektur-Planung (10 Std.)
- [ ] Netzwerk-Topologie-Diagramm erstellen (logisch)
- [ ] Physisches Netzwerkdiagramm erstellen
- [ ] VLAN-Design planen:
  - VLAN 1: Management (192.168.1.0/24)
  - VLAN 10: Server (192.168.10.0/24)
  - VLAN 20: Storage (192.168.20.0/24)
  - VLAN 100: Clients (10.0.100.0/24)
- [ ] IP-Adressplan erstellen (alle Geräte dokumentieren)
- [ ] Routing-Konzept entwickeln

#### 2.2 Sicherheitskonzept (8 Std.)
- [ ] Firewall-Regelwerk definieren
- [ ] Zugriffskontroll-Strategie entwickeln
- [ ] Verschlüsselungskonzept (TLS, SSH, Datenverschlüsselung)
- [ ] Netzwerksegmentierung begründen
- [ ] Sicherheitsrichtlinien dokumentieren

#### 2.3 Server-Infrastruktur-Planung (10 Std.)
- [ ] Hypervisor-Konfiguration planen
- [ ] VM-Design erstellen:
  - VM 1: Cloud-Dienst (Nextcloud/ownCloud)
  - VM 2: Benutzerverwaltung (LDAP/FreeIPA)
  - VM 3: Monitoring (Zabbix/Prometheus)
  - VM 4: Firewall (pfSense/OPNsense)
- [ ] Ressourcen-Zuteilung (CPU, RAM, Disk) pro VM
- [ ] Storage-Konzept (NAS-Integration, Datastores)

#### 2.4 Backup-Strategie (4 Std.)
- [ ] Backup-Konzept entwickeln
- [ ] Recovery-Zeiten definieren
- [ ] Retention-Policy festlegen
- [ ] Backup-Automatisierung planen

#### 2.5 Dokumentation (3 Std.)
- [ ] Pflichtenheft vervollständigen
- [ ] Technische Spezifikationen dokumentieren
- [ ] Kostenschätzung erstellen

#### Deliverables:
- Vollständiges Pflichtenheft
- Netzwerk-Topologie-Diagramme (logisch + physisch)
- IP-Adressplan
- VLAN-Konfiguration
- Sicherheitskonzept
- Hardware-/Software-Spezifikationen
- Backup-Strategie
- Kostenschätzung

---

### Phase 3: Praktische Durchführung (ca. 30 Std.)

#### 3.1 Vorbereitung (5 Std.)
- [ ] Hardware bereitstellen
- [ ] Workspace einrichten
- [ ] Software herunterladen (ISOs, Images):
  - Proxmox VE ISO
  - TrueNAS ISO
  - pfSense/OPNsense ISO
  - Linux-Distributionen für VMs
- [ ] Netzwerkkabel vorbereiten

#### 3.2 Basis-Installation (8 Std.)
- [ ] Hypervisor-Server aufbauen
  - [ ] Proxmox VE installieren
  - [ ] Netzwerk-Interfaces konfigurieren
  - [ ] Updates durchführen
- [ ] Router konfigurieren
  - [ ] Basis-Konfiguration
  - [ ] VLANs einrichten
- [ ] NAS aufbauen
  - [ ] TrueNAS installieren
  - [ ] RAID konfigurieren
  - [ ] Netzwerk-Interfaces konfigurieren
- [ ] Verkabelung herstellen
  - [ ] Alle Komponenten verbinden
  - [ ] Netzwerk-Verbindungen testen

#### 3.3 Netzwerk-Konfiguration (6 Std.)
- [ ] VLANs auf Router konfigurieren
- [ ] VLANs auf Switch konfigurieren (falls vorhanden)
- [ ] IP-Adressen vergeben
- [ ] Routing konfigurieren
- [ ] Netzwerk-Tests durchführen:
  - [ ] Ping-Tests zwischen VLANs
  - [ ] Latenz-Messungen
  - [ ] Bandbreiten-Tests (iperf3)

#### 3.4 Storage-Setup (4 Std.)
- [ ] RAID auf NAS konfigurieren
- [ ] Storage-Pools erstellen:
  - Pool 1: Produktivdaten
  - Pool 2: Backups
  - Pool 3: ISO-Images
- [ ] NFS aktivieren und testen
- [ ] SMB/CIFS aktivieren und testen
- [ ] NFS-Datastore in Proxmox einbinden
- [ ] Shares erstellen und Berechtigungen setzen

#### 3.5 VM-Deployment (6 Std.)
- [ ] VM-Templates vorbereiten (falls möglich)
- [ ] VM 1: Cloud-Dienst erstellen
  - [ ] VM anlegen (z.B. 2 CPU, 4 GB RAM, 50 GB Disk)
  - [ ] Linux installieren (Ubuntu/Debian)
  - [ ] Nextcloud installieren und konfigurieren
  - [ ] Netzwerk-Anbindung testen
- [ ] VM 2: Benutzerverwaltung erstellen
  - [ ] VM anlegen (z.B. 2 CPU, 2 GB RAM, 30 GB Disk)
  - [ ] Linux installieren
  - [ ] LDAP/FreeIPA installieren und konfigurieren
- [ ] VM 3: Monitoring erstellen
  - [ ] VM anlegen (z.B. 2 CPU, 2 GB RAM, 30 GB Disk)
  - [ ] Linux installieren
  - [ ] Zabbix oder Prometheus/Grafana installieren
- [ ] VM 4: Firewall (pfSense/OPNsense) erstellen
  - [ ] VM anlegen (z.B. 2 CPU, 2 GB RAM, 20 GB Disk)
  - [ ] pfSense/OPNsense installieren
  - [ ] Firewall-Regeln konfigurieren
  - [ ] Inter-VLAN-Routing einrichten

#### 3.6 Service-Konfiguration (8 Std.)
- [ ] Cloud-Dienst konfigurieren:
  - [ ] Benutzer anlegen
  - [ ] Freigaben einrichten
  - [ ] Web-Zugriff testen
- [ ] Firewall-VM konfigurieren:
  - [ ] Firewall-Regeln implementieren
  - [ ] NAT konfigurieren
  - [ ] Zugriffskontrolle testen
- [ ] Monitoring-System aufsetzen:
  - [ ] Monitoring-Agenten installieren
  - [ ] Dashboards konfigurieren
  - [ ] Alerts einrichten
- [ ] Zentrale Benutzerverwaltung konfigurieren:
  - [ ] Benutzer anlegen
  - [ ] Gruppen erstellen
  - [ ] Berechtigungen testen

#### 3.7 Testing und Dokumentation (8 Std.)
- [ ] Funktionstests durchführen:
  - [ ] VLAN-Isolation testen
  - [ ] VM-Erstellung und -Start testen
  - [ ] Storage-Zugriff testen
  - [ ] Backup und Recovery testen
  - [ ] Cloud-Dienst-Zugriff testen
- [ ] Performance-Tests:
  - [ ] Netzwerk-Durchsatz messen (iperf3)
  - [ ] Storage-Performance testen (fio)
  - [ ] VM-Boot-Zeit messen
- [ ] Sicherheits-Tests:
  - [ ] Port-Scans (nmap)
  - [ ] Firewall-Regeln testen
  - [ ] VLAN-Isolation verifizieren
- [ ] Konfigurationsdokumentation:
  - [ ] Alle Konfigurationen dokumentieren
  - [ ] Screenshots erstellen
  - [ ] Zugangsdaten dokumentieren (sicher aufbewahren)

#### Deliverables:
- Funktionierende Hypervisor-Umgebung
- Mindestens 2 VMs laufen stabil
- Konfigurierter Router mit Firewall
- NAS mit eingerichteten Shares
- Netzwerkverbindung zwischen allen Komponenten
- Konfigurationsdokumentation
- Test-Protokolle

---

### Phase 4: Präsentationserstellung (ca. 5 Std.)

#### Aufgaben:
- [ ] PowerPoint-Präsentation erstellen (15-20 Minuten)
- [ ] Struktur der Präsentation:
  1. Projektvorstellung und Zielsetzung (3 Min.)
  2. Theoretische Netzwerkplanung (5 Min.)
  3. Praktische Implementierung - Demo (7 Min.)
  4. Herausforderungen und Lessons Learned (3 Min.)
  5. Ausblick und Erweiterungen (2 Min.)
- [ ] Demo-Vorbereitung:
  - [ ] Proxmox Web-GUI zeigen
  - [ ] NAS-Shares zeigen
  - [ ] VM starten/stoppen demonstrieren
  - [ ] Firewall-Konfiguration zeigen
  - [ ] Monitoring-Dashboard zeigen
- [ ] Präsentationsmittel vorbereiten:
  - [ ] PowerPoint-Datei
  - [ ] Beamer testen
  - [ ] Backup-Plan (USB-Stick)

#### Deliverables:
- PowerPoint-Präsentation
- Demo-Script
- Backup-Präsentationsmittel

---

### Phase 5: Auswertung und Ausblick (ca. 10 Std.)

#### Aufgaben:
- [ ] Projektauswertung:
  - [ ] Was hat gut funktioniert?
  - [ ] Was waren die größten Herausforderungen?
  - [ ] Was würde ich anders machen?
- [ ] Dokumentation finalisieren:
  - [ ] Alle Dokumente durchgehen
  - [ ] Vollständigkeit prüfen
  - [ ] Formatierung überarbeiten
- [ ] Erweiterungsmöglichkeiten dokumentieren:
  - [ ] WLAN-Integration
  - [ ] VPN-Lösung
  - [ ] High-Availability
  - [ ] Container-Plattform
- [ ] Lessons Learned dokumentieren
- [ ] Finale Abgabe vorbereiten:
  - [ ] Alle Dateien sammeln
  - [ ] Checkliste durchgehen
  - [ ] Backup erstellen

#### Deliverables:
- Finale Projekt-Dokumentation
- Auswertung und Lessons Learned
- Ausblick auf Erweiterungen

---

## Abnahmekriterien

### Theoretische Planung:
- ✅ Vollständiges Lastenheft
- ✅ Vollständiges Pflichtenheft
- ✅ Netzwerk-Topologie-Diagramme (logisch + physisch)
- ✅ IP-Adressplan
- ✅ VLAN-Design (mindestens 3 Segmente)
- ✅ Sicherheitskonzept mit Firewall-Regeln
- ✅ Hardware-/Software-Spezifikationen
- ✅ Backup-Strategie
- ✅ Kostenschätzung

### Praktische Umsetzung:
- ✅ Hypervisor installiert und konfiguriert
- ✅ Router mit Firewall konfiguriert
- ✅ NAS mit RAID und Shares eingerichtet
- ✅ Mindestens 2 VMs laufen stabil
- ✅ Netzwerkverbindung zwischen allen Komponenten
- ✅ Cloud-Dienst funktionsfähig
- ✅ Zentrale Benutzerverwaltung implementiert
- ✅ Monitoring funktionsfähig
- ✅ Dokumentation der Konfiguration
- ✅ Funktionstests erfolgreich

---

## Risiken und Gegenmaßnahmen

| Risiko | Wahrscheinlichkeit | Auswirkung | Gegenmaßnahme |
|--------|-------------------|------------|---------------|
| Hardware-Ausfall | Mittel | Hoch | Backup-Konzept, Ersatz-Hardware verfügbar halten |
| Kompatibilitätsprobleme | Mittel | Mittel | Hardware Compatibility Lists prüfen, Vorab-Tests |
| Zeitüberschreitung | Hoch | Mittel | Pufferzeiten einplanen, Scope auf Minimum reduzierbar |
| Fehlende Kenntnisse | Mittel | Mittel | Vorab-Recherche, Online-Tutorials, Dokumentation nutzen |
| Performance-Engpässe | Niedrig | Niedrig | Performance-Tests, Skalierungsreserven einplanen |

---

## Meilensteine

- **Meilenstein 1:** Theoretische Planung abgeschlossen (ca. 55 Std.)
- **Meilenstein 2:** Praktische Umsetzung abgeschlossen (ca. 85 Std.)
- **Meilenstein 3:** Präsentation fertig (ca. 90 Std.)
- **Meilenstein 4:** Finale Abgabe (100 Std.)

---

## Notizen und Anmerkungen

- Hardware wird gestellt (keine Beschaffung nötig)
- Fokus auf Open Source Lösungen (keine Lizenzkosten)
- Proof-of-Concept-Umgebung (nicht produktiv)
- Dokumentation ist kritisch für die Bewertung
- Präsentation sollte technische Details zeigen, aber verständlich bleiben

---

**Erstellt am:** $(date +%Y-%m-%d)  
**Status:** In Bearbeitung

