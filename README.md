🚀 Termin Monitor - Orbital Control

Ein minimalistisches, weltraum-inspiriertes Dashboard zur Terminverwaltung mit Echtzeit-Synchronisation über die GitHub API.
🌌 Features

    Echtzeit-Countdown: Alle Termine werden sekundengenau bis zum Zielzeitpunkt heruntergezählt.

    GitHub-Sync: Speichert alle Daten automatisch in einer termine.json in deinem Repository (funktioniert als serverlose Datenbank).

    Formatierungs-Tools: Integrierte Toolbar für Fettschrift, ~~Durchstreichen~~ und Farben.

    Checkbox-System: Aufgabenlisten direkt in den Notizen erstellen und abhaken.

    ICS-Import: Importiere Kalenderdaten direkt aus .ics Dateien.

    Sicherer Zugang: Geschütztes System durch ein PIN-Login-Overlay und Session-Management (Logout-Funktion).

    Responsive Design: Optimiert für Desktop und mobile Endgeräte mit Glasmorphismus-Effekten.

🛠️ Installation & Setup

    Repository spiegeln: Lade die index.html in dein GitHub-Repository hoch.

    Datenstruktur: Erstelle eine leere termine.json im selben Verzeichnis (Inhalt: []).

    API-Token: Stelle sicher, dass dein GitHub Personal Access Token (PAT) im Code hinterlegt ist, um Schreibrechte auf die JSON-Datei zu haben.

    Hosten: Aktiviere GitHub Pages in den Repository-Einstellungen, um den Monitor weltweit unter deiner .github.io URL aufzurufen.

📂 Dateistruktur

    index.html: Die gesamte App (HTML5, CSS3, Vanilla JavaScript).

    termine.json: Die Datenbank, in der alle Einträge verschlüsselt (Base64) gespeichert werden.

🔐 Sicherheitshinweis

Dieses Projekt nutzt ein Client-seitiges Token-Management. Für maximale Sicherheit in öffentlichen Repositories wird empfohlen, den Token über GitHub Actions oder ein Backend zu verschleiern.

---

Here is the professional English version of the README.md. I’ve polished the wording to give it a high-tech "Command Center" feel, matching your code's aesthetic.
🚀 Appointment Monitor - Orbital Control

A minimalist, space-inspired dashboard for appointment management featuring real-time synchronization via the GitHub API.
🌌 Features

    Real-Time Countdown: All appointments are tracked down to the second with a live countdown timer.

    GitHub Cloud Sync: Automatically saves and fetches data from a termine.json file in your repository (acting as a serverless database).

    Rich Text Toolbar: Integrated formatting tools for Bold, ~~Strikethrough~~, and custom text colors.

    Dynamic Checklists: Create and toggle interactive task lists directly within your notes.

    ICS Import: Seamlessly import calendar events from standard .ics files.

    Secure Access: Protected by a PIN-coded "System Login" overlay and local session management (Logout functionality).

    Glassmorphism UI: High-fidelity space aesthetic using NASA imagery and modern CSS backdrop filters.

🛠️ Installation & Setup

    Repository Setup: Upload the index.html to your GitHub repository.

    Database Initialisation: Create a file named termine.json in the same directory with the content [].

    API Configuration: Ensure your GitHub Personal Access Token (PAT) is correctly configured within the script variables to allow write access.

    Deployment: Enable GitHub Pages in your repository settings to access your monitor via your personal github.io URL.

📂 File Structure

    index.html: The core application (HTML5, CSS3, Vanilla JavaScript).

    termine.json: The database file storing all entries in a JSON structure.

🔐 Security Disclaimer

This project uses client-side token management for simplicity. For deployment in public environments, it is recommended to restrict token scopes or use a backend proxy to keep credentials hidden from the source code.
