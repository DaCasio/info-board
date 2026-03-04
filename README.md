# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.1-00cae3.svg)
![License](https://img.shields.io/badge/License-Private-ff4d4d.svg)

Ein hochmoderner, browserbasierter Termin-Planer mit orbitalem Design und direkter Cloud-Synchronisation via GitHub API. Optimiert für Desktop-Management und passive E-Ink-Displays.

---

## 🚀 Kernfunktionen / Core Features

### 🇩🇪 Deutsch
* **Echtzeit-Synchronisation:** Speichert Daten direkt in deinem GitHub-Repo via REST API.
* **Duale Ansicht:** Wechsel zwischen **Monitor-Liste** und **Kalender-Ansicht**.
* **Smart Filtering:** "LIVE NOW" Erkennung, Archiv-Funktion und der **# NOTAG** Filter.
* **Backup-System:** Exportiere deine Daten jederzeit als JSON-Datei mit Zeitstempel.
* **Markdown & Checkboxen:** Unterstützt Fett-Text, Farben und interaktive Aufgabenlisten.
* **ICS-Import:** Direkter Import aus Kalender-Dateien.

### 🇺🇸 English
* **Real-Time Sync:** Persists data directly to your GitHub repository via REST API.
* **Dual Interface:** Toggle between tactical **Monitor List** and **Calendar View**.
* **Smart Filtering:** "LIVE NOW" detection, archiving, and the **# NOTAG** filter.
* **Backup System:** Export your data at any time as a timestamped JSON file.
* **Markdown & Checkboxes:** Native support for bold text, colors, and interactive to-dos.
* **ICS Import:** Quick import functionality from external calendar files.

---

## 🛠️ Einrichtung / Setup Instructions

1. **GitHub:** Erstelle ein privates Repo und eine `termine.json` mit `[]`.
2. **Token:** Generiere ein GitHub PAT (classic) mit `repo` Scope. Teile es auf `t1` und `t2` auf.
3. **URL:** Passe die `G_URL` im Script an dein Repository an.
4. **PIN:** Standard-PIN ist `0508`. Ändere den Base64-String in `P_ENC` für Sicherheit.

---

## 📖 Bedienung / How to Use

| Aktion / Action | Beschreibung (DE) | Description (EN) |
| :--- | :--- | :--- |
| **💾 BACKUP** | Lädt alle Termine als lokale JSON-Datei herunter. | Downloads all events as a local JSON file. |
| **# NOTAG** | Filtert alle Termine ohne Kategorien heraus. | Filters all events that have no tags assigned. |
| **ICS IMPORT** | Lädt Termindaten aus einer `.ics` Datei vor. | Pre-fills data from an `.ics` calendar file. |
| **CALENDAR** | Visualisiert Termine im Monatsraster. | Visualizes events in a monthly grid. |

---

## 🔒 Sicherheit / Security
**DE:** Die HTML-Datei enthält sensible Token-Daten. Hoste sie nur in privaten Umgebungen oder lokal.  
**EN:** This file contains sensitive API tokens. Host privately or run locally.

---
*Developed for Orbital Control Systems. Status: Operational.*
