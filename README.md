fastingtracker App

⏱️ 16:8 Intervallfasten Tracker (PWA)

Eine minimalistische, datenschutzfreundliche Progressive Web App (PWA) für das 16:8 Intervallfasten im nativen iOS-Dark-Mode-Design (Apple Watch / Health Look).

✨ Features

Zentraler 16h-Fortschrittsring: Live-Countdown der verbleibenden Fastenzeit, Prozentanzeige sowie automatische Überzeit-Berechnung (+00:00:00) nach Erreichen des 16-Stunden-Ziels.

Stoffwechsel-Phasen in Echtzeit: Zeigt passend zur aktuellen Fastendauer an, in welcher physiologischen Phase sich der Körper befindet (Blutzuckerabfall, Glykogenabbau, Fettverbrennung & Ketose, Autophagie).

Startzeit nachträglich anpassen: Über das Uhr-Symbol unten rechts lässt sich der Fastenbeginn jederzeit rückwirkend korrigieren, falls das Starten vergessen wurde.

Optionales Gewichts-Tracking (Neu): Kann flexibel in den Einstellungen aktiviert werden. Ermöglicht die unkomplizierte Eingabe des heutigen Gewichts direkt im Essensfenster und speichert dieses tagesbasiert in der Historie ab.

Optionaler iOS-Timer & Benachrichtigung: Auf Wunsch übergibt die App beim Starten oder Anpassen des Fastens die exakt verbleibenden Sekunden an die native iOS-Kurzbefehle-App und startet automatisch den System-Timer (inklusive Anzeige in der Dynamic Island und auf dem Sperrbildschirm).

Fasten-Historie: Speichert abgeschlossene Fasteneinheiten übersichtlich mit Datum, Dauer, Zielstatus und (optional) dem eingetragenen Gewicht.

100 % Offline & Privat: Keine Datenbank, kein Tracking, kein Backend. Alle Daten bleiben lokal im localStorage des Browsers. Suchmaschinen-Indexierung ist per noindex, nofollow deaktiviert.

Optimiert für iOS: Unterstützt Safe-Area-Abstände (Dynamic Island / Notch) sowie ein eigenes apple-touch-icon für den Homescreen.

📱 Installation als App auf dem iPhone (Homescreen)

Öffne den Link in Safari auf dem iPhone.

Tippe unten in der Leiste auf das Teilen-Symbol (Quadrat mit Pfeil nach oben).

Wähle „Zum Home-Bildschirm“ aus und bestätige oben rechts mit „Hinzufügen“.

Die App startet nun vom Homescreen im Vollbildmodus ohne Browser-Leisten wie eine native App.

⚖️ Gewichts-Tracking nutzen

Tippe in der Fasten-App unten rechts auf das Uhr-Symbol (Startzeit anpassen & Einstellungen).

Aktiviere den Schalter „Gewichts-Tracking“ (wird direkt im Gerät gespeichert).

Im Essensfenster (wenn kein aktives Fasten läuft) erscheint nun ein dezentes Eingabefeld, in dem du dein heutiges Gewicht eintragen und speichern kannst.

Das Gewicht wird automatisch mit in deiner Fasten-Historie abgespeichert und dort in der Tagesübersicht angezeigt.

🔔 Optionale iOS-Benachrichtigung einrichten (iPhone-Timer)

Da iOS Hintergrund-Timer in reinen Web-Apps ohne externen Push-Server pausiert, nutzt diese App eine direkte Schnittstelle zur nativen Apple Kurzbefehle-App (Shortcuts).

1. Einmalig den Kurzbefehl importieren

Tippe in den App-Einstellungen auf den Link „Kurzbefehl laden“ und lade diesen direkt auf dein iPhone (benötigt einmalig die Kurzbefehle-App).

2. Funktion in der Fasten-App aktivieren

Tippe in der Fasten-App unten rechts auf das Uhr-Symbol.

Aktiviere den Schalter „Benachrichtigung bei Ziel“.

Sobald du nun auf „Fasten beginnen“ oder im Anpassungsmenü auf „Übernehmen“ tippst, wird automatisch ein nativer iPhone-Timer mit der exakt verbleibenden Restzeit bis zum 16-Stunden-Ziel gestartet.

🛠️ Tech-Stack

HTML5 & Vanilla JavaScript (Keine Build-Tools oder Frameworks nötig)

Tailwind CSS (via CDN)

Lucide Icons (via CDN)

Web Storage API (localStorage für Zustand, Einstellungen & Historie)
