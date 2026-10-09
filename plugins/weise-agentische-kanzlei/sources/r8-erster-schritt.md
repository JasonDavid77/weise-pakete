# Testbetrieb mit KI-Agenten und Mandatsdaten: Was eine deutsche Wirtschaftskanzlei braucht (Stand Oktober 2026)

Für den ersten Testbetrieb braucht die Kanzlei vor allem eine saubere Vertragskette nach § 43e BRAO und ein aufgeräumtes Microsoft-365-Berechtigungsmodell, nicht unbedingt eigene GPU-Server. Die Wahl des Modells ist zweitrangig. Empfohlen wird ein eng abgegrenzter Pilot über drei bis sechs Monate mit 15–40 Berufsträgern auf einer EU-gehosteten Plattform, entweder einem spezialisierten Kanzleianbieter oder einem Unternehmensangebot. Datenschutz-Folgenabschätzung, Schulung und messbare Ziele müssen vor dem Start stehen.

## TL;DR

- **Weg und Kosten:** Die Kanzlei kann zwischen drei Wegen wählen, alle zulässig. Ein Unternehmensangebot wie Microsoft 365 Copilot kostet laut Microsoft-Preisangaben 18,20–26,00 € pro Nutzer und Monat. Spezialisierte Kanzleianbieter liegen zwischen rund 300 € und 2.000 US-$ pro Platz und Monat, wobei nur der Preis von Beck-Noxtua öffentlich ist. Eigener Betrieb und private Cloud bedeuten einmalig etwa 20.000–55.000 € oder 500–3.000 € pro Monat. Für einen ersten Test mit Mandatsdaten empfehlen wir einen EU-gehosteten Fachanbieter oder einen strikt konfigurierten M365-Tenant. Eigene Server lohnen sich erst später.
- **Pflichten vor dem Start:** Den Rahmen setzen Berufsrecht und Datenschutz.
  - § 43e BRAO verlangt eine eigene Verschwiegenheitsverpflichtung in Textform mit Belehrung über die strafrechtlichen Folgen. Der Auftragsverarbeitungsvertrag (AVV) ersetzt sie nicht. Bei Verarbeitung im Ausland ist ein vergleichbarer Geheimnisschutz nötig.
  - Hinzu kommen eine Datenschutz-Folgenabschätzung, die KI-Kompetenzpflicht nach Art. 4 KI-Verordnung (seit 2. Februar 2025, seit 27. Juli 2026 durch die Verordnung (EU) 2026/1744 zu einer Unterstützungspflicht abgeschwächt) und in M365 aktiv gesetzte Grenzen: Flex Routing ausschalten, Anthropic-Modelle in EU-Tenants deaktiviert lassen.
- **Typische Fehler:** Die häufigsten Fehler sind ungeprüfte KI-Ausgaben, Oversharing in SharePoint und Pilotprojekte ohne messbare Ziele.
  - Ungeprüfte Ausgaben: AG Köln (2. Juli 2025) und LG Frankfurt (25. September 2025) rügten Anwälte für erfundene Fundstellen.
  - Projekte ohne Ziele: Gartner prognostizierte im Juni 2025, dass über 40 % der Agentic-AI-Projekte bis Ende 2027 eingestellt werden.

## 1. Befunde

### 1.1 Wege zu einer KI, die mit Mandatsdaten arbeiten darf

| Weg | Vorteile | Nachteile | Kosten (Größenordnung) | Belegqualität |
|---|---|---|---|---|
| **Eigener Betrieb (On-Premise)** mit offenen Modellen (Llama, Mistral, Qwen) | Daten verlassen die Kanzlei nicht.\[1\] Kein Dienstleister im Sinne von § 43e BRAO für die Modellverarbeitung, keine Auslandsfrage | Modelle laut Anbieter schwächer als kommerzielle Spitzenmodelle.\[2\] Eigene Wartung, eigenes Sicherheitsteam, Agentenfunktionen müssen selbst gebaut werden | Server der A100-Klasse 20.000–35.000 €, laufend ca. 950–2.550 €/Monat (tomczak.dev, 2026); Gesamtkosten über 36 Monate ca. 55.000 € (hostspezial.de, Anbieterangabe)\[3\]\[4\] | Nur Anbieter- und Beraterseiten, keine unabhängige Kostenstudie gefunden |
| **Private Cloud** (GPU-Instanzen bei IONOS, Hetzner, OVHcloud, T Cloud) | EU-Anbieter ohne US-Mutter, AVV möglich, kein eigenes Hardware-Management\[4\] | Integration und Betrieb liegen weiter bei der Kanzlei oder einem Dienstleister. Auch hier ist eine Verpflichtung nach § 43e BRAO nötig | 1,50–4 €/Stunde für A100-Klasse (tomczak.dev); 500–3.000 €/Monat (software-entwickeln-lassen.com)\[4\]\[5\] | Beraterangaben |
| **Unternehmensangebote großer Anbieter** (Microsoft 365 Copilot, ChatGPT Enterprise, API über Azure/EU) | Tiefe Integration in die vorhandene M365-Umgebung, vertragliche Zusagen (EU Data Boundary, kein Training mit Kundendaten), schnell startbar | US-Mutterkonzern und damit CLOUD Act.\[1\] Standardeinstellungen ändern sich, z. B. Flex Routing seit April 2026.\[6\] Für juristische Arbeit nicht spezialisiert | Microsoft 365 Copilot 26,00 €, Copilot Business 18,20 € pro Nutzer und Monat zusätzlich zur M365-Lizenz (Microsoft-Preisangabe laut it-p.de und ki-syndikat.de, abgerufen September 2026)\[7\] | Preis: Herstellerangabe, gut belegt |
| **Spezialisierte Kanzleianbieter** (Harvey, Legora, Beck-Noxtua, Libra u. a.) | Juristische Workflows, Agenten, Tabellen-Review. Beck-Noxtua mit beck-online-Inhalten und deutschem Hosting (IONOS/Open Telekom Cloud, laut Vergleichsportal).\[8\]\[9\] Erfahrung mit Kanzlei-Compliance | Mindestabnahmen und Jahresverträge. Bei Harvey und Legora keine öffentlichen Preise.\[10\] Zusätzliche Vertragskette über Modellanbieter (OpenAI, Anthropic) | Beck-Noxtua: PLUS 299 €, PREMIUM 499 € je Lizenz und Monat (laut lulius.ai mit Verweis auf beck-noxtua.de, 7. September 2026); früher 1.050 €/Monat für drei Lizenzen (Podcast RBA427).\[11\]\[12\] Harvey: geschätzt 1.200–2.000 US-$/Platz/Monat bei 20–50 Plätzen Minimum. Legora: geschätzt 3.000 US-$/Nutzer/Jahr bei 10 Plätzen oder 300–800 US-$/Monat (widersprüchliche Schätzungen Dritter)\[8\]\[13\]\[14\] | Harvey- und Legora-Preise sind **unbestätigte Schätzungen** von Wettbewerbern (lulius.ai, juriscout.com, vaquill.ai). Juriscout kennzeichnet sie selbst als „UNVERIFIED“\[15\] |

