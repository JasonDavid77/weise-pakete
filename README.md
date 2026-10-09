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

## Ein Paket einreichen

Sie haben Lernmaterial, das anderen hilft? So kommt es in diesen Katalog:

1. Legen Sie auf GitHub eine eigene Kopie dieses Repos an (Schaltfläche „Fork“).
2. Bauen Sie Ihr Paket dort in einem Zweig `paket/<name>` unter `plugins/<name>/`, tragen Sie es in `.claude-plugin/marketplace.json` ein (mit `"category": "weise-paket"`) und ergänzen Sie die Paketliste oben.
3. Stellen Sie einen Pull Request. Die Vorlage fragt eine kurze Prüfliste ab: Format, Prüfsummen, nur Daten, Herkunft, Lizenz, nichts Vertrauliches.
4. Der Betreiber prüft jede Einreichung: Prüfsummen, Aufbau, Herkunft und Lizenz, und ob etwas Vertrauliches oder ein Bezug zu einem Arbeitgeber oder Auftraggeber zu erkennen ist. Danach übernimmt er das Paket, bittet um Änderungen oder lehnt ab. Ein Anspruch auf Aufnahme besteht nicht.

Was nicht hierher gehört: Material, das Sie nicht veröffentlichen dürfen (etwa Texte hinter einer Bezahlschranke oder aus einem lizenzierten Produkt), und alles Vertrauliche. Mit Ihrem Pull Request stellen Sie Ihr Material unter die Lizenz, die Sie im Paket nennen.

## Lizenz

MIT für diesen Katalog. Jedes Paket nennt die Herkunft und die Nutzungsbedingungen seines Materials selbst.
