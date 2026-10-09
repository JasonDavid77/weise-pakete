# Wissenspakete für den Weisen

Öffentlicher Katalog für Wissenspakete zum Plugin [Der Weise](https://github.com/JasonDavid77/der-weise) (ab Version 4.1.0).

Ein Wissenspaket ist fertiges Lernmaterial zu einem Thema, als Text. Es ist ein eigenes kleines Plugin ohne Befehle und enthält nur Daten: keine Lernziele, keinen Lernstand und keine Abfrage-Karten. Mit `/weise:paket` legt der Weise daraus auf Ihrem Rechner ein Lernthema an. Ihr Lernziel legen Sie dabei selbst fest.

## Pakete

| Paket | Inhalt | Stand |
|---|---|---|
| `weise-agentische-kanzlei` | Agentische Kanzlei: acht Rechercheberichte zu agentischer KI in der Rechtsberatung, Zuschnitt agentische Rechtsabteilung als Produkt (Deutsch) | 2026-10-01 |

## Installieren

In der Claude-Desktop-App: Profil unten links > Einstellungen > unter „Anweisungen“ auf „Plugins“ > Repo `JasonDavid77/weise-pakete` angeben > beim Paket auf das Plus. Mit Befehlen:

```
/plugin marketplace add https://github.com/JasonDavid77/weise-pakete.git
/plugin install <paket>@weise-pakete
```

Danach eine neue Sitzung und `/weise:paket`.

## Ein Paket bauen

Das Format steht in der Anleitung des Weisen: [docs/wissenspaket.md](https://github.com/JasonDavid77/der-weise/blob/main/docs/wissenspaket.md). Wichtig: Das Repo braucht eine Datei `.gitattributes` mit `* -text`, sonst stimmen unter Windows die Prüfsummen nicht.

## Lizenz

MIT für diesen Katalog. Jedes Paket nennt die Herkunft und die Nutzungsbedingungen seines Materials selbst.