**Einschätzung:** Für eine Wirtschaftskanzlei mit M365 sind zwei Wege für den ersten Test am sinnvollsten.

- **Variante A:** ein spezialisierter Kanzleianbieter mit EU-Hosting. Er liefert die meisten Agenten- und Workflow-Funktionen.
- **Variante B:** Microsoft 365 Copilot in einem strikt konfigurierten Tenant. Er bietet die geringste Integrationsreibung, aber weniger juristische Tiefe.

Eigener Betrieb lohnt sich für einen ersten Test kaum. Die Hardware ist billig, teuer sind Integration, Absicherung und Agentenlogik. Die Amortisationsrechnungen der Anbieter („Break-Even nach 18 Monaten“) sind Marketingangaben.\[3\]

Zum deutschen Markt gibt es belegte Datenpunkte, die den Unterschied zum internationalen Markt zeigen:

- Gleiss Lutz schloss laut eigener Pressemitteilung vom 6. März 2024 als erste unabhängige deutsche Wirtschaftskanzlei eine strategische Partnerschaft mit Harvey, „nach einem Pilot mit über 125 Juristinnen und Juristen“.\[16\]\[17\]\[18\]
- Laut Harvey (Anbieterangabe, undatiert) haben inzwischen mehr als 350 Anwälte bei Gleiss Lutz Harvey integriert.\[19\]
- Laut beck-aktuell (24. September 2026) nennt Harvey nach eigenen Angaben über 3.000 Kunden in mehr als 70 Ländern, darunter Gleiss Lutz und Heuking.\[20\]
- International dominieren Harvey und Legora.\[14\]\[15\]
- Für rein deutschsprachige Recherche bauen deutsche Verlage eigene Lösungen: Beck-Noxtua (C.H. Beck) und die juris KI-Suite.\[14\]\[21\]

### 1.2 Anforderungen aus Berufsrecht, Datenschutz und Informationssicherheit

**Berufsrecht (belegt)**

- **§ 43e BRAO** ist die Erlaubnisnorm (Gesetzeswortlaut, u. a. wiedergegeben bei der Hanseatischen RAK Hamburg):
  - **Abs. 1:** Zugang zu Mandatsgeheimnissen nur, „soweit dies für die Inanspruchnahme der Dienstleistung erforderlich ist“.\[22\]\[23\]
  - **Abs. 2:** sorgfältige Auswahl des Dienstleisters.\[23\]\[24\] Endet, wenn die Vorgaben nicht mehr eingehalten werden.\[25\]\[26\]
  - **Abs. 3:** Vertrag in Textform. Der Dienstleister wird „unter Belehrung über die strafrechtlichen Folgen einer Pflichtverletzung zur Verschwiegenheit“ verpflichtet und darf nur das Erforderliche zur Kenntnis nehmen.\[22\] Für Unterauftragnehmer ist eine Regelung zu treffen.\[23\]\[25\]
  - **Abs. 4:** Bei Dienstleistungen im Ausland ist ein „dem Schutz im Inland vergleichbar[er]“ Geheimnisschutz nötig. Die RAK Hamburg verweist auf die Gesetzesbegründung: Für EU-Mitgliedstaaten könne „in der Regel“ davon ausgegangen werden. Andere Staaten sind im Einzelfall zu prüfen.\[23\]\[24\]
  - **Abs. 5:** Einwilligung des Mandanten bei Dienstleistungen, die unmittelbar einem einzelnen Mandat dienen.\[25\]\[27\]
- **BRAK, „Hinweise zum Einsatz von künstlicher Intelligenz (KI)“** (Dezember 2024, BRAK-Ausschuss RDG, Dr. Frank Remmertz) verlangt:
  - eine eigenverantwortliche Endkontrolle der KI-Ergebnisse,\[28\]
  - das Need-to-know-Prinzip bei Cloud-Diensten,\[29\]
  - Anonymisierung oder Verschlüsselung, wo möglich.\[30\]
  Die Hinweise erheben „keinen Anspruch auf Vollständigkeit“.\[31\] Laut der BRAK-Publikationsseite (abgerufen Oktober 2026) sind sie weiterhin auf dem Stand 12/2024; eine Aktualisierung gibt es nicht.\[32\]
- **DAV, Initiativ-Stellungnahme Nr. 32/2025** (Juli 2025, Forum für Wirtschaftskanzleien):
  - KI- und Cloud-Einsatz ist bei Einhaltung von § 43e BRAO berufsrechtlich zulässig.\[33\]\[34\]
  - Die Stellungnahme hält selbst fest, dass „KI-Anbieter […] die Unterzeichnung entsprechender“ Verpflichtungen scheuen.\[35\]
  - Sie empfiehlt Anbieter mit EU-Infrastruktur und den Ausschluss der Nutzung zu Trainingszwecken.\[30\]\[36\]
  - Nach Sekundärdarstellungen (visionarydata.de) sieht der DAV in rein maschineller Verarbeitung ohne Kenntnisnahme durch Menschen kein „Offenbaren“ im Sinne von § 203 StGB.\[37\]

