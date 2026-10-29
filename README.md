# fastingtracker App

# ⏱️ 16:8 Intervallfasten Tracker (PWA)

Eine minimalistische, datenschutzfreundliche Progressive Web App (PWA) für das **16:8 Intervallfasten** im nativen iOS-Dark-Mode-Design (Apple Watch / Health Look).

🔗 **Live-App:** [https://otc-demo.github.io/fastingtracker/](https://otc-demo.github.io/fastingtracker/)

---

## ✨ Features

* **Zentraler 16h-Fortschrittsring:** Live-Countdown der verbleibenden Fastenzeit, Prozentanzeige sowie automatische Überzeit-Berechnung (`+00:00:00`) nach Erreichen des 16-Stunden-Ziels.
* **Stoffwechsel-Phasen in Echtzeit:** Zeigt passend zur aktuellen Fastendauer an, in welcher physiologischen Phase sich der Körper befindet (Blutzuckerabfall, Glykogenabbau, Fettverbrennung & Ketose, Autophagie).
* **Startzeit nachträglich anpassen:** Über das Uhr-Symbol unten rechts lässt sich der Fastenbeginn jederzeit rückwirkend korrigieren, falls das Starten vergessen wurde.
* **Optionaler iOS-Timer & Benachrichtigung (Neu):** Auf Wunsch übergibt die App beim Starten oder Anpassen des Fastens die exakt verbleibenden Sekunden an die native iOS-Kurzbefehle-App und startet automatisch den System-Timer (inklusive Anzeige in der Dynamic Island und auf dem Sperrbildschirm).
* **Fasten-Historie:** Speichert abgeschlossene Fasteneinheiten übersichtlich mit Datum, Dauer und Zielstatus.
* **100 % Offline & Privat:** Keine Datenbank, kein Tracking, keine Cookies. Alle Daten bleiben lokal im `localStorage` des Browsers. Suchmaschinen-Indexierung ist per `noindex, nofollow` deaktiviert.
* **Optimiert für iOS:** Unterstützt Safe-Area-Abstände (Dynamic Island / Notch) sowie ein eigenes `apple-touch-icon` für den Homescreen.

---

## 📱 Installation als App auf dem iPhone (Homescreen)

1. Öffne [https://otc-demo.github.io/fastingtracker/](https://otc-demo.github.io/fastingtracker/) in **Safari** auf dem iPhone.
2. Tippe unten in der Leiste auf das **Teilen-Symbol** (Quadrat mit Pfeil nach oben).
3. Wähle **„Zum Home-Bildschirm“** aus und bestätige oben rechts mit **„Hinzufügen“**.
4. Die App startet nun vom Homescreen im Vollbildmodus ohne Browser-Leisten wie eine native App.

---

## 🔔 Optionale iOS-Benachrichtigung einrichten (iPhone-Timer)

Da iOS Hintergrund-Timer in reinen Web-Apps ohne externen Push-Server pausiert, nutzt diese App auf Wunsch eine direkte Schnittstelle zur nativen **Apple Kurzbefehle-App (Shortcuts)**. Das Feature ist standardmäßig deaktiviert und kann von jedem Nutzer selbst eingeschaltet werden.

### 1. Einmalig den Kurzbefehl auf dem iPhone anlegen
1. Öffne auf dem iPhone die vorinstallierte App **Kurzbefehle** und tippe oben rechts auf **`+`**.
2. Benenne den Kurzbefehl ganz oben exakt in **`Fasten`** um (Groß-/Kleinschreibung beachten).
3. Tippe auf **„Aktion hinzufügen“**, suche nach **„Timer starten“** und wähle die Aktion aus.
4. Passe die Zeile *„Timer starten für `[Dauer]` `[Minuten]`“* wie folgt an:
   * Stelle die Einheit von `Minuten` auf **`Sekunden`** um.
   * Halte den Finger auf das Feld **`[Dauer]`** gedrückt und wähle **„Kurzbefehl-Eingabe“** aus.
5. *(Optional)* Füge darunter als zweite Aktion **„Zum Home-Bildschirm“** hinzu, damit nach dem Starten des Timers sofort wieder der Homescreen bzw. die App im Vordergrund ist.
6. Tippe oben rechts auf **„Fertig“**.

### 2. Funktion in der Fasten-App aktivieren
1. Tippe in der Fasten-App unten rechts auf das **Uhr-Symbol** (*Startzeit anpassen*).
2. Aktiviere den Schalter **„Benachrichtigung bei Ziel“** (wird dauerhaft im Gerät gespeichert).
3. Sobald du nun auf **„Fasten beginnen“** oder im Anpassungsmenü auf **„Übernehmen“** tippst, wird automatisch ein nativer iPhone-Timer mit der exakt verbleibenden Restzeit bis zum 16-Stunden-Ziel gestartet.

---

## 🛠️ Tech-Stack

* **HTML5 & Vanilla JavaScript** (Keine Build-Tools oder Frameworks nötig)
* **Tailwind CSS** (via CDN)
* **Lucide Icons** (via CDN)
* **Web Storage API** (`localStorage` für Zustand, Einstellungen & Historie)
