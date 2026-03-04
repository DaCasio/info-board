# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.0-00cae3.svg)
![License](https://img.shields.io/badge/License-Private-ff4d4d.svg)
![Status](https://img.shields.io/badge/Status-Operational-00ff00.svg)

Ein hochmoderner, browserbasierter Termin-Planer mit orbitalem Design und direkter Cloud-Synchronisation via GitHub API. Optimiert für Desktop-Management und passive E-Ink-Displays.
A state-of-the-art, browser-based appointment planner featuring an orbital design and direct cloud synchronization via the GitHub API. Optimized for desktop management and passive e-ink displays.
---

## 🚀 Kernfunktionen / Core Features

### 🇩🇪 Deutsch
* **Echtzeit-Synchronisation:** Speichert Daten direkt in deinem GitHub-Repo via REST API.
* **Duale Ansicht:** Wechsel zwischen einer taktischen **Monitor-Liste** und einer strategischen **Kalender-Ansicht**.
* **Intelligentes Filtersystem:** Automatische "LIVE NOW" Erkennung, Archiv-Funktion und der neue **# NOTAG** Filter für unsortierte Einträge.
* **Präzisions-Countdown:** Live-Ticks für verbleibende Zeit bis zum Start oder Ende eines Termins.
* **Rich Content:** Unterstützt Markdown-Formatierung, Farben und interaktive Checkboxen innerhalb der Notizen.
* **ICS-Schnittstelle:** Schneller Import von Terminen aus externen Kalender-Dateien.

### 🇺🇸 English
* **Real-Time Sync:** Persists data directly to your private GitHub repository via REST API.
* **Dual Interface:** Toggle between a tactical **Monitor List** and a strategic **Calendar View**.
* **Smart Filtering:** Features automatic "LIVE NOW" detection, archiving, and the new **# NOTAG** filter for uncategorized entries.
* **Precision Countdown:** Live ticking countdowns for both start times and deadlines.
* **Rich Content:** Native support for Markdown-style formatting, colors, and interactive checkboxes in notes.
* **ICS Interface:** Quick import functionality for external calendar files.

---

## 🛠️ Einrichtung / Setup Instructions

### 1. Repository Setup
* **DE:** Erstelle ein privates Repo und eine `termine.json` mit dem Inhalt `[]`.
* **EN:** Create a private repo and an empty `termine.json` containing `[]`.

### 2. Authentication (GitHub PAT)
* **DE:** Erstelle ein Personal Access Token (classic) mit `repo` Scope. Teile es im Code auf `t1` und `t2` auf.
* **EN:** Generate a Personal Access Token (classic) with `repo` scope. Split the token into `t1` and `t2` variables in the code.

### 3. Configuration
* **DE:** Passe `G_URL` an deinen User- und Repository-Namen an. Standard-PIN: `0508`.
* **EN:** Adjust `G_URL` to match your username and repo. Default PIN: `0508`.

---

## 📖 Bedienung / How to Use

| Aktion / Action | Beschreibung / Description (DE) | Description (EN) |
| :--- | :--- | :--- |
| **Save** | Titel + Enddatum sind Pflicht. | Title + End Date are required. |
| **Search** | Filtert Titel und Notizen in Echtzeit. | Filters titles and notes in real-time. |
| **NOTAG Filter** | Findet alle Termine ohne Kategorien. | Finds all appointments without tags. |
| **Checkboxes** | Klickbare Aufgaben in der Kartenansicht. | Clickable to-do items directly in the card. |
| **Archive** | Tag `ARCHIV` versteckt den Termin. | Tag `ARCHIV` hides entry from main list. |
| **Calendar** | Visualisiert Termine im Monatsraster. | Visualizes events in a monthly grid. |

---

## 🔒 Sicherheit / Security Note
**DE:** Da das Tool das GitHub-Token im Quellcode nutzt, darf die Datei **niemals öffentlich** zugänglich sein. Hosting nur via GitHub Pages (Privat) oder lokal.

**EN:** Since this tool stores the GitHub token in the source code, the file must **never be made public**. Host via private GitHub Pages or run locally.

---
*Developed for Orbital Control Systems. Status: Operational.*
