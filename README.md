# 🛰️ Termin Monitor - Orbital Control

![Version](https://img.shields.io/badge/Version-3.3-00cae3.svg)
![Status](https://img.shields.io/badge/Status-Operational-00ff00.svg)

Ein hochoptimiertes Kontrollzentrum für Termine und Fristen. Entwickelt für maximale Übersichtlichkeit auf Desktop-Systemen und E-Ink-Dashboards, mit direkter Anbindung an die GitHub-Cloud.

---

## 🛠️ Neue Funktionen in v3.3

### 💾 Redundanz & Datensicherheit
* **Duale Backup-Strategie:** Deine Daten liegen primär verschlüsselt in der GitHub-Cloud. Mit der neuen **Backup-Funktion** kannst du jederzeit einen lokalen Snapshot als `.json` ziehen.
* **Ein-Klick-Restore:** Über den (jetzt rechtsbündig isolierten) **Restore-Button** lassen sich Backups einspielen, die sofort wieder mit dem Orbit (GitHub) synchronisiert werden.

### 🎨 Interface-Optimierung
* **System-Isolation:** Die Buttons für Backup und Restore wurden an den rechten Rand der Toolbar verschoben. Dies trennt administrative Aufgaben visuell von der Textformatierung (Links).
* **Adaptive Toolbar:** Auf mobilen Geräten stapeln sich die Buttons automatisch, um die Bedienbarkeit zu gewährleisten.

---

## 🚀 Kernfunktionen

| Feature | Beschreibung |
| :--- | :--- |
| **Cloud-Sync** | Volle Integration der GitHub API für geräteübergreifendes Arbeiten. |
| **Live-Erkennung** | Termine, die gerade stattfinden, werden prominent gelb markiert (**● LIVE NOW**). |
| **Smart Tags** | Automatisches Filtern nach Kategorien inkl. Spezial-Filter **# NOTAG** für Unsortiertes. |
| **Markdown+** | Unterstützung für Checkboxen, Fettdruck und Farbcodes direkt im Notizfeld. |
| **ICS-Schnittstelle** | Importiere externe Kalender-Events direkt per Datei-Upload. |

---

## ⚙️ Installation & Konfiguration

1.  **Repository:** Erstelle ein privates GitHub-Repo.
2.  **Datei:** Lege eine `termine.json` mit dem Inhalt `[]` an.
3.  **Authentifizierung:** * Erzeuge ein Personal Access Token (PAT) bei GitHub.
    * Teile das Token im Script auf `t1` und `t2` auf (Sicherheitsmaßnahme gegen einfache Scraper).
4.  **PIN-Schutz:** Der Standard-Zugang ist `0508`. Der Wert kann im Script unter `P_ENC` (Base64) geändert werden.

---

## 🔒 Sicherheitshinweis
Diese Anwendung ist für den **privaten Gebrauch** konzipiert. Da das API-Token im Quelltext segmentiert vorliegt, sollte die HTML-Datei nur lokal oder auf passwortgeschützten Servern gehostet werden.

---
*Orbital Control Systems - Secure. Sync. Succeed.*
