# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.5-00cae3.svg)
![Status](https://img.shields.io/badge/Status-Operational-00ff00.svg)

---

## 🇩🇪 Deutsch: Übersicht

Ein Kontrollzentrum für Termine, Fristen und Zeitfenster. Optimiert für die Desktop-Verwaltung in `index.html` sowie für passive E-Ink-Dashboards über `display.html`, mit direkter GitHub-Cloud-Synchronisation.

### 🚀 Kernfunktionen

- **Echtzeit-Sync:** Speichert Daten direkt im GitHub-Repository über die REST API.
- **Backup & Restore:** Lokale JSON-Snapshots erstellen und mit einem Klick wiederherstellen.
- **Duale Ansicht:** Wechsel zwischen Monitor-Liste und grafischem Kalender.
- **Intelligente Sortierung:** Vor einer Startzeit nach START, danach nach ENDE/Fälligkeit sortiert.
- **Tages-Trenner:** Termine werden nach ihrem relevanten Tag gruppiert. Beim Übergang zum nächsten Tag zeigt eine deutlich sichtbare Datums-Trennlinie, wo der neue Tag beginnt.
- **Überfälligkeits-Zähler:** Nach Ablauf bleibt ein Termin klar als `FÄLLIG` markiert und zeigt zusätzlich die bereits verstrichene Zeit an, z. B. `ÜBERFÄLLIG SEIT 02d 05:18:00`.
- **Monate & Resttage:** Zusätzlich zum Countdown wird die verbleibende Zeit als volle Monate und Resttage angezeigt.
- **Smart Filtering:** LIVE-Erkennung, Archiv-Funktion und dynamische Tag-Filter.
- **Rich Text & Checklisten:** Unterstützt Fettdruck, Kursivschrift, Unterstreichung, Durchstreichung, farbige Notizen und strukturierte Checklisten.
- **ICS-Import:** Importiert Termine aus `.ics`-Kalenderdateien; einzelne Einträge können vor dem Import ausgewählt werden.
- **Display-Optimierung:** Separate, bewusst minimalistische `display.html` für E-Ink- und passive Bildschirme.
- **Wiederholungslogik:** Täglich, wöchentlich mit festen Tagen, zweiwöchentlich, monatlich per Datum, monatlich per Wochentag, halbjährlich und jährlich.

### 🖥️ Hauptansicht und Display

| Bereich | `index.html` | `display.html` |
|---|---|---|
| Zweck | Verwalten, erstellen und bearbeiten | Passive, reine Anzeige |
| Login | PIN-Login erforderlich | Kein Login |
| Ansicht | Monitor, Kalender, Editor, Filter | Reduzierte Terminübersicht |
| Aktualisierung | Live-Countdown im Sekundentakt | Datenabruf und Anzeigeaktualisierung alle 60 Sekunden |
| Tages-Trenner | Ja | Ja, für E-Ink vereinfacht |
| Überfälligkeits-Zähler | Ja, sekundengenau | Ja, im Minutenraster |

---

## 🇺🇸 English: Overview

A control center for appointments, deadlines, and time windows. It is optimized for desktop management in `index.html` and passive E-Ink dashboards via `display.html`, with direct GitHub cloud synchronization.

### 🚀 Key Features

- **Real-Time Sync:** Persists data directly to a GitHub repository through the REST API.
- **Backup & Restore:** Create local JSON snapshots and restore them with one click.
- **Dual Interface:** Toggle between the Monitor List and a graphical Calendar.
- **Intelligent Sorting:** Sorts by START before an item begins, then by END/deadline afterwards.
- **Day Separators:** Groups appointments by their relevant day and adds a clear date separator when the next day starts.
- **Overdue Counter:** After an item expires, it remains visibly marked as `DUE` and additionally shows elapsed overdue time, for example `OVERDUE FOR 02d 05:18:00`.
- **Months & Remaining Days:** Shows complete months and remaining days alongside the countdown.
- **Smart Filtering:** LIVE detection, archiving, and dynamic tag filters.
- **Rich Text & Checklists:** Supports bold, italic, underline, strikethrough, colored notes, and structured checklists.
- **ICS Import:** Imports appointments from `.ics` calendar files, including pre-import item selection.
- **Display Optimization:** A separate, deliberately minimalist `display.html` for E-Ink and passive screens.
- **Recurrence Logic:** Daily, weekly with fixed weekdays, biweekly, monthly by date, monthly by weekday, half-yearly, and yearly.

---

## 📁 Dateistruktur / File Structure

```text
├── index.html       # Haupt-Editor + Monitor + Kalender; PIN-Login erforderlich
├── display.html     # Passive E-Ink-/Dashboard-Anzeige; read-only, kein Login
├── termine.json     # Datenbank: JSON-Array mit allen Terminen
└── README.md        # Diese Dokumentation
```

---

## 📜 Versions-Historie / Version History

### **v1.0 - The Core (Basis)**

- **DE:** Grundlegendes Listing, lokale Speicherung, einfaches Design.
- **EN:** Basic listing, local storage, simple design.

### **v2.0 - Orbital Sync**

- **DE:** Einführung der GitHub-API-Anbindung für Cloud-Sync. PIN-Login-System integriert.
- **EN:** Introduction of GitHub API cloud synchronization and an integrated PIN login system.

### **v3.0 - Tactical UI**

- **DE:** Neues „Orbital“-Dark-Design, Countdown-Timer und Tag-System.
- **EN:** New Orbital dark design, countdown timers, and tag system.

### **v3.1 - Calendar & Rich Text**

- **DE:** Kalenderansicht und erweiterte Textformatierung mit Fett, Farben und Checkboxen.
- **EN:** Calendar view and enhanced text formatting with bold text, colors, and checkboxes.

### **v3.2 - Redundancy Update**

- **DE:** Backup- und Restore-Logik für JSON-Dateien ergänzt.
- **EN:** Added backup and restore logic for JSON files.

### **v3.3 - System Layout**

- **DE:** Toolbar optimiert; Backup- und Restore-Buttons rechtsbündig isoliert.
- **EN:** Toolbar optimization; backup and restore buttons isolated on the right.

### **v3.4 - Smart Sorting**

- **DE:** Intelligente Sortierung: Termine mit Startzeit werden vor dem Start nach START, danach nach ENDE sortiert. Die Logik gilt für `index.html` und `display.html`.
- **EN:** Intelligent sorting: appointments with start times are sorted by START before beginning and by END afterwards. Applied to `index.html` and `display.html`.

### **v3.5 - Day Segments & Overdue Tracking (Current)**

- **DE:** Ergänzt sichtbare Tages-Trenner in Monitor und E-Ink-Display. Der heutige Bereich wird besonders markiert. Überfällige Termine bleiben auf `FÄLLIG` und zeigen zusätzlich eine fortlaufende Zeit seit dem Fälligkeitszeitpunkt. Die Monats-/Resttage-Anzeige bleibt erhalten.
- **EN:** Added visible day separators in both the Monitor and E-Ink display. Today is highlighted. Overdue items remain marked as `DUE` and additionally show elapsed time since their deadline. The months/remaining-days display remains available.

---

## ⚙️ Einrichtung / Setup (DE/EN)

1. **GitHub:** Erstelle ein privates Repository mit einer Datei `termine.json`; ihr initialer Inhalt ist `[]`.
2. **Token:** Erzeuge einen GitHub Personal Access Token (classic) mit passendem Repository-Zugriff und hinterlege ihn im Code. Für die bestehende Aufteilung werden `t1` und `t2` verwendet.
3. **PIN:** Die aktuelle Standard-PIN ist `0508`. Für eine Änderung den passenden Base64-Wert in `P_ENC` aktualisieren.
4. **URLs:** Passe `G_URL` in `index.html` beziehungsweise `GITHUB_URL` in `display.html` auf dein Repository an.
5. **Datenformat:** Jeder Termin wird in `termine.json` als Objekt im JSON-Array gespeichert. Pflichtfelder sind mindestens Titel (`name`) und Fälligkeit/Ende (`ziel`).

### Für E-Ink- und Passive-Displays

- `display.html` direkt öffnen; ein Login ist nicht erforderlich.
- Die Daten werden automatisch alle 60 Sekunden von GitHub neu geladen.
- Die Anzeige wird ebenfalls im 60-Sekunden-Raster aktualisiert.
- Die Ansicht ist absichtlich read-only und auf gute Lesbarkeit bei geringer Farbvielfalt ausgelegt.

---

*Orbital Control Systems v3.5 - Precision Scheduling for Mission Critical Operations.*
