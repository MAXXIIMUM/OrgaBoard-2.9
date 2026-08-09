# OrgaBoard

Fertige statische Version für GitHub Pages.

## Enthalten
- Wochenplanung und Login
- Automatische Terminfarben
- Verkauf: Produkt und Modell auswählbar
- Altgeräte-Modellauswahl
- K70 frei eintragbar
- Automatischer PDF-Download im A4-Querformat
- Mobilfreundliche PDF-Beschriftung
- Lokale Speicherung im Browser

## GitHub Pages
1. Den Inhalt der ZIP-Datei in ein GitHub-Repository hochladen.
2. Settings → Pages öffnen.
3. "Deploy from a branch" auswählen.
4. Branch `main` und Ordner `/ (root)` auswählen.
5. Speichern.

Hinweis: Termine werden aktuell im Browser des jeweiligen Geräts gespeichert.


## Benutzer
- Björn Hahne
- Jessica Wunder
- Thomas Villnow (BM)
- Carsten Böhrensen (TL)

Passwort für alle Benutzer: `Test`


## Getrennte Benutzerbereiche
Jeder Benutzer verwendet einen eigenen localStorage-Bereich. Termine und Umsätze von Björn, Jessica und Tohmas werden nicht miteinander vermischt.


## Zubehör
Die Produktauswahl enthält jetzt eine umfangreiche Vorwerk-Kobold-Zubehörliste. Bei Zubehör kann zusätzlich eine freie Bezeichnung eingegeben werden.


## Vorführung & Geräteverleih
Bei Vorführgeräten kann passendes Zubehör ausgewählt oder frei eingetragen werden. Geräteverleih verfügbar für VK7, VR7, VT300, VG100+ und VM7 mit den angegebenen Zubehör-/Stationspaketen.


## Produkt-KI & App-Icon
Die App enthält einen lokalen Produkt-Assistenten mit eingebettetem Vorwerk-Katalog, Suchfunktion und Produktbeschreibungen. Außerdem sind App-Icon, Apple-Touch-Icon und Web-App-Manifest enthalten.


## Produktbilder
Die enthaltenen Produktbilder für VK7, VR7, SP7 und TM7 stammen von offiziellen Vorwerk-Medienseiten und werden lokal aus dem `assets`-Ordner geladen.


## Dustin Login
Die Login-Seite enthält das bereitgestellte Dustin-Motiv als professionelles Hero-Visual.


Dustin wird auf der Login-Seite als Bild aus `assets/dustin-login.jpg` geladen.


## Verkaufspreise
Bei jedem verkauften Artikel kann jetzt ein Preis pro Stück eingetragen werden. Die Positionssumme wird automatisch aus Anzahl × Preis berechnet und in den Wochenumsatz übernommen.


## Direkter Verkauf
Der Menüpunkt `Verkäufe` und der Schnellzugriff `Neuer Verkauf` öffnen jetzt ein eigenes Verkaufsfenster. Dort werden Produkt, Modell, Anzahl und Preis pro Stück eingetragen. Die Gesamtsumme wird automatisch berechnet und zum Wochenumsatz addiert.


## Handy-Kalender
Neue Termine können beim Speichern als `.ics`-Kalenderdatei an das Handy übergeben werden. Auf unterstützten Mobilbrowsern öffnet sich die Teilen-Funktion; ansonsten wird eine Kalenderdatei heruntergeladen, die mit Apple Kalender, Google Kalender oder anderen Kalender-Apps geöffnet werden kann.


## Verkauf wie Vorführung
Im Verkaufsbereich stehen jetzt wie bei der Vorführung Bereich/Produkt, Modell und Zubehör zur Auswahl. Zusätzlich bleiben Anzahl, Preis pro Stück und automatische Summe erhalten.


## Umsatzarten
Die Umsatzübersicht trennt jetzt Produktumsatz und K70-Umsatz. Gesamt eingenommen = Produktumsatz + K70-Umsatz. K70 kann im Verkaufsbereich frei eingetragen werden.


## Produktumsatz direkt im Termin
Im Terminfenster stehen jetzt zusätzlich `Produktumsatz (€)`, `Verkauftes Produkt` und `Modell`. Der Produktumsatz ist frei eintragbar und wird getrennt vom K70-Umsatz in der Wochenübersicht berücksichtigt.


## Mehrere Produkte pro Termin
Im Terminfenster können jetzt über `+ Weiteres Produkt hinzufügen` beliebig mehrere verkaufte Produkte erfasst werden. Für jede Position lassen sich Produkt, Modell und Anzahl separat auswählen. Der Produktumsatz bleibt frei eintragbar.


## Kalender-Erinnerung
Exportierte Kalendertermine enthalten jetzt automatisch eine Erinnerung 1 Tag vor dem Termin (`VALARM`, `TRIGGER:-P1D`).


## Kalender-Download
Im Schnellzugriff gibt es jetzt den Button `Termine fürs Handy`. Er lädt alle Termine der aktuellen Woche als eine `.ics`-Datei herunter. Jeder Termin enthält automatisch eine Erinnerung 1 Tag vorher.


## Neuer Benutzer
Carsten Böhrensen wurde als eigener Benutzer ergänzt. Passwort: `Test`.

## KI-Chat
Der Produkt-Chat wurde repariert und läuft jetzt direkt in der GitHub-Pages-Version auf Basis des eingebetteten Produktkatalogs. Dafür ist kein API-Schlüssel erforderlich.