**Datenschutz (belegt)**

- Die Datenschutzkonferenz (DSK) hat drei Orientierungshilfen veröffentlicht:
  - „KI und Datenschutz“ (Mai 2024),\[38\]
  - „Empfohlene technische und organisatorische Maßnahmen bei Entwicklung und Betrieb von KI-Systemen“ (Juni 2025),\[39\]
  - „Datenschutzrechtliche Besonderheiten generativer KI-Systeme mit RAG-Methode“ (17. Oktober 2025, 18 Seiten).\[40\]
- Danach braucht es eine Prüfung im Einzelfall und aktuelle technisch-organisatorische Maßnahmen (TOM). In der Praxis heißt das: eine Datenschutz-Folgenabschätzung (DSFA) nach Art. 35 DSGVO über alle Komponenten (Retriever, Vektordatenbank, LLM), so die Auswertung von SKW Schwarz.\[40\]\[41\]
- Für Kanzleien mit Agenten, die Mandatsakten durchsuchen, ist eine DSFA nach unserer Einschätzung praktisch immer geboten.
- Der AVV nach Art. 28 DSGVO ist notwendig, deckt aber nicht § 43e BRAO und § 203 StGB ab. Beides sind getrennte Ebenen.\[25\]\[27\]\[42\]

**Datenstandort und CLOUD Act (belegt, mit Gegenposition)**

- Anton Carniaux, Leiter Corporate, External & Legal Affairs bei Microsoft France, antwortete am 10. Juni 2025 unter Eid vor dem französischen Senat auf die Frage, ob Daten nie ohne französische Zustimmung an US-Behörden gingen: „Nein, das kann ich nicht garantieren“. Das sei aber „noch nie vorgekommen“.\[43\]
- Microsoft meldete im Februar 2025 den Abschluss der EU Data Boundary.\[44\]\[45\]
- Seit dem **17. April 2026** ist für viele EU- und EFTA-Tenants jedoch **Flex Routing standardmäßig aktiv**. Bei Lastspitzen kann die LLM-Inferenz von Copilot dann außerhalb der EU stattfinden.\[46\]\[47\] Admins können das unter „Do not allow flex routing“ abschalten (Office365itpros, 7. April 2026; schneider.im). Laut einem Microsoft-Statement gegenüber Tweakers gilt für große Organisationen eventuell ein Opt-in.\[48\]\[49\]
- Seit dem **7. Januar 2026** ist Anthropic Unterauftragsverarbeiter für Copilot. Diese Modelle sind laut Microsoft-Dokumentation **von der EU Data Boundary ausgenommen**; für EU-, EFTA- und UK-Tenants sind sie standardmäßig aus.\[47\]\[48\]\[50\]
- OpenAI bietet seit Februar 2025 europäische Datenresidenz und seit Januar 2026 Inferenz-Residenz in Europa, beides für berechtigte Enterprise-, Edu- und API-Kunden (Anbieterangabe, openai.com).\[51\]\[52\]

**Verschlüsselung und Protokollierung:** Belastbare, KI-spezifische Pflichtvorgaben für Kanzleien haben wir nicht gefunden. Die Anforderungen folgen aus Art. 32 DSGVO und den DSK-TOM.

**Einschätzung:** Mindestens nötig sind:
- Verschlüsselung bei Übertragung und Speicherung,
- dokumentierte Aufbewahrungs- und Löschfristen für Prompts und Ausgaben,
- Audit-Logs (in M365 über Purview), wer welchen Agenten auf welche Akte angesetzt hat,
- Mandatstrennung, um Interessenkonflikte und Chinese Walls abzubilden.

Ein Hinweis zur Verschlüsselung (vsx.is): Der CLOUD Act kann einen Anbieter nicht zwingen, Daten zu entschlüsseln, für die er keine Schlüssel hat.\[53\] Kundenseitig verwaltete Schlüssel sind deshalb das stärkste technische Gegenmittel.

**Weitere Pflichten:**

- **Art. 4 KI-Verordnung:** gilt seit 2. Februar 2025, auch im Pilot. Die Verordnung (EU) 2026/1744 (Digital Omnibus) vom 8. Juli 2026, gültig seit 27. Juli 2026, hat die Pflicht abgeschwächt. Die alte Fassung „nach besten Kräften sicherzustellen“ gilt nicht mehr. Nach dem neuen Wortlaut (Textwiedergabe bei buzer.de) müssen Anbieter und Betreiber nur noch Maßnahmen ergreifen, „um die Entwicklung der KI-Kompetenz ihres Personals … zu unterstützen“. Laut regulatoryblog.eu verlangt die Pflicht damit „kein bestimmtes Kompetenzniveau“.
- **Mitbestimmung:** Wo ein Betriebsrat besteht, gilt § 87 Abs. 1 Nr. 6 BetrVG.
  - Das BAG entschied am 8. März 2022 (1 ABR 20/21), Office 365 sei eine „technische Einrichtung“ in diesem Sinn.\[54\]
  - Das ArbG Hamburg (16. Januar 2024, 24 BVGa 1/24) verneinte die Mitbestimmung nur, weil ChatGPT über private Accounts im Browser genutzt wurde. Das lässt sich nicht auf von der Kanzlei bereitgestellte Lizenzen übertragen.\[55\]\[56\]
  - Eine Gerichtsentscheidung speziell zu Copilot oder Legal-KI gibt es nach unserer Recherche nicht.\[56\]

### 1.3 Einbindung in eine zentral verwaltete M365-Kanzlei-IT

**Belegt:**

