# Haushaltsbuch

Web-App für iPhone und iPad, mit der ihr Einnahmen und Ausgaben aufschreibt. Sie funktioniert ohne Anmeldung und auch offline.

## Funktionen

- **Buchungen:** Ausgabe oder Einnahme, Betrag, Datum, Kategorie, Beschreibung und Person („bezahlt von / für“).
- **Monatsbilanz:** Einnahmen, Ausgaben und was übrig bleibt, Monat für Monat.
- **Ausgaben nach Kategorie** mit Anteil in Prozent.
- **Sicherung:** speichert alle Buchungen als JSON-Datei über das Teilen-Menü (Dateien, AirDrop, Mail).
- **Sicherung laden:** führt eine Sicherung mit den vorhandenen Buchungen zusammen, ohne Doppelte. So lassen sich die Einträge von zwei Geräten zusammenlegen.
- **CSV-Export** des angezeigten Monats, zum Beispiel für Excel oder Numbers.

## Daten

Alle Daten liegen **nur auf dem Gerät**, im Speicher von Safari für diese App. Mach regelmäßig eine Sicherung und leg sie in „Dateien“ → iCloud Drive ab. Die App erinnert dich daran, wenn die letzte Sicherung länger als 30 Tage her ist.

## Auf das iPhone bringen

1. In GitHub: **Settings → Pages → Source: „GitHub Actions“** einstellen.
2. Unter **Actions → „Haushaltsbuch veröffentlichen“ → Run workflow** den Workflow starten.
3. Die angezeigte Adresse auf dem iPhone in **Safari** öffnen.
4. **Teilen → „Zum Home-Bildschirm“** wählen.

## Entwicklung

Die App liegt in `www/`. Sie besteht aus reinem HTML, CSS und JavaScript und braucht keinen Build-Schritt. Zum Testen startest du einen lokalen Server: `python3 -m http.server -d www`.
