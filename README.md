# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.3-00cae3.svg)
![Status](https://img.shields.io/badge/Status-Operational-00ff00.svg)

---

## 🇩🇪 Deutsch: Übersicht
Ein hochmodernes Kontrollzentrum für Termine und Fristen. Optimiert für Desktop-Management und passive Dashboards, mit direkter GitHub-Cloud-Synchronisation.

### 🚀 Kernfunktionen
* **Echtzeit-Sync:** Speichert Daten direkt in deinem GitHub-Repo via REST API.
* **Backup & Restore:** Lokale JSON-Snapshots erstellen und mit einem Klick wiederherstellen.
* **Duale Ansicht:** Wechsel zwischen Monitor-Liste und grafischem Kalender.
* **Smart Filtering:** "LIVE NOW" Erkennung, Archiv-Funktion und der **# NOTAG** Filter.
* **Rich Text:** Unterstützt Checkboxen, Fettdruck und Farbcodes.
* **ICS-Import:** Direkter Import aus externen Kalender-Dateien (.ics).

---

## 🇺🇸 English: Overview
A state-of-the-art control center for deadlines and appointments. Optimized for desktop management and passive dashboards, featuring direct GitHub cloud synchronization.

### 🚀 Key Features
* **Real-Time Sync:** Persists data directly to your GitHub repository via REST API.
* **Backup & Restore:** Create local JSON snapshots and restore them with a single click.
* **Dual Interface:** Toggle between a tactical Monitor List and a graphical Calendar.
* **Smart Filtering:** "LIVE NOW" detection, archiving, and the **# NOTAG** filter.
* **Rich Text:** Native support for checkboxes, bold text, and color codes.
* **ICS Import:** Direct import functionality from external calendar files (.ics).

---

## 📜 Versions-Historie / Version History

### **v1.0 - The Core (Basis)**
* **DE:** Grundlegendes Listing, lokale Speicherung, einfaches Design.
* **EN:** Basic listing, local storage, simple design.

### **v2.0 - Orbital Sync**
* **DE:** Einführung der GitHub API Anbindung für Cloud-Sync. PIN-Login-System integriert.
* **EN:** Introduction of GitHub API for cloud sync. Integrated PIN login system.

### **v3.0 - Tactical UI**
* **DE:** Neues "Orbital" Dark-Design, Countdown-Timer, Tag-System und ICS-Import.
* **EN:** New "Orbital" dark design, countdown timers, tag system, and ICS import.

### **v3.1 - Calendar & Rich Text**
* **DE:** Implementierung der Kalender-Ansicht und Textformatierung (Bett, Farbe, Checkboxen).
* **EN:** Implementation of Calendar View and text formatting (bold, color, checkboxes).

### **v3.2 - Redundancy Update**
* **DE:** Backup- und Restore-Logik für JSON-Dateien hinzugefügt.
* **EN:** Added backup and restore logic for JSON files.

### **v3.3 - System Layout (Current)**
* **DE:** Optimierung der Toolbar. System-Buttons (Backup/Restore) sind nun rechtsbündig isoliert.
* **EN:** Toolbar optimization. System buttons (Backup/Restore) are now isolated on the right side.

---

## ⚙️ Einrichtung / Setup (DE/EN)

1. **GitHub:** Create a private repo with a `termine.json` containing `[]`.
2. **Token:** Generate a GitHub PAT (classic) and split it into `t1` and `t2` in the code.
3. **PIN:** Standard PIN is `0508`. Change the Base64 string in `P_ENC` for security.
4. **URL:** Update `G_URL` to point to your repository.

---
*Orbital Control Systems - Developed for Precision.*