## RM Dashboard
Swen Liebig war als RM (Regional Manager) ergänzt und wurde wieder entfernt. Ohne hinterlegten RM-Benutzer bleibt das RM-Dashboard aktuell für niemanden erreichbar.

## Team-Kommunikation
Nachrichten und geteilte Termine sind als lokale Demo-Funktion eingebaut.

Wichtig: GitHub Pages ist rein statisch. Damit Nachrichten, geteilte Termine und RM-Daten wirklich zwischen verschiedenen Handys/PCs synchronisiert werden, braucht die produktive Version ein Backend mit zentraler Datenbank und Authentifizierung.

## Funktionsstand
Diese Version repariert den Produkt-KI-Chat, RM-Dashboard, Nachrichten und Termin-Sharing für die lokale GitHub-Pages-Demo.

WICHTIG: GitHub Pages ist statisch. Nachrichten, Mitarbeiterdaten und geteilte Termine funktionieren in dieser ZIP zuverlässig innerhalb desselben Browsers/Geräts. Für echte Synchronisation zwischen unterschiedlichen Handys/PCs braucht OrgaBoard ein Backend mit zentraler Datenbank und Authentifizierung.

## Browser-KI v5
Die KI läuft vollständig im Browser und benötigt keinen API-Schlüssel. Sie durchsucht den lokal eingebetteten Vorwerk-Katalog, kann Modelle vergleichen, Zubehör nennen, anstehende OrgaBoard-Termine abfragen und vollständige Termine per Chat anlegen.

Beispiele:
- `Was kannst du mir über den VK7 sagen?`
- `Vergleiche VK7 und VR7`
- `Welches Zubehör gibt es für den VK7?`
- `Welche Termine stehen als nächstes an?`
- `Termin morgen um 15:00 bei Müller anlegen`

## Nachrichten
Nachrichten und geteilte Termine arbeiten im Browser-Modus über localStorage. Dadurch funktionieren sie zwischen den Benutzerkonten auf demselben Browser/Gerät. Eine geräteübergreifende Synchronisation benötigt später wieder ein Backend.


## Top-Produkte & PDF-Fix
Top-Produkte berücksichtigt jetzt sowohl direkte Verkäufe als auch im Termin erfasste mehrere Produkte. Der frei eingetragene Produktumsatz wird bei mehreren Produkten anteilig nach Stückzahl für die Rangliste verteilt. Im PDF werden Produktumsatz, K70-Umsatz und Gesamtumsatz je Woche sichtbar ausgewiesen.

## KI-Fix v6
Der Terminparser wurde neu aufgebaut. Er versteht jetzt unter anderem:
- `Termin morgen um 15 Uhr bei Müller anlegen`
- `Termin am 12.08. um 10:30 bei Familie Wolf eintragen`
- `Termin Freitag von 14 bis 16 Uhr mit Schmidt erstellen`
- Rückfragen, wenn Datum, Uhrzeit oder Betreff fehlen.

Für VK7, VR7, SP7 und TM7 werden lokale Originalbilder aus offiziellen Vorwerk-Medien verwendet.

## Fix Teddy / Nachrichten / Produkt-KI
- Dustin/Teddy wird als echte lokale PNG-Datei vollständig dargestellt (`object-fit: contain`).
- Nachrichten wurden als einfacher lokaler 1:1-Chat neu aufgebaut. Beim Benutzerwechsel im selben Browser bleiben Nachrichten erhalten und ungelesene Nachrichten werden markiert.
- Die VK7-Antwort zeigt jetzt ein umfangreiches Produktprofil mit Originalbild, Preisstand, Beschreibung, Funktionen, technischen Daten, Laufzeiten und System-Zubehör.


## Bedienungsanleitung
Im linken Menü gibt es jetzt den neuen Punkt `Bedienungsanleitung`. Das integrierte Hilfecenter enthält eine Suche, zwölf Kapitel, Schritt-für-Schritt-Erklärungen, KI-Beispiele sowie Hinweise zu Kalender, PDF, Nachrichten und Benutzerrollen.

## Verbesserungspaket
- Fehler behoben: „Senden“ (Team-Nachrichten), „Termin teilen“ und der Sprung ins RM-Dashboard waren durch einen fehlerhaften `<script>`-Tag komplett inaktiv – funktioniert jetzt.
- Fehler behoben: Der Produkt-KI-Chat (Dock rechts) hat Nachrichten und Antworten teils doppelt angezeigt, weil zwei Klick-Handler gleichzeitig aktiv waren – jetzt nur noch einer.
- **Kernfehler behoben: Die KI war auf allen Bildschirmen unter 1450px Breite (also den meisten Laptops, Tablets und Handys) komplett unsichtbar und ließ sich nicht bedienen.** Über den Button „Produkte KI“ in der Seitenleiste öffnet sie sich dort jetzt als Vollbild-Fenster mit Schließen-Button. Auf größeren Bildschirmen bleibt sie wie gewohnt dauerhaft sichtbar.
- Fehlende `manifest.webmanifest` ergänzt (wurde referenziert, war aber nicht enthalten – nötig für App-Icon/PWA-Installation).
- Ladezeit verbessert: externe Skripte (PDF/Screenshot) blockieren den ersten Seitenaufbau nicht mehr.
- Barrierefreiheit: Tastaturbedienung für Termine/Tage, sichtbarer Fokusrahmen, `aria-label` für alle reinen Icon-Buttons, fehlendes Bild-Alt ergänzt.
- Toter Code entfernt (alte, nicht mehr erreichbare Nachrichten-Funktion), Meta-Beschreibung und Theme-Angaben ergänzt.

