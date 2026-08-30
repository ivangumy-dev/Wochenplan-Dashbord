# Ivan · Wochenplan — Web App

## Dateien
- `index.html` — die App selbst
- `manifest.json` — macht sie installierbar (Name, Icon, Farben)
- `sw.js` — Service Worker für Offline-Nutzung
- `icons/` — App-Icons in allen benötigten Grössen

## Lokal öffnen
`index.html` funktioniert sofort per Doppelklick — Wochenplan, Speicherung, Export/Import
laufen dabei ganz normal. Nur "Zum Home-Bildschirm hinzufügen" und die Offline-Funktion
greifen erst, wenn die Dateien auf einem echten Webserver (mit https) liegen — das ist eine
technische Vorgabe der Browser, keine Einschränkung dieser App.

## Hosting
Alle vier Dateien (inkl. `icons/`-Ordner) zusammen an einen beliebigen Ort hochladen, z.B.
kostenlos über GitHub Pages — genau wie bei RidePilot. Sag Bescheid, wenn ich das für dich
einrichten soll.

## Daten
Alles bleibt lokal im Browser des jeweiligen Geräts (kein Server, kein Konto). Auf einem
zweiten Gerät installiert, startet die App dort mit eigenem, leerem Stand — Abgleich nur
über "Backup exportieren" (Daten-Tab) und auf dem anderen Gerät importieren.
