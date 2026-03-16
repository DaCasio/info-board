# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.5-00cae3.svg)
![Status](https://img.shields.io/badge/Status-Operational-00ff00.svg)
![Platform](https://img.shields.io/badge/Platform-Web--Dashboard-blue.svg)

---

## 🇩🇪 Deutsch: Übersicht
Ein hochmodernes Kontrollzentrum für Termine und Fristen, optimiert für Desktop-Management und passive Dashboards (wie E-Ink Displays). Das System nutzt eine direkte GitHub-Cloud-Synchronisation als Backend.

### 🚀 Kernfunktionen
* **Echtzeit-Sync:** Volle Integration der GitHub REST API zur Datenspeicherung in deinem Repository.
* **Duale Ansicht:** Nahtloser Wechsel zwischen einer taktischen Monitor-Liste und einem grafischen Kalender.
* **Smart Filtering:** Intelligente "LIVE NOW" Erkennung, Archiv-Funktion und dedizierter **# NOTAG** Filter.
* **Rich Text & Checklisten:** Unterstützung für Fettdruck, Farbcodes und ein integriertes Checklisten-System für Aufgaben innerhalb von Terminen.
* **E-Ink Optimierung:** Spezielle `display.html` für passive Anzeige-Panels ohne interaktive Elemente (View-Only).
* **Backup & Restore:** Integrierte Logik zum Erstellen lokaler Snapshots und zur schnellen Wiederherstellung.

---

## 🇺🇸 English: Overview
A state-of-the-art control center for deadlines and appointments. Optimized for desktop management and passive dashboards, featuring direct GitHub cloud synchronization.

### 🚀 Key Features
* **Real-Time Sync:** Persists data directly to your GitHub repository via REST API.
* **Dual Interface:** Toggle between a tactical Monitor List and a graphical Calendar.
* **Rich Text & Checklists:** Support for bold text, color codes, and a built-in checklist system for sub-tasks.
* **Passive Display Mode:** Dedicated `display.html` optimized for E-Ink dashboards (view-only mode).
* **Data Redundancy:** Local JSON backup and restore logic included.

---

## 🛠️ Technische Struktur / Architecture

| Datei | Beschreibung |
| :--- | :--- |
| `index.html` | Das Haupt-Kontrollzentrum (Admin-Interface) zum Erstellen und Editieren. |
| `display.html` | Optimierte Anzeige für E-Ink Displays (automatischer Refresh, keine Interaktion). |
| `termine.json` | Die zentrale Datenbank im GitHub-Repository. |

---

## 📜 Versionshistorie / Changelog

### **v3.5 - Checklist Update (Current)**
* **DE:** Einführung des Checklisten-Systems. Aufgaben können nun innerhalb von Terminen erstellt und abgehakt werden.
* **EN:** Introduction of the checklist system. Tasks can now be created and managed within events.

### **v3.4 - E-Ink Integration**
* **DE:** Entwicklung der `display.html`. Reine Anzeige-Ansicht für passive Displays mit optimiertem Kontrast.
* **EN:** Development of `display.html`. View-only mode for passive displays with optimized contrast.

### **v3.3 - System Layout**
* **DE:** Optimierung der Toolbar und Trennung der System-Buttons (Backup/Restore).
* **EN:** Toolbar optimization and isolation of system buttons.

### **v3.2 - Redundancy Update**
* **DE:** Implementierung der Backup- und Restore-Logik für JSON-Snapshots.
* **EN:** Added backup and restore logic for JSON files.

---

## ⚙️ Einrichtung / Setup

1.  **GitHub Repo:** Erstelle ein privates Repository mit einer `termine.json`, die initial `[]` enthält.
2.  **Access Token:** Generiere einen GitHub PAT (classic) mit `repo` Berechtigungen.
3.  **Konfiguration:** Hinterlege den Token (gesplittet in `t1` und `t2` zur Sicherheit) und die Repository-URL in den HTML-Dateien.
