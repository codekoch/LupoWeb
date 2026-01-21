# 🎓 <a href="https://codekoch.github.io/LupoWeb/lupo_web.html">LuPO Web </a>- NRW Oberstufen-Planung im Browser

Eine webbasierte, systemunabhängige Alternative zum offiziellen LuPO-Programm für die Laufbahnberatung in der gymnasialen Oberstufe (NRW).

⚠️ Wichtiger Hinweis: Dies ist keine offizielle Software des Landes NRW oder von SVWS. Es handelt sich um ein Community-Projekt. Die Nutzung erfolgt auf eigene Gefahr. Bitte überprüfen Sie alle Planungen stets auf Konformität mit der aktuellen APO-GOSt.

🌟 Über das Projekt
Das offizielle LuPO-Programm (Laufbahn- und Planungstool Oberstufe) ist eine Windows-Anwendung. In einer immer diverseren Gerätelandschaft (iPads, MacBooks, Chromebooks) stellt dies Schulen oft vor technische Hürden.

LuPO Web löst dieses Problem: Es ist eine reine HTML-Datei, die in jedem modernen Browser läuft.

Keine Installation notwendig.

Läuft offline (nach dem Laden).

Datenschutzfreundlich: Alle Daten bleiben im Browser des Nutzers, nichts wird auf Server hochgeladen.

Dieses Projekt entstand ursprünglich als "Proof of Concept" mit Unterstützung von KI (Antigravity), um zu zeigen, wie leicht bestehende Sofware modernisert werden kann. Die Community ist herzlich eingeladen, den Code zu verbessern und aktuell zu halten!

✨ Features
Das Projekt besteht aus zwei Hauptkomponenten:

1. Lehrer-Manager (<a href="https://codekoch.github.io/LupoWeb/lupo_web.html">lupo_web.html</a>)
Konfiguration: Aktivieren/Deaktivieren von Fächern, Festlegen von Stundenzahlen, Start-/Endphasen und Zusatzkursen.

Regelwerk: Definition von "Verbotenen Fächerkombinationen" (z.B. Religionslehre vs. Philosophie).

Export: Generiert per Knopfdruck die Schüler-Version als eigenständige HTML-Datei, die genau auf das Schulprofil zugeschnitten ist.

2. Schüler-Wahl & Abirechner (<a href="https://codekoch.github.io/LupoWeb/lupo_schueler_wahl.html">lupo_schueler_wahl.html</a>)
Laufbahnplanung: Interaktive Wahl von EF.1 bis Q2.2.

Validierung: Prüft live gegen gängige Belegungsverpflichtungen (z.B. "Kunst/Musik in Q1", "Durchgehende Fremdsprache", "Schwerpunkt", "Anzahl LKs").

Abitur-Planung: Wahl der 4 Abiturfächer mit Prüfung der Aufgabenfelder.

🧮 Zulassungsrechner (Block I): Ein integrierter Rechner erlaubt es Schülern, ihre (erwarteten) Noten einzutragen. Das Tool berechnet live die Zulassung, zählt Defizite und prüft Pflichteinbringungen.

Speichern/Laden: Planungen können als lokale Datei (.txt/.json) gespeichert und später wieder geladen werden.

🚀 Nutzung
Für Administratoren / Oberstufenkoordinatoren
Lade die Datei lupo_web_Kochrezept.html herunter und öffne sie im Browser.

Konfiguriere das Fächerangebot deiner Schule (Reiter "Konfiguration").

Klicke auf "Exportieren (.html)".

Verteile die heruntergeladene Datei (lupo_schueler_wahl.html) an die Schülerschaft (z.B. via Moodle, Teams oder E-Mail).

Für Schülerinnen und Schüler
Öffne die erhaltene HTML-Datei im Browser (am PC, Tablet oder Handy).

Wähle deine Fächer und Abiturfächer.

Achte auf die Hinweise in der rechten Spalte (Fehler/Warnungen).

Nutze den Reiter "Noten & Zulassung", um deine Punkte zu simulieren.

Klicke auf "Speichern", um deinen Stand zu sichern, oder "Drucken" für ein Beratungsgespräch.

🛠️ Technische Details
Stack: React 18, TailwindCSS, Babel Standalone.

Single File: Der gesamte Code (Logik, Styles, UI) befindet sich in einer einzigen HTML-Datei. Es ist kein Build-Prozess (Node.js, Webpack, etc.) nötig, um die Datei zu nutzen oder anzupassen.

Datenformat: Die Speicherdateien sind einfaches JSON.

🤝 Mitwirken (Contributing)
Da dieses Projekt auf einem KI-Entwurf basiert, ist es "Work in Progress". Die APO-GOSt ist komplex und ändert sich. Es werden sicherlich noch Sonderfälle fehlen (z.B. Projektkurse, spezielle Sportprofile, Bilingualer Zweig).

Du bist herzlich eingeladen, mitzuwirken!

Forke das Repository.

Öffne die HTML-Dateien in einem Code-Editor.

Der React-Code befindet sich direkt im <script type="text/babel"> Tag.

Verbessere die Validierungslogik (VALIDATION_LOGIC Variable) oder das UI.

Erstelle einen Pull Request.

Wir suchen besonders Hilfe bei:

Verfeinerung der Validierungsregeln (Sonderfälle).

Verbesserung der "Print"-Ansicht (CSS).

Erweiterung um Import-Funktionen für offizielle LuPO-Dateien (.lup).

📄 Lizenz & Haftung
Der Quellcode ist Open Source. Haftungsausschluss: Die Berechnungen in diesem Tool dienen lediglich der Orientierung. Rechtsverbindlich sind ausschließlich die Beratungen durch die Oberstufenkoordinatoren und die offizielle Berechnung in der Schild-NRW Datenbank. Für Entscheidungen, die auf Basis dieser Software getroffen werden, wird keine Haftung übernommen.