- **Copilot erbt die Berechtigungen:** Copilot sieht alles, worauf der Nutzer in SharePoint, OneDrive, Teams und Exchange zugreifen darf. Über Jahre gewachsene, zu weit gefasste Freigaben („Oversharing“) werden dadurch sichtbar.\[57\]\[58\] Microsoft stellt dafür Werkzeuge bereit:
  - SharePoint Advanced Management, verfügbar ab der ersten Copilot-Lizenz im Tenant,\[59\]\[60\]
  - Restricted Content Discovery (Seiten aus der Copilot-Suche nehmen, ohne Rechte zu ändern),\[61\]
  - Purview-Sensitivitätslabels.\[62\]
- **Studienlage:** Der CoreView-Report „State of Microsoft 365 Security and Governance 2026“ (21. Juli 2026) beruht laut coreview.com auf einer Umfrage unter 279 IT- und Sicherheitsverantwortlichen. Ergebnis: „66% of organizations delayed or cancelled a Copilot rollout due to concerns about the data it could surface via SharePoint.“ CoreView verkauft selbst Governance-Werkzeuge für M365.
- **Prompt-Injection:** EchoLeak (CVE-2025-32711, CVSS 9.3) war eine Zero-Click-Lücke in Microsoft 365 Copilot. Eine präparierte E-Mail genügte, um interne Daten abfließen zu lassen.\[63\]\[64\]
  - Entdeckt hat sie Aim Security; die Fallstudie ist auf arXiv (2509.10540) veröffentlicht.\[64\]\[65\]
  - Microsoft behob die Lücke im Mai 2025 serverseitig. Ausnutzung in freier Wildbahn ist nicht bekannt.\[63\]\[66\]
  - Für Agenten, die E-Mails und Fremddokumente lesen, ist das das zentrale Sicherheitsthema.

**Einschätzung, Integrationsmuster für den Test:**

- **Identität:** Ausschließlich Entra-ID-Konten (Single Sign-on, MFA), eine eigene Sicherheitsgruppe für Pilotteilnehmer, bedingter Zugriff nur von verwalteten Geräten.
- **Datenraum:** Agenten arbeiten nur auf einem abgegrenzten Pilot-Datenraum, z. B. eigenen SharePoint-Seiten oder einem eigenen DMS-Workspace mit ausgewählten Mandaten und Mandanteneinwilligung. Kein Zugriff auf den Gesamtbestand.
- **Tenant-Einstellungen vor Start:**
  - Flex Routing aus,\[67\]
  - Anthropic-Unterauftragsverarbeiter aus (sofern nicht gesondert nach § 43e Abs. 4 BRAO geprüft),\[67\]
  - Web-Grounding für mandatsbezogene Arbeit prüfen,
  - Purview-Audit und DLP-Regeln aktiv.
- **Fachanbieter:** Anbindung über Entra-SSO und Word- oder Outlook-Add-ins. DMS-Konnektoren (iManage, NetDocuments, SharePoint) nur lesend und nur für den Pilotdatenraum.
- **Schatten-KI:** Private ChatGPT-Konten und Consumer-Dienste im Kanzleinetz sperren oder per Richtlinie verbieten.\[26\] Sonst entsteht parallel eine unkontrollierte Nutzung.

### 1.4 Rollen, Ansprechpartner und Zeitbedarf

**Rollen (Einschätzung, gestützt auf DSK, BRAK und Praxisbeispiele):**

| Rolle | Aufgabe im Pilot |
|---|---|
| Sponsor in der Kanzleileitung (Managing Partner) | Budget, Go/No-Go-Entscheidung, Mandantenkommunikation |
| Fachbereich (2–3 Praxisgruppen, je ein Partner als „Use-Case-Owner“) | Anwendungsfälle, Qualitätsmaßstab, Endkontrolle der Ergebnisse |
| Legal Tech / Innovation | Anbieterauswahl, Prompt- und Workflow-Design, KPI-Messung |
| IT / M365-Administration | Tenant-Einstellungen, Berechtigungsbereinigung, SSO, DMS-Anbindung |
| Informationssicherheit | Bedrohungsmodell (Prompt-Injection), Logging, Anbieterprüfung (ISO 27001, BSI C5) |
| Datenschutzbeauftragter | DSFA, AVV, Verzeichnis der Verarbeitungstätigkeiten |
| Berufsrecht / General Counsel der Kanzlei | Verpflichtung nach § 43e BRAO, Prüfung nach Abs. 4, Mandanteneinwilligung nach Abs. 5, Mandatsbedingungen |
| Betriebsrat (falls vorhanden) | Mitbestimmung nach § 87 Abs. 1 Nr. 6 BetrVG, ggf. Betriebsvereinbarung |
| Schulungsverantwortliche | KI-Kompetenz nach Art. 4 KI-VO |

**Belegte Zeit- und Größenangaben aus Kanzleien:**

- **Gleiss Lutz:** Pilot mit über 125 Juristen vor der Partnerschaft mit Harvey (März 2024).\[17\]\[18\] Dauer und Vorlaufzeit sind nicht veröffentlicht.
- **Bird & Bird:** sechsmonatige Testphase mit 675 Personen aus fast allen Büros vor dem kanzleiweiten Legora-Rollout 2025. Die Zahlen gelten weltweit, nicht nur für Deutschland. CEO Christian Bartsch: getestet „mit einer Reihe von KPIs für ausgewählte Anwendungsfälle“ (Recht & Politik).\[68\]
- **Hengeler Mueller:** Laut Harvey (Anbieterangabe, undatiert) erfolgte der kanzleiweite Rollout „in just six weeks“, aber erst nach einer begrenzten Vorphase. Eine Pflichtschulung mit AI-Governance war das „ticket to a license“.\[69\]
- **Vorlaufzeit vor dem Pilot:** Für keine DACH-Kanzlei haben wir eine öffentliche Angabe gefunden (etwa für DSFA, Vertrag oder Betriebsvereinbarung).

