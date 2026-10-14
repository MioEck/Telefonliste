# Riesebyer Telefonliste

Web-App (PWA) im blauen Milchglas-Design für die Telefonnummern der Kollegen.

- Liste mit Suche, alphabetisch gruppiert
- Name antippen → Details: alle Nummern, E-Mail, Geburtsdatum, Notizen – alles editierbar
- Nummer / 📞 antippen → Anruf startet (`tel:`-Link)
- Import der Telefonliste aus Bild (Foto/Scan) oder PDF per Texterkennung (Tesseract.js / pdf.js, läuft im Browser), mit Prüf-Schritt vor der Übernahme
- Daten werden lokal im Browser gespeichert; Sicherung als JSON exportier-/ladbar

Start: `index.html` über einen Webserver öffnen (z. B. GitHub Pages) und auf dem Handy „Zum Startbildschirm hinzufügen“.

## Updates

Bei jeder Änderung `APP_VERSION` in `index.html` und `version.json` auf denselben neuen Wert setzen.
Die App prüft beim Öffnen, beim Zurückkehren und alle 5 Minuten und lädt sich dann selbst neu
(nicht während ein Bearbeiten-/Import-Fenster offen ist). Die gespeicherten Daten bleiben erhalten.
