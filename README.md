# 🛰️ Termin Monitor - Orbital Control System

![Version](https://img.shields.io/badge/Version-3.3-00cae3.svg)
![Build](https://img.shields.io/badge/Build-Operational-00ff00.svg)
![License](https://img.shields.io/badge/License-Private-ff4d4d.svg)

A high-performance, browser-based scheduling and monitoring dashboard with a tactical "Orbital" aesthetic. Optimized for desktop management and passive E-Ink displays, featuring direct cloud synchronization via the GitHub REST API.

---

## 🚀 Key Features

* **Real-Time Cloud Sync:** Persists all data directly to a private GitHub repository.
* **Dual-View Interface:** Seamlessly toggle between a tactical **Monitor List** and a full **Monthly Calendar**.
* **Smart Filtering:** Includes specialized filters for "LIVE NOW" events, archived data, and a unique **# NOTAG** filter for uncategorized entries.
* **Rich Text & Tasks:** Native support for Markdown-style bolding, custom color codes, and interactive checkboxes within notes.
* **Redundancy System:** Integrated **Backup (Export)** and **Restore (Import)** functions for local data safety.
* **ICS Integration:** Directly pre-fill event data from standard `.ics` calendar files.

---

## 🛠️ Installation & Setup

1.  **Repository:** Create a private GitHub repository.
2.  **Storage:** Initialize a file named `termine.json` containing only `[]`.
3.  **Authentication:** * Generate a GitHub Personal Access Token (PAT) with `repo` scope.
    * Split the token into constants `t1` and `t2` within the script.
4.  **URL:** Update the `G_URL` constant in the script to match your repository path.
5.  **Security:** The default PIN is `0508`. Change the Base64 string in `P_ENC` for custom security.

---

## 📜 Version History (Changelog)

### **v1.0 - The Foundation**
* Initial release of the "Info-Board".
* Basic GitHub API integration for saving and loading.
* Simple list view of upcoming deadlines.

### **v2.0 - Tactical UI & UX**
* Introduced the "Orbital" dark-mode design with NASA imagery.
* Added the **Countdown Engine** (days, hours, minutes, seconds).
* Implemented **Tagging System** and basic filtering.
* Added the **Copy/Duplicate** function for recurring tasks.

### **v3.0 - The Calendar Update**
* Integrated a full **Interactive Calendar View**.
* Added **Event Duration** support (Start-Date vs. End-Date).
* Introduced the **"LIVE NOW"** status for ongoing events.
* Enhanced Note Formatting: Bolding (`**`), Strikethrough (`--`), and Custom Colors (`[color:...]`).

### **v3.1 - Connectivity & Tasks**
* Added **ICS File Import** for external calendar integration.
* Implemented **Interactive Checkboxes** within the note field (`[ ]` / `[x]`).
* Auto-refresh logic (60s sync / 1s UI update).

### **v3.2 - Redundancy Update**
* Added **💾 BACKUP** function: Export all data as a local `.json` file.
* Added **📂 RESTORE** function: Overwrite cloud data with a local backup file (including safety confirmation).

### **v3.3 - Layout Finalization (Current)**
* **System Isolation:** Realigned Backup/Restore buttons to the right side of the toolbar to separate administrative tasks from content formatting.
* **Responsive Fixes:** Improved mobile behavior for the new toolbar layout.
* **Status Logic:** Refined countdown priorities between Start and End dates.

---

## 🔒 Security Disclaimer
This application is designed for **private use**. Because the API tokens are stored in the client-side code (even if segmented), this HTML file should only be hosted in private environments or run locally.

---
*Developed for Orbital Control Systems. Status: Fully Operational.*