**Einschätzung Zeitbedarf bis zum Start:** realistisch **8–16 Wochen**, davon:
- 3–6 Wochen Anbieterauswahl und Vertragsverhandlung (§ 43e-Anlage, AVV, Unterauftragnehmerliste),
- parallel 4–8 Wochen DSFA, Tenant-Härtung und Berechtigungsbereinigung des Pilotdatenraums,
- 1–2 Wochen Schulung.

Der Test selbst sollte nach den Beispielen 3–6 Monate dauern. Engpass ist erfahrungsgemäß die Vertragsverhandlung, weil KI-Anbieter laut DAV ungern Verpflichtungen nach § 43e unterschreiben, und bei M365 die Bereinigung der Berechtigungen.\[35\]

### 1.5 Typische Fehler beim ersten Schritt

1. **Ungeprüfte Ausgaben in Schriftsätzen.**
   - Das AG Köln (2. Juli 2025, 312 F 130/25) stellte fest, Fundstellen in einem Schriftsatz seien „offenbar mittels künstlicher Intelligenz generiert und frei erfunden“, und verwies auf § 43a Abs. 3 BRAO.\[70\]\[71\]\[72\]\[73\]
   - Das LG Frankfurt am Main (25. September 2025, 2-13 S 56/24) rügte frei erfundene BGH-Zitate.\[71\]
   - Beide Fälle betreffen generische KI ohne Anbindung an Datenbanken.\[74\]
2. **AVV gilt als ausreichend.** Ohne eigene Verschwiegenheitsverpflichtung nach § 43e BRAO mit Strafbelehrung und ohne Unterauftragnehmerkette ist die berufsrechtliche Seite nicht erfüllt.\[25\]\[26\]\[27\]
3. **Standardeinstellungen werden übernommen.** Flex Routing und Modell-Unterauftragsverarbeiter werden nicht geprüft. Microsoft hat 2026 mehrfach Standardwerte geändert.\[6\]\[50\]
4. **Copilot im unbereinigten Tenant.** Oversharing wird erst im Pilot sichtbar, etwa wenn Mandats- oder Personalakten in Antworten auftauchen.\[57\]\[75\] Dann wird aus dem KI-Projekt ein Projekt zur Bereinigung der Berechtigungen.\[76\]
5. **„Agent Washing“ und Pilot ohne Ziel.** Gartner (25. Juni 2025) prognostiziert, dass über 40 % der Agentic-AI-Projekte bis Ende 2027 wegen Kosten, unklarem Nutzen oder unzureichender Risikokontrollen eingestellt werden. Nur etwa 130 von tausenden Anbietern böten echte Agentenfunktionen.\[77\]\[78\]
6. **Zu breiter Zugriff für Agenten.** Wenn Agenten E-Mails und Fremddokumente lesen und zugleich handeln dürfen, vergrößert sich die Angriffsfläche durch Prompt-Injection (EchoLeak).\[66\]\[79\]
7. **Schulung als Formalie.** Art. 4 KI-VO verlangt KI-Kompetenz. Hengeler Mueller koppelt die Lizenz an eine Pflichtschulung (Anbieterangabe von Harvey).\[69\]

## 2. Gegenbelege und offene Punkte

- **Ist der Weg über US-Anbieter überhaupt zulässig?** Hier stehen sich zwei Lager gegenüber.
  - Anbieter lokaler LLMs (z. B. koreva.de, wz-it.com) halten Cloud-KI mit US-Bezug wegen CLOUD Act für kaum vereinbar mit der Verschwiegenheit.\[1\] Das sind Anbieterangaben mit Eigeninteresse.\[27\]
  - Gegenposition: Der DAV hält den Einsatz bei Einhaltung von § 43e BRAO für zulässig.\[33\] Microsoft verweist darauf, dass eine Herausgabe noch nie vorgekommen sei. Gleiss Lutz und Hengeler Mueller setzen Harvey ein, ein US-Anbieter.\[20\]\[43\]\[80\]\[81\]
  - **Offen:** Ob der US-Geheimnisschutz „vergleichbar“ im Sinne von § 43e Abs. 4 BRAO ist, ist nicht gerichtlich geklärt. Die Kanzlei muss das selbst bewerten und dokumentieren.\[24\]\[82\]
- **Datenschutzaufsicht zu Copilot:** Der Hessische Datenschutzbeauftragte (HBDI) stellte am 14. November 2025 per Pressemitteilung fest: „Microsoft 365 kann datenschutzkonform genutzt werden“. Grundlage ist ein 137-seitiger Bericht von Prof. Dr. Alexander Roßnagel. Der Bericht betrifft Microsoft 365 allgemein. Copilot-spezifische KI-Risiken bewertet er laut aurum-consulting.de „ausdrücklich nicht“. Den Volltext haben wir nicht ausgewertet.
- **Preise:** Die Preise von Harvey und Legora stammen fast ausschließlich von Wettbewerbern (lulius.ai) oder Vergleichsportalen.\[14\] Sie widersprechen sich, bei Legora etwa 3.000 US-$/Jahr gegenüber 300–800 US-$/Monat.\[8\]\[13\] Verbindlich sind nur Angebote.
- **Gartner-Prognose:** Sie beruht laut Gartner auf einer Webinar-Umfrage unter 3.412 Teilnehmern (Januar 2025).\[77\] Es ist eine Prognose, kein Messergebnis.
- **Gescheiterte Kanzleipiloten in DACH:** Öffentlich dokumentierte Abbrüche haben wir nicht gefunden. Das spricht eher für Publikationsverzerrung als für fehlende Fehlschläge.
- **Rechtsprechung zu Agenten:** Es gibt keine Entscheidungen zur Haftung für autonome KI-Agenten in Kanzleien und keine Entscheidung zur Mitbestimmung bei Copilot.
- **BRAK-Hinweise:** Stand Dezember 2024.\[83\] Agenten und neue Funktionen wie Flex Routing sind darin nicht behandelt.

## 3. Empfehlung

