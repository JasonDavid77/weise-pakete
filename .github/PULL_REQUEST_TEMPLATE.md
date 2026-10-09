<!-- Vorlage für ein neues oder aktualisiertes Wissenspaket. Bitte jede Zeile abhaken oder kurz begründen. -->

## Paket

- Name: `weise-<thema>`
- Version und Stand des Materials:
- Worum es geht (ein Satz):

## Prüfliste

- [ ] **Format 1:** Der Ordner `plugins/<paket>/` hat `.claude-plugin/plugin.json`, `weise-paket.json`, `sources/` mit `sources/readme.md` und eine `README.md` ([Anleitung](https://github.com/JasonDavid77/der-weise/blob/main/docs/wissenspaket.md)).
- [ ] **Nur Daten:** keine Skills, Befehle, Agenten, Hooks, Skripte, kein Server; in `sources/` nur `.md` und `.txt`.
- [ ] **Prüfsummen:** Jede Datei in `sources/` steht mit ihrer SHA-256 im Manifest, `anzahl` stimmt. Geprüft habe ich mit:
- [ ] **Katalog:** Eintrag in `.claude-plugin/marketplace.json` mit `"category": "weise-paket"` und relativer Quelle `./plugins/<paket>`; eine Zeile in der Paketliste der README.
- [ ] **Herkunft:** `quelle` im Manifest sagt, woher das Material stammt und wie es entstanden ist (auch: mit KI recherchiert, ja oder nein).
- [ ] **Lizenz:** Ich darf das Material veröffentlichen. Die Lizenz steht in der Paket-README, in `hinweis` und als `license` in `plugin.json`. Fremde Texte sind nur verlinkt oder kurz zitiert.
- [ ] **Nichts Vertrauliches:** keine Mandats-, Kunden- oder Personendaten, keine internen Unterlagen, Zahlen oder Namen eines Arbeitgebers oder Auftraggebers, keine Zugangsdaten, keine lokalen Pfade.
- [ ] **Nutzungsneutral:** kein Lernziel, kein Lernstand, keine Abfrage-Karten, kein Bezug auf ein einzelnes Projekt.
- [ ] **Volatilität:** `volatilitaet` und `stand` sind gesetzt; der Weise warnt, wenn die Frist abgelaufen ist.

## Hinweise für die Prüfung

<!-- Was sollte man wissen? Zum Beispiel: Welche Teile sind Einschätzung, welche belegt? -->
