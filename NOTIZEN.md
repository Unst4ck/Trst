# NOTIZEN – Meine Einkaufsliste

## Was ist das?
Eine einfache Einkaufslisten-App für mich selbst, zuerst für das iPhone.
Die Daten werden nur auf dem Gerät gespeichert (im Browser-Speicher „localStorage“).
Nach dem ersten Öffnen funktioniert die App auch ohne Internet.

## Technik
- `index.html`: die ganze App (HTML + CSS + JavaScript)
- `manifest.json`: Name und Symbol für den Home-Bildschirm
- `sw.js`: „Service Worker“, legt die App auf dem Gerät ab, damit sie offline startet
- `icons/`: das App-Symbol in verschiedenen Größen
- Kein Server, keine Anmeldung, keine Kosten. Die Seite liegt kostenlos bei GitHub Pages.

## Was wir gemacht haben
- [x] Teil 1: Titel „Meine Einkaufsliste“, Eingabefeld, Knopf „Hinzufügen“, Liste der Artikel
- [x] Teil 2: Artikel als erledigt markieren (durchgestrichen) und löschen
- [x] Teil 3: Liste automatisch speichern und beim Öffnen wieder anzeigen
- [x] Teil 4a: Offline-Funktion und App-Symbol eingebaut
- [ ] Teil 4b: GitHub Pages einschalten und App auf den iPhone-Home-Bildschirm legen

## Was noch fehlt / Ideen für später
- Mehrere Listen (z. B. Supermarkt, Drogerie)
- Verbindung zum PC (Liste auf mehreren Geräten sehen)
- Später eine „richtige“ iPhone-App

## Wie man das Projekt öffnet
- **Auf dem iPhone (dauerhaft):** https://unst4ck.github.io/Trst/ in Safari öffnen,
  dann „Teilen“ → „Zum Home-Bildschirm“. Ab dann immer über das Symbol öffnen
  (Safari und das Symbol haben getrennte Speicher).
- **Vorschau in Claude:** https://claude.ai/artifact/Ud3BYnta4Ns4zqqhFtzzh6
  (nur zum Ausprobieren, Speichern dort nicht zuverlässig)
- **Am Computer:** Die Datei `index.html` herunterladen und doppelt anklicken.

## Wichtig für Änderungen (für Claude / Entwickler)
- Nach jeder Änderung an `index.html` oder anderen Dateien in `sw.js` die
  Versionsnummer `CACHE` erhöhen, sonst sieht das iPhone die neue Version erst beim übernächsten Öffnen.
