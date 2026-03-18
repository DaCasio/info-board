# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.4-00cae3.svg)
![Status](https://img.shields.io/badge/Status-Operational-00ff00.svg)

---

## 🇩🇪 Deutsch: Übersicht
Ein hochmodernes Kontrollzentrum für Termine und Fristen. Optimiert für Desktop-Management und passive E-Ink-Dashboards, mit direkter GitHub-Cloud-Synchronisation.

### 🚀 Kernfunktionen
* **Echtzeit-Sync:** Speichert Daten direkt in deinem GitHub-Repo via REST API.
* **Backup & Restore:** Lokale JSON-Snapshots erstellen und mit einem Klick wiederherstellen.
* **Duale Ansicht:** Wechsel zwischen Monitor-Liste und grafischem Kalender.
* **Intelligente Sortierung:** Priorisiert Startzeiten (vor Verstreichen) → Endzeiten (danach).
* **Smart Filtering:** "LIVE NOW" Erkennung, Archiv-Funktion und Tag-Filter.
* **Rich Text:** Unterstützt **Fettdruck**, *Kursiv*, farbige Notizen und strukturierte Checkliste.
* **Display-Optimierung:** Separat `display.html` für E-Ink/Passive-Bildschirme.
* **Wiederholungslogik:** Täglich, wöchentlich (feste Tage), monatlich, halbjährlich, jährlich.

---

## 🇺🇸 English: Overview
A state-of-the-art control center for deadlines and appointments. Optimized for desktop management and passive E-Ink dashboards, featuring direct GitHub cloud synchronization.

### 🚀 Key Features
* **Real-Time Sync:** Persists data directly to your GitHub repository via REST API.
* **Backup & Restore:** Create local JSON snapshots and restore with one click.
* **Dual Interface:** Toggle between tactical Monitor List and graphical Calendar.
* **Intelligent Sorting:** Start time priority (pre-start) → End time (post-start).
* **Smart Filtering:** "LIVE NOW" detection, archiving, and dynamic tag filters.
* **Rich Text:** Native **bold**, *italic*, colored notes, and structured checklists.
* **Display Optimization:** Dedicated `display.html` for E-Ink/passive screens.
* **Recurrence Logic:** Daily, weekly (fixed days), monthly, half-yearly, yearly.

---

## 📜 Versions-Historie / Version History

### **v1.0 - The Core (Basis)**
* **DE:** Grundlegendes Listing, lokale Speicherung, einfaches Design.
* **EN:** Basic listing, local storage, simple design.

### **v2.0 - Orbital Sync**
* **DE:** Einführung der GitHub API Anbindung für Cloud-Sync. PIN-Login-System integriert.
* **EN:** Introduction of GitHub API for cloud sync. Integrated PIN login system.

### **v3.0 - Tactical UI**
* **DE:** Neues "Orbital" Dark-Design, Countdown-Timer, Tag-System.
* **EN:** New "Orbital" dark design, countdown timers, tag system.

### **v3.1 - Calendar & Rich Text**
* **DE:** Kalender-Ansicht und erweiterte Textformatierung (Fett, Farbe, Checkboxen).
* **EN:** Calendar View and enhanced text formatting (bold, color, checkboxes).

### **v3.2 - Redundancy Update**
* **DE:** Backup- und Restore-Logik für JSON-Dateien hinzugefügt.
* **EN:** Added backup and restore logic for JSON files.

### **v3.3 - System Layout**
* **DE:** Toolbar-Optimierung. Backup/Restore-Buttons rechtsbündig isoliert.
* **EN:** Toolbar optimization. Backup/Restore buttons isolated right-aligned.

### **v3.4 - Smart Sorting (Current)**
* **DE:** **Intelligente Sortierung:** Termine mit Startzeit werden vor Start nach START, danach nach ENDE sortiert. Sowohl `index.html` als auch `display.html` betroffen.
* **EN:** **Intelligent Sorting:** Appointments with start times sort by START (pre-start) then END (post-start). Applied to both `index.html` and `display.html`.

---
├── index.html # Haupt-Editor + Kalender (Login erforderlich)
├── display.html # Passive Anzeige (E-Ink/Dashboards, read-only)
├── termine.json # Datenbank (JSON-Array)
└── README.md # Diese Datei

---

## ⚙️ Einrichtung / Setup (DE/EN)

1. **GitHub:** Erstelle ein privates Repo mit `termine.json` (Inhalt: `[]`).
2. **Token:** Erzeuge GitHub PAT (classic) → Aufteilen in `t1`/`t2` im Code.
3. **PIN:** Standard-PIN `0508`. Für Sicherheit `P_ENC` Base64-String ändern.
4. **URLs:** `G_URL` auf dein Repository anpassen (`dacasio` → **dein Username**).

### Für E-Ink/Passive-Displays:
- `display.html` direkt öffnen → Kein Login erforderlich
- Automatische Updates alle 60 Sekunden

---
*Orbital Control Systems v3.4 - Precision Scheduling for Mission Critical Operations.*

Hauptänderungen:

    Version 3.4 mit Smart Sorting hervorgehoben

    Intelligente Sortierlogik als neue Kernfunktion

    display.html als E-Ink/Passive-Display explizit erwähnt

    Dateistruktur für Klarheit hinzugefügt

    Wiederholungslogik präzisiert

    aktueller Status (3.4) klar markiert



## 📁 Dateistruktur / File Structure