1. **Weg wählen:** Pilot mit einem EU-gehosteten Kanzleianbieter (Variante A) oder einem gehärteten M365-Copilot-Tenant (Variante B). Kein Eigenbetrieb im ersten Schritt.
2. **Vertragspaket:** Vertragsunterzeichnung erst, wenn eine § 43e-Anlage mit Strafbelehrung, ein AVV, die vollständige Liste der Unterauftragnehmer (inklusive Modellanbieter), der Ausschluss von Training, Löschfristen und ein dokumentierter Vermerk nach Abs. 4 vorliegen.
3. **Umfang:** 15–40 Nutzer aus zwei bis drei Praxisgruppen, abgegrenzter Datenraum, ausgewählte Mandate mit Einwilligung nach Abs. 5. Drei bis fünf messbare Anwendungsfälle, z. B. Due-Diligence-Tabellen, Vertragsvergleich, Zusammenfassung von Akten.
4. **Kontrolle:** Pflichtschulung vor Lizenzvergabe, Vier-Augen-Prüfung jeder nach außen gehenden Ausgabe, Logging, monatlicher Bericht an die Kanzleileitung.
5. **Budget (Einschätzung):** Lizenzen ca. 5.000–60.000 € für sechs Monate, je nach Weg und Nutzerzahl. Dazu kommen intern 0,5–1 Vollzeitstelle aus IT und Legal Tech sowie externe Beratung für DSFA und Vertrag.
6. **Zeitplan:** Start nach 8–16 Wochen. Entscheidung über den Rollout nach drei bis sechs Monaten anhand vorab festgelegter KPIs.

## 4. Hinweis zu den Quellen

Herausgeber und Datum der verwendeten Quellen sind im Text an der jeweiligen Aussage genannt. Angaben von Anbietern über sich selbst sind als Anbieterangabe gekennzeichnet; Schätzungen und eigene Bewertungen als Einschätzung.

## Quellen

