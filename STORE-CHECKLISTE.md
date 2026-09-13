# Wochenplan – bereit für den Store

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | die App im neuen Stil |
| `manifest.json` | Name, Farben, Icons – ersetzt die alte Fassung |
| `datenschutz.html` | Datenschutzerklärung für beide Stores |
| `capacitor.config.json` | für die spätere native Verpackung |
| `icons/` | bereits vorhanden, bleibt unverändert |

Adresse der Datenschutzerklärung fürs Store-Formular:
`https://ivangumy-dev.github.io/Wochenplan-Dashbord/datenschutz.html`

---

## Was sich am Aussehen geändert hat

- Farben, Schrift, Karten und Knöpfe gleich wie bei RidePilot (gemeinsames UI-Kit)
- Reiter als runde Pillen, oben angeheftet und seitlich scrollbar statt gedrängt
- Heutiger Tag türkis hervorgehoben, „Heute"-Marke deutlich sichtbar
- Erledigt-Knöpfe rund, 44 px gross – auf dem iPhone sicher treffbar
- Erledigt-Zustand grün statt nur ein Häkchen
- Dunkelmodus folgt automatisch dem System
- Meldungsband oben statt springendem Text
- Vorlagen als Kacheln, ab Tablet dreispaltig

Funktionen, Daten und Sicherungen bleiben unverändert – nur die Optik wurde ersetzt.

---

## Store-Texte

**Name:** Wochenplan – Alltag & Verein
**Untertitel:** Deine Woche von Montag bis Sonntag
**Kategorie:** Produktivität
**Preis:** CHF 2.00 (oder gratis, falls als Begleit-App gedacht)
**Bundle-ID:** ch.ivangumy.wochenplan

**Beschreibung:**

> Der Wochenplan zeigt deine ganze Woche auf einen Blick – Montag bis Sonntag, 7 bis 23 Uhr.
>
> Zwei Bereiche: privater Alltag und Vereinsaufgaben, sauber getrennt und trotzdem in einer Ansicht.
>
> Heute: was heute ansteht, in einer Liste, direkt abhakbar.
>
> Vorlagen: wiederkehrende Aufgaben mit einem Tipp einsetzen statt jedes Mal tippen.
>
> Wochen-Setup: drei Prioritäten, Fixtermine und eine Notiz für die Woche.
>
> Sicherung: alles als Datei exportieren und wiederherstellen.
>
> Alle Daten bleiben auf deinem Gerät. Kein Konto, keine Anmeldung, keine Werbung.

**Stichwörter:** Wochenplan, Planer, Aufgaben, Woche, Haushalt, Verein, Schweiz

---

## Was du selbst machen musst

1. Dateien ins Repo `Wochenplan-Dashbord` laden (`index.html` und `manifest.json` ersetzen, die anderen neu)
2. Screenshots: Heute, Meine Woche, Wohnzimmer, Vorlagen, Wochen-Setup
3. Verpacken mit Capacitor (Mac oder iPad nötig für iOS):
   ```
   npm install @capacitor/cli @capacitor/core
   npx cap init
   npx cap add ios
   npx cap add android
   npx cap sync
   ```
4. Im Apple-Formular angeben: App sammelt keine Daten. Altersfreigabe 4+.
