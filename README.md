# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.2-00cae3.svg)
![License](https://img.shields.io/badge/License-Private-ff4d4d.svg)

Ein hochmoderner, browserbasierter Termin-Planer mit orbitalem Design und direkter Cloud-Synchronisation via GitHub API. Optimiert für Desktop-Management und passive E-Ink-Displays.

---

## 🚀 Kernfunktionen / Core Features

### 🇩🇪 Deutsch
* **Echtzeit-Synchronisation:** Speichert Daten direkt in deinem GitHub-Repo via REST API.
* **Backup & Restore:** Exportiere deine Daten als JSON-Datei und stelle sie bei Bedarf mit einem Klick wieder her.
* **Duale Ansicht:** Wechsel zwischen **Monitor-Liste** und **Kalender-Ansicht**.
* **Smart Filtering:** "LIVE NOW" Erkennung, Archiv-Funktion und der **# NOTAG** Filter.
* **Markdown & Checkboxen:** Unterstützt Fett-Text, Farben und interaktive Aufgabenlisten.
* **ICS-Import:** Direkter Import aus Kalender-Dateien.

### 🇺🇸 English
* **Real-Time Sync:** Persists data directly to your GitHub repository via REST API.
* **Backup & Restore:** Export your data as a JSON file and restore it with a single click if needed.
* **Dual Interface:** Toggle between tactical **Monitor List** and **Calendar View**.
* **Smart Filtering:** "LIVE NOW" detection, archiving, and the **# NOTAG** filter.
* **Markdown & Checkboxes:** Native support for bold text, colors, and interactive to-dos.
* **ICS Import:** Quick import functionality from external calendar files.

---

## 🛠️ Einrichtung / Setup Instructions

1. **GitHub:** Erstelle ein privates Repo und eine `termine.json` mit `[]`.
2. **Token:** Generiere ein GitHub PAT (classic) mit `repo` Scope. Teile es auf `t1` und `t2` im Code auf.
3. **URL:** Passe die `G_URL` im Script an dein Repository an.
4. **PIN:** Standard-PIN ist `0508`. Ändere den Base64-String in `P_ENC` für zusätzliche Sicherheit.

---

## 📖 Bedienung / How to Use

| Aktion / Action | Beschreibung (DE) | Description (EN) |
| :--- | :--- | :--- |
| **💾 BACKUP** | Lädt alle Termine als lokale JSON-Datei herunter. | Downloads all events as a local JSON file. |
| **📂 RESTORE** | Lädt eine JSON-Datei hoch und überschreibt den Orbit-Speicher. | Uploads a JSON file and overwrites the cloud storage. |
| **# NOTAG** | Filtert alle Termine ohne Kategorien heraus. | Filters all events that have no tags assigned. |
| **ICS IMPORT** | Lädt Termindaten aus einer `.ics` Datei vor. | Pre-fills data from an `.ics` calendar file. |

---

## 🔒 Sicherheit / Security
**DE:** Die HTML-Datei enthält sensible Token-Daten. Hoste sie nur in privaten Umgebungen oder lokal.  
**EN:** This file contains sensitive API tokens. Host privately or run locally.

---
*Developed for Orbital Control Systems. Status: Operational.*