1. [KI für Kanzleien: Lokale LLMs rechtskonform nutzen](https://koreva.de/blog/ki-im-recht)
2. [Lokale KI im Unternehmen 2026: On-Premise-LLMs mit ollama für KMU](https://skill-sprinters.de/blog/tools/lokale-ki-on-premise-ollama-kmu-2026/)
3. [KI On-Premise & LLM Infrastruktur für Unternehmen](https://www.hostspezial.de/loesungen/ki-on-premise.html)
4. [KI On-Premise Kosten: Wann lohnt sich der eigene Server?](https://tomczak.dev/blog/ki-on-premise-kosten-rechner)
5. [Lokale LLM für Unternehmen: DSGVO-konform KI nutzen 2026](https://www.software-entwickeln-lassen.com/ratgeber/lokale-llm-unternehmen-dsgvo)
6. [Microsoft turned on Copilot flex routing by default on April 17. Your data may now leave the EU. — Lobster Pack](https://www.lobsterpack.com/blog/microsoft-copilot-flex-routing-eu-data/)
7. [Microsoft Copilot Kosten 2026: Preise & Lizenzen für Unternehmen](https://www.it-p.de/blog/kosten-copliot/)
8. [Die besten KI-Tools für Anwälte 2026 im Vergleich — Lulius](https://www.lulius.ai/blog/ki-tools-anwaelte-2026)
9. [Harvey AI vs. Noxtua: Legal AI für deutsche Kanzleien? (2026) — Lulius](https://www.lulius.ai/blog/harvey-ai-vs-noxtua)
10. [Legal AI Vergleich 2026 — Anbieter, Preise und Eignung](https://www.lulius.ai/vergleich)
11. [RBA427 Im Test: "Beck-Noxtua" - Beck \~ Risikobasierter Ansatz Podcast](https://www.podcast.de/episode/707313328/rba427-im-test-beck-noxtua-beck)
12. [beck-online Kosten 2026: Module, Preise und Kündigung — Lulius](https://www.lulius.ai/blog/beck-online-kosten)
13. [Harvey AI Pricing: \$1,200-\$2,000/Seat vs Legora & CoCounsel](https://www.vaquill.ai/blog/harvey-legora-cocounsel-pricing-reality)
14. [Legal AI Deutschland 2026: Alle Anbieter im Preisvergleich — Lulius](https://www.lulius.ai/blog/legal-ai-vergleich-deutschland)
15. [Harvey vs. Legora vs. Noxtua vs. Beck-Noxtua 2026: Legal AI für deutsche BigLaw](https://juriscout.com/insights/harvey-vs-legora-vs-noxtua-2026)
16. [Artificial intelligence – Gleiss Lutz establishes strategic partnership with Harvey AI | Gleiss Lutz](https://www.gleisslutz.com/en/mandates-firm-news/artificial-intelligence-gleiss-lutz-establishes-strategic-partnership-harvey-ai)
17. [KI in Kanzleien: Gleiss Lutz schließt Pakt mit Harvey - Extrajournal.Net](https://extrajournal.net/2024/03/11/ki-in-kanzleien-gleiss-lutz-schliesst-pakt-mit-harvey/)
18. [Künstliche Intelligenz](https://www.zri-online.de/aktuell/kuenstliche-intelligenz-gleiss-lutz-begruendet-strategische-partnerschaft-mit-harvey-ai-77668/)
19. [How Gleiss Lutz Uses Harvey Legal AI](https://www.harvey.ai/customers/gleiss-lutz)
20. [Legal Tech: KI-Anbieter Harvey drängt in deutsche Hörsäle](https://www.beck-aktuell.de/ausbildung-und-karriere/studium-referendariat/ki-anbieter-harvey-deutsche-hochschulen-universitaeten-2026-09-24)
21. [Beck-Noxtua Erfahrungen 2026: Tests, Preise, Grenzen — Lulius](https://www.lulius.ai/blog/beck-noxtua-erfahrungen)
22. [KI und Berufsrecht](https://www.jaehne-guenther.de/ki-und-berufsrecht/)
23. [§ 43e BRAO — Inanspruchnahme von Dienstleistungen](https://www.lulius.ai/gesetze/brao/43e)
24. [Hanseatische Rechtsanwaltskammer Hamburg](https://www.rak-hamburg.de/mitglieder/berufsrecht/inanspruchnahmevondienstleistungen/)
25. [Digitales Vertragsmanagement in Kanzleien: was § 43e BRAO verlangt](https://legal-tech-verzeichnis.de/fachartikel/digitales-vertragsmanagement-in-kanzleien-was-paragraph-43e-brao-verlangt/)
26. [43e BRAO KI: Was Anwaltskanzleien 2026 brauchen](https://pexon-consulting.de/blog/43e-brao-ki/)
27. [KI für Anwaltskanzleien - §43e BRAO- & §203-konform](https://wz-it.com/ki/branchen/anwaltskanzlei/)
28. [Künstliche Intelligenz](https://www.iww.de/kp/berufsrecht/kuenstliche-intelligenz-leitfaden-der-brak-zum-einsatz-von-ki-in-der-beratungspraxis-f165486)
29. [Effizienter Einsatz von KI in Anwaltskanzleien - dacuro GmbH](https://www.dacuro.de/neuigkeiten/beitrag/dsgvo-ki-einsatz-in-rechtsanwaltskanzleien)
30. [Darf die KI Anwalt sein? - Anwaltspraxis Magazin](https://anwaltspraxis-magazin.de/kanzleimagazin/darf-die-ki-anwalt-sein/)
31. [Künstliche Intelligenz in Anwaltskanzleien: BRAK veröffentlicht Leitfaden](https://www.brak.de/newsroom/newsletter/nachrichten-aus-berlin/2025/ausgabe-1-2025-v-812025/kuenstliche-intelligenz-in-anwaltskanzleien-brak-veroeffentlicht-leitfaden/)
32. [Handlungshinweise und Leitfäden](https://www.brak.de/publikationen/handlungshinweise/)
33. [KI in der anwaltlichen Praxis: Chancen und rechtliche Rahmenbedingungen](https://dataagenda.de/ki-in-der-anwaltlichen-praxis-chancen-und-rechtliche-rahmenbedingungen/)
34. [DAV: KI-Einsatz mit dem Anwaltsberuf vereinbar](https://pylehound.com/de/news/28-07-2025-DAV-stellungnahme-ki-einsatz/)
35. [Deutscher Anwaltverein Littenstraße 11, 10179 Berlin Tel.: +49 30 726152-0](https://anwaltverein.de/newsroom/sn-32-25-einsatz-von-ki-in-der-anwaltschaft?file=files%2Fmedia%2Fnews%2Freplicator%2Fstellungnahmen%2Fdav-sn-32-25.pdf)
36. [INHALTSVERZEICHNIS AUSGABE 9/2025 D A T E N S C H U T Z 2 Editorial](https://dataagenda.de/wp-content/uploads/2025/09/NewsBox_09_2025_250904_2-1.pdf)
37. [§203 StGB und Cloud-KI: Was Kanzleien wissen müssen](https://visionarydata.de/blog/203-stgb-cloud-ki-steuerberater)
38. [DSK veröffentlicht Orientierungshilfe zur Künstlichen Intelligenz](https://www.kdsa-ost.de/aktuelles/dsk-veroeffentlicht-orientierungshilfe-zur-kuenstlichen-intelligenz.html)
39. [Datenschutzkonferenz](https://www.datenschutzkonferenz-online.de/orientierungshilfen.html)
40. [PRESSEMITTEILUNG der Konferenz der unabhängigen Datenschutzaufsichtsbehörden](https://www.datenschutzkonferenz-online.de/media/pm/DSK_PM_OH-RAG-Systeme.pdf)
41. [KI-Flash: Neue Orientierungshilfe der DSK zu RAG-basierten KI-Systemen](https://www.skwschwarz.de/news/KI-Flash-Neue-Orientierungshilfe-der-DSK-zu-RAG-basierten-kI-Systemen)
42. [KI und Berufsgeheimnis: § 203 StGB und § 43e BRAO](https://www.agentifizierung.de/softwarekosten-senken/ki-berufsgeheimnistraeger-mandantendaten)
43. [Microsoft kann US-Zugriff auf EU-Cloud nicht verhindern!](https://www.dr-datenschutz.de/microsoft-kann-us-zugriff-auf-eu-cloud-nicht-verhindern/)
44. [Microsofts EU Data Boundary: Fortschritt mit Vorsicht](https://www.dr-datenschutz.de/microsofts-eu-data-boundary-fortschritt-mit-vorsicht/)
45. [Microsofts EU Data Boundary abgeschlossen](https://www.abtis.de/aktuelles/news/microsofts-eu-data-boundary-abgeschlossen)
46. [What Microsoft 365 Copilot flex routing means for EU businesses?](https://www.investglass.com/microsoft-365-copilot-flex-routing/)
47. [Microsoft 365 Copilot, GDPR and EU Data Residency](https://eyalmarcus.com/microsoft-copilot-gdpr-eu-data-residency/)
48. [Flex Routing Dilemma for European Copilot Customers](https://office365itpros.com/2026/04/07/flex-routing-copilot-europe/)
49. [Act now: Microsoft Copilot Data Moves Outside EU - What To Do \[2026-04\]](https://www.schneider.im/microsoft-365-copilot-flex-routing-data-can-move-outside-the-eu/)
50. [Microsoft + Anthropic: the M365 subprocessor change you owe your customers a notice on](https://registora.com/m365-anthropic-subprocessor-change)
51. [CompanyGPT vs. ChatGPT for enterprises: what data residency really covers](https://innfactory.ai/en/services/companygpt/vs-chatgpt/)
52. [openai launches data residency in europe](https://techcrunch.com/2025/02/06/openai-launches-data-residency-in-europe)
53. [CLOUD Act: was er wirklich sagt, was er nicht kann und warum er den europäischen Cloud-Markt umkrempelt - VSX.is](https://vsx.is/de/cloud-act-was-er-wirklich-sagt-was-er-nicht-kann-und-warum-er-den-europaischen-cloud-markt-umkrempelt/)
54. [Bundesarbeitsgericht Beschluss vom 8. März 2022 Erster Senat - 1 ABR 20/21 -](https://www.bundesarbeitsgericht.de/wp-content/uploads/2022/07/1-ABR-20-21.pdf)
55. [Erstes Urteil zu Rechten des Betriebsrats bei Einsatz von künstlicher Intelligenz - Bird & Bird](https://www.twobirds.com/de/insights/2024/germany/erstes-urteil-zu-rechten-des-betriebsrats-bei-einsatz-von-kuenstlicher-intelligenz)
56. [Copilot Betriebsvereinbarung: 6 Streitpunkte 2026](https://aurum-consulting.de/2026/copilot-betriebsvereinbarung)
57. [Copilot Security Check: Oversharing stoppen vor 2026-Rollout](https://pexon-consulting.de/blog/microsoft-365-copilot-security-check/)
58. [Microsoft 365 Copilot Oversharing: Stop It Before You Deploy](https://www.myworkdrive.com/blog/microsoft-365-copilot-oversharing)
59. [Copilot Data Oversharing: Fix Permissions First](https://uprite.com/copilot-data-oversharing/)
60. [Microsoft 365 Copilot Oversharing: How to Find and Fix It](https://accuroai.co/blog/microsoft-copilot-permissions-sprawl-m365-data-leak)
61. [Oversharing in SharePoint: Berechtigungen vor Copilot aufräumen](https://www.boddenberg.de/purview-oversharing-sharepoint/)
62. [Copilot Oversharing? 5 Fixes That Work](https://www.hubsite365.com/en-ww/crm-pages/5-reasons-your-copilot-is-oversharing-and-how-to-fix-it.htm)
63. [EchoLeak (CVE-2025-32711): What the Microsoft Copilot Prompt Injection Vulnerability Means for Your Data](https://sentra.io/blog/copilot-echoleak-prompt-injection)
64. [\[2509.10540\] EchoLeak: The First Real-World Zero-Click Prompt Injection Exploit in a Production LLM System](https://arxiv.org/abs/2509.10540)
65. [Inside CVE-2025-32711 (EchoLeak): Prompt injection meets AI exfiltration](https://www.hackthebox.com/blog/cve-2025-32711-echoleak-copilot-vulnerability)
66. [EchoLeak Vulnerability: What Microsoft's CVE-2025-32711 Revealed About AI Agent Security Gaps](https://www.reco.ai/blog/echoleak-vulnerability)
67. [Flex routing and Copilot - Mindcore Techblog](https://blog.mindcore.dk/2026/04/flex-routing-and-copilot/)
68. [Bird & Bird führt KI-Lösung kanzleiweit Legora ein - Recht & Politik](https://www.rechtundpolitik.com/rechtsmarkt/personal/bird-bird-fuehrt-ki-loesung-kanzleiweit-legora-ein/)
69. [How Hengeler Mueller Uses Harvey Legal AI](https://www.harvey.ai/customers/hengeler-mueller)
70. [AG Köln: Anwalt zitiert KI-Halluzinationen vor Gericht - datenschutzticker.de](https://www.datenschutzticker.de/2025/10/ag-koeln-anwalt-zitiert-ki-halluzinationen-vor-gericht/)
71. [KI in der Anwaltspraxis](https://vonlauffundbolz.de/ki-in-der-anwaltspraxis/)
72. [AG Köln: Berufsrechtliche Bewertung eines KI-generierten Schriftsatzes - Dr. jur. Jens Usebach LL.M │Rechtsanwalt & Fachanwalt │Kündigungsschutz & Arbeitsrecht](https://www.jura.cc/rechtstipps/ag-koeln-berufsrechtliche-bewertung-eines-ki-generierten-schriftsatzes/)
73. [Zwischen Technik und Täuschung: Wenn KI in Schriftsätzen halluziniert - Legal Tech Lab Cologne e.V.](https://legaltechcologne.de/blog/zwischen-technik-und-taeuschung-wenn-ki-in-schriftsaetzen-halluziniert/)
74. [Anwalt blamiert sich mit halluziniertem KI-Schriftsatz](https://legal-tech-verzeichnis.de/legal-tech-nachrichten/anwalt-blamiert-sich-mit-halluziniertem-ki-schriftsatz-gericht-spricht-von-verstoss-gegen-brao/)
75. [How Copilot Exposes Overshared SharePoint Data (And How to Fix It)](https://www.epcgroup.net/copilot-sharepoint-permissions-oversharing-fix-2026)
76. [Microsoft 365 Copilot: Lohnt sich der Rollout 2026?](https://pexon-consulting.de/blog/microsoft-365-copilot-value-workshop/)
77. [Why Agentic AI Projects Get Canceled (and How to Ship)](https://www.digitalapplied.com/blog/agentic-ai-project-cancellations-gartner-40-percent-2026)
78. [Why 40% Of Agentic AI Projects May Be Canceled By 2027](https://www.forbes.com/sites/robertszczerba/2026/07/07/why-40-of-agentic-ai-projects-may-be-canceled-by-2027/)
79. [EchoLeak Zero-Click Data Exfiltration](https://www.promptfoo.dev/lm-security-db/vuln/echoleak-zero-click-data-exfiltration-a87757e2/)
80. [Harvey: KI-Software für Kanzleien auf 15,5 Mrd. Dollar bewertet](https://www.it-boltwise.de/harvey-ki-software-fuer-kanzleien-auf-155-mrd-dollar-bewertet.html)
81. [Harvey vs Legora: Which Legal AI Are Firms Choosing in 2026? — Claude for Lawyers](https://claudeforlawyers.com/blog/harvey-vs-legora)
82. [§ 43e BRAO: KI-Dienstleister rechtssicher einbinden — Lulius](https://www.lulius.ai/blog/43e-brao-ki-dienstleister)
83. [KI in Anwaltskanzleien (BRAK) - NWB Livefeed](https://datenbank.nwb.de/Dokument/1060545/)
