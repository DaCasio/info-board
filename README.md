Hier ist eine strukturierte **README.md** für dein GitHub-Repository, die beide Dateien (`index.html` für die Verwaltung und `display.html` für die Anzeige) erklärt.

---

# 🚀 Orbital Termin Monitor

Ein minimalistisches, GitHub-basiertes Termin-Management-System. Es besteht aus einem interaktiven Dashboard zur Verwaltung und einer optimierten Anzeige für Color E-Ink Displays oder Wandmonitore.

## 📋 Features

* **Zwei-Komponenten-System:**
* `index.html`: Admin-Panel mit PIN-Schutz, Erstellung, Bearbeitung und Archivierung von Terminen.
* `display.html`: Clean-Display-Ansicht, optimiert für E-Ink (keine Gradients, hoher Kontrast).


* **Archiv-Funktion:** Termine mit dem Tag `ARCHIV` werden automatisch aus der Hauptansicht ausgeblendet und in einen separaten Archiv-Bereich verschoben.
* **Serverless:** Nutzt die GitHub API als Backend (JSON-Datenbank).
* **Smart Features:** Countdown-Anzeige, Checklisten-Support in den Notizen, Farbcodes und ICS-Import.

---

## 🛠 Einrichtung / Setup

1. Erstelle eine Datei namens `termine.json` in deinem Repository mit folgendem Inhalt: `[]`.
2. Stelle sicher, dass dein **GitHub Personal Access Token (PAT)** in den HTML-Dateien hinterlegt ist (Variablen `t1` und `t2`).
3. Passe die `G_URL` / `GITHUB_URL` an dein Repository an.

---

## 📖 Komponenten / Components

### 1. Termin-Verwaltung (`index.html`)

Das Kontrollzentrum für deine Termine.

* **Login:** Gesichert durch eine PIN (Base64 kodiert).
* **Tags:** Nutze Tags zur Kategorisierung.
* **Archivierung:** Füge das Tag `ARCHIV` hinzu, um einen Termin aus der aktiven Liste zu entfernen. Er bleibt in der Datenbank, ist aber nur noch über den "Archiv"-Filter sichtbar.
* **Editor:** Unterstützt Fett-Text (`**`), Durchstreichen (`--`), Farben und interaktive Checkboxen (`[ ]` / `[x]`).

### 2. E-Ink Display (`display.html`)

Die reine Anzeige-Oberfläche.

* **Auto-Filter:** Blendet alle Termine mit dem Tag `ARCHIV` automatisch aus.
* **Optimiertes Design:** Klare Linien und kräftige Farben für eine perfekte Lesbarkeit auf digitalen Bilderrahmen oder E-Paper Displays.
* **Live-Update:** Aktualisiert die Daten alle 30 Sekunden automatisch von GitHub.

---

# 🇬🇧 English Version

## 📋 Overview

A minimalist appointment monitoring system using GitHub as a backend.

* `index.html`: Administrative dashboard for creating and managing tasks.
* `display.html`: High-contrast view optimized for Color E-Ink displays.

## 📁 Archive Logic

* **Archiving:** Any appointment tagged with `ARCHIV` (case-insensitive) will be hidden from the "ALL" view in the dashboard and completely hidden from the `display.html`.
* **Restoring:** Simply remove the `ARCHIV` tag to make the appointment visible on the monitor again.

## 🚀 Deployment

1. Initialize a `termine.json` file in your repo: `[]`.
2. Update the GitHub Token and Repo URL in both HTML files.
3. Open `index.html` to start managing your orbital schedule.
