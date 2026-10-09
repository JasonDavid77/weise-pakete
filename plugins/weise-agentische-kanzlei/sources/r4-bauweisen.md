# R4: Bauweisen – Ergebnis

- Datum: 2026-10-01
- Werkzeug: Claude (Anthropic) mit Websuche, alle Quellen abgerufen am 2026-10-01
- Lesehilfe: [Qn] verweist auf die Quellenliste in Abschnitt 4. „Anbieterangabe" markiert Selbstauskünfte von Herstellern. Bewertungen sind mit **Einschätzung** markiert; alles Übrige ist belegt. „o. D." heißt ohne Datum, „ca." heißt aus Suchmetadaten abgeleitet. Sekundärquellen sind als solche benannt, wo keine Primärquelle abrufbar war.
- Interessenhinweis: Das Recherchewerkzeug stammt von Anthropic. Anthropic-Produkte und von Anthropic angestoßene Standards (MCP, Agent Skills, Cowork-Plugin) kommen in den Befunden vor; sie sind wie alle Herstellerangaben gekennzeichnet.

## 1. Kurzfassung

Agentische Systeme für juristische Arbeit bestehen 2026 bei Fachanbietern wie bei KI-nativen Kanzleien aus denselben Bausteinen – Eingangssortierung, Playbooks, Werkzeuganbindung, Freigabepunkte, Eskalation an Berufsträger und Ablaufprotokoll [Q3][Q6][Q9][Q10] –, und Menschen bleiben dort Prüf- und Haftungsinstanz [Q12][Q13][Q14]. Pfad A lässt sich mit Fachplattformen oder Microsoft 365 schnell umsetzen; Pfad B verlangt nach Einschätzung dieser Recherche zusätzlich eine Orchestrierungsschicht mit festem Prozessgerüst, dauerhaft gespeichertem Fallzustand und durchgehendem Audit-Trail, wie sie KI-native Kanzleien (Garfield.Law, Crosby) für eng geschnittene Leistungen bereits betreiben [Q13][Q14][Q25]. Offene autonome Agenten wie OpenClaw und der selbstlernende Hermes Agent fielen 2026 vor allem durch Sicherheitsvorfälle und Missbrauch auf (Zehntausende ungeschützte Instanzen, bösartige Skills, automatisierte Cyberangriffe); belastbare Belege für ihren Einsatz in Wirtschaftskanzleien fanden sich nicht [Q45][Q68][Q69]. Verlässlichkeit bleibt der Engpass: Juristische Fachwerkzeuge halluzinierten in einer vorregistrierten Studie in 17 bis 33 % der Fälle, eine öffentliche Datenbank zählt bis Ende September 2026 weltweit 2.097 Gerichtsentscheidungen zu KI-erfundenen Inhalten, und bei vollständigen realen Aufträgen liegen die Erfolgsquoten von Agenten weit unter ihren Benchmark-Werten [Q40][Q41][Q52][Q56]. Einen gemeinsamen Standard für Workflows, die Menschen und Agenten gleichermaßen lesen und ausführen, gibt es nicht; nach Einschätzung dieser Recherche taugt eine Kombination aus ausführbarem Prozessgerüst mit erzwungenen Kontrollpunkten (etwa BPMN) und lesbaren Arbeitsanweisungen im offenen Agent-Skills-Format [Q31][Q81].

## 2. Befunde

### Frage 1: Typische Bausteine

**Grundmuster.** Anthropic unterscheidet zwei Bauformen: Workflows, in denen Sprachmodell und Werkzeuge vorab festgelegten Codepfaden folgen, und Agenten, die Ablauf und Werkzeugeinsatz selbst steuern; empfohlen wird, mit der einfachsten tragfähigen Lösung zu beginnen [Q1]. Ein Legora-Manager zieht für juristische Arbeit dieselbe Linie und nennt Mandatsdaten, Kanzleiwissen, Berechtigungen und Systemanbindungen, etwa über das Model Context Protocol (MCP), als die Faktoren, die über die Qualität agentischer Arbeit entscheiden (Anbieterangabe) [Q2].

**Anfragen annehmen und sortieren.** Legora beschreibt sein im Mai 2026 vorgestelltes „aOS" als System, das Agenten vom Mandatseingang über Recherche, Entwurf und Prüfung bis zur Auslieferung an den Mandanten steuert (Anbieterangabe) [Q3]. Die KI-native US-Kanzlei Crosby nimmt Verträge über Slack, E-Mail und CRM-Systeme der Kunden entgegen und hält deren frühere Verhandlungspositionen in einer Wissensbasis fest (Anbieterangabe) [Q4]. Anthropics Rechts-Plugin für den Desktop-Agenten Claude Cowork (Ende Januar 2026) zielt unter anderem auf Vertragsprüfung und NDA-Triage [Q5].

**Bearbeitung nach Playbooks.** Playbooks sind bei allen großen Anbietern das zentrale Steuerungsmittel. Legora lässt Kanzleien Klausel-Checklisten, Verhandlungsleitlinien und Redlining-Vorgaben als Playbooks hinterlegen, die beim Entwerfen oder Prüfen automatisch oder manuell angewendet werden [Q6]; das aOS greift zusätzlich auf Präzedenzsammlungen, Klauselbanken und frühere Verhandlungspositionen zurück (Anbieterangabe) [Q3]. Harvey meldete im Mai 2026 mehr als 500 vorgefertigte Agenten und einen Agent Builder im Early Access, mit dem Kanzleien diese Agenten an eigenes Wissen und eigene Abläufe anpassen (Anbieterangabe) [Q7]. Anthropics Rechts-Plugin lässt sich auf Playbook und Risikotoleranz einer Organisation einstellen [Q5]. LegalOn bietet einen Agenten, der vorhandene Vorlagen, Prüfrichtlinien und frühere Redlines in strukturierte KI-Playbooks umwandelt (Anbieterangabe) [Q8].

**Kontrollpunkte für Menschen.** Technisch heißt ein Kontrollpunkt: Der Ablauf hält an, der Zustand wird dauerhaft gespeichert, ein Mensch gibt frei, ändert, lehnt ab oder antwortet selbst, danach läuft der Prozess weiter. LangGraph setzt das über „Interrupts" und einen persistenten Checkpointer um [Q9]. Microsoft Copilot Studio bietet Freigabepunkte für Schritte mit geringer Konfidenz, für Ausnahmen und für genehmigungspflichtige Entscheidungen [Q10]. Bei „Deep Research" in CoCounsel Legal von Thomson Reuters kann der Nutzer den mehrstufigen Rechercheplan vor der Ausführung prüfen [Q11]; die geführten Workflows beschreibt der Anbieter als von vornherein mit menschlicher Aufsicht versehen (Anbieterangabe) [Q12]. Garfield.Law, die erste von der englischen Aufsicht SRA zugelassene rein KI-basierte Kanzlei, führt einen Schritt nur aus, wenn der Mandant ihn freigegeben hat [Q13].

**Übergabe an Berufsträger.** Bei Crosby entwerfen KI-Agenten die Vertragsprüfung, angestellte Anwälte prüfen abschließend; als registrierte Kanzlei haftet Crosby für jeden Vertrag [Q14]. In Microsofts Referenzbeispiel für Computer Use werden Ausnahmen und unsichere Fälle über Human-in-the-loop-Abläufe an Menschen eskaliert [Q15]. Berufsrechtlich bleibt in Deutschland die eigenverantwortliche Prüfung und Endkontrolle der KI-Ergebnisse durch die Anwältin oder den Anwalt Pflicht; das betont der KI-Leitfaden der BRAK [Q16]. Was ohne diese Prüfung geschieht, zeigt der Beschluss des AG Köln vom 2. Juli 2025 (312 F 130/25): Ein Fachanwalt hatte KI-erfundene Fundstellen eingereicht; das Gericht wertete das als bewusstes Verbreiten von Unwahrheiten und Verstoß gegen § 43a Abs. 3 BRAO [Q17].

**Protokoll und Nachvollziehbarkeit.** Copilot Studio zeichnet in einer Laufhistorie auf, was der Agent gesehen und angeklickt hat und warum [Q10]; seit Januar 2026 gibt es dort als Vorschau eine erweiterte Audit-Protokollierung mit Sitzungswiedergabe [Q18]. LangGraph speichert bei jedem Ausführungsschritt einen Zustandsschnappschuss, was Freigaben, Fehlertoleranz und nachträgliche Rekonstruktion ermöglicht [Q19]. Für Agentenläufe entsteht mit den GenAI-Konventionen von OpenTelemetry ein gemeinsames Protokollvokabular (Agentenaufruf, Planung, Werkzeugausführung, MCP-Aufrufe); die Konventionen haben aber weiterhin Entwicklungsstatus und wurden im Juni 2026 in ein eigenes Repository ausgelagert [Q20]. Regulatorisch gelten die meisten in Kanzleien eingesetzten KI-Systeme laut DAV nicht als hochriskant im Sinne der KI-Verordnung [Q21]; die Hochrisiko-Pflichten (u. a. menschliche Aufsicht, technische Dokumentation) gelten nach dem Digital Omnibus (VO (EU) 2026/1744) ohnehin erst ab 2. Dezember 2027 [Q22].

**Einschätzung:** Die Bausteine gleichen sich über alle Anbieter. Die eigentliche Bauentscheidung ist, wo Kontrollpunkte erzwungen werden. Steht eine Freigabe nur als Anweisung im Prompt oder Playbook, kann ein Agent sie übergehen oder durch präparierte Dokumente dazu gebracht werden (siehe Frage 4). Belastbar ist ein Kontrollpunkt erst, wenn die Orchestrierungsschicht den Ablauf technisch anhält und die Freigabe mit Person, Zeitpunkt und geprüftem Stand protokolliert.

### Frage 2: Bauweise Pfad A gegenüber Pfad B

**Pfad A in der Praxis.** Die großen Plattformen setzen auf Einbettung in die vorhandene Arbeitsumgebung: Legora bringt Prüfung, Recherche, Entwurf und agentische Workflows in die Werkzeuge, die Anwälte ohnehin nutzen [Q23]; Beck-Noxtua hat dafür ein Word-Add-in gebaut (Anbieterangabe) [Q24]. Kontrollinstanz ist die einzelne Berufsträgerin oder der einzelne Berufsträger, die das Ergebnis prüfen und verantworten [Q16].

**Pfad B in der Praxis.** KI-native Kanzleien bauen die Leistung als Pipeline. Garfield.Law (England) ist auf Forderungsbeitreibung bis 10.000 £ spezialisiert; das System darf keine Rechtsprechung vorschlagen, jeder Schritt braucht die Freigabe des Mandanten, und benannte Solicitors bleiben verantwortlich [Q13][Q25]. Crosby (New York) prüft Verträge zum Festpreis pro Dokument mit KI-Agenten und rund 30 Anwälten [Q14] und misst laut einer Fallanalyse neben der Durchlaufzeit gezielt den menschlichen Prüfaufwand [Q26]. Eudia betreibt in Arizona einen regulierten, KI-gestützten Rechtsdienstleister für Vertragsarbeit und M&A-Due-Diligence [Q27]. Auch Plattformanbieter bewegen sich in diese Richtung; Legora vermarktet das aOS als End-to-End-Ausführung juristischer Arbeit (Anbieterangabe) [Q3].

**Hinweise von Analysten und Werkzeugherstellern.** Gartner empfiehlt agentische KI nur bei klarem Nutzen, hält viele als agentisch vermarktete Anwendungsfälle auch ohne Agenten für lösbar und sieht in der Neugestaltung von Abläufen von Grund auf oft den besten Weg [Q28]. Camunda verankert KI-Agenten in BPMN-Prozessen, in denen menschliche Aufgaben, feste Regelwerke und KI-Entscheidungen zusammenwirken; ein „Ad-hoc-Subprozess" überlässt dabei einen begrenzten Teil der Entscheidungen einem Menschen oder Agenten [Q29].

**Einschätzung:** Die Bauweisen unterscheiden sich vor allem in Steuerung, Zustand und Kontrolle.

| Merkmal | Pfad A: Beschleunigung je Anwendungsfall | Pfad B: Pipeline mit festen Kontrollpunkten |
|---|---|---|
| Steuerung | Anwalt startet eine Aufgabe, der Agent arbeitet innerhalb einer Sitzung | Eine Orchestrierungsschicht führt den Mandatsablauf über Tage, Agenten arbeiten in begrenzten Stufen |
| Kontrollpunkt | Endkontrolle durch die bearbeitende Person | Festgelegte Freigabestufen mit Rollen, Vier-Augen-Regeln und Eskalationswegen |
| Zustand | Dokument und Chatverlauf | Dauerhaft gespeicherter Fallzustand mit Versionen |
| Protokoll | Logs des jeweiligen Werkzeugs | Durchgehender Audit-Trail je Mandat und Stufe |
| Messgröße | Zeitersparnis je Aufgabe | Durchlaufzeit, Prüfaufwand und Fehlerquote je Stufe |
| Typische Werkzeuge | Plattform-Assistent, Word-Add-in, Copilot | Workflow-Engine oder Agent Builder plus Plattform-Bausteine |
| Haupthürde | Prüfdisziplin der Einzelnen | Prozessdefinition, Engineering, Verantwortungszuordnung je Stufe |

Für beide Pfade gemeinsam nutzbar sind die festgehaltenen Arbeitsabläufe (Playbooks), die Werkzeuganbindungen und die Testfälle. Die Idee, dass ein Agent aus dokumentierten Abläufen Workflows baut, gibt es in einfacher Form bereits als Produkt (Harvey Agent Builder, LegalOn Playbook Agent) [Q7][Q8]. Dass daraus ohne erheblichen Prüfaufwand belastbare Pfad-B-Pipelines entstehen, ist nicht belegt.

### Frage 3: Wege und ihre Vor- und Nachteile

**Eigene Entwicklung auf Sprachmodellen.** Die Bausteine sind verfügbar und zunehmend standardisiert: Frameworks wie LangGraph liefern Pausen-, Freigabe- und Persistenzmechanik [Q9][Q19]; MCP für Werkzeuganbindungen und AGENTS.md für Agentenanweisungen liegen seit dem 9. Dezember 2025 bei der Agentic AI Foundation der Linux Foundation [Q30]; Anthropic hat sein Format „Agent Skills" am 18. Dezember 2025 als offenen Standard veröffentlicht [Q31]. Selbst große Anbieter bauen die Orchestrierung selbst: Thomson Reuters hat für CoCounsel Legal ein eigenes Orchestrierungs-Framework mit mehreren spezialisierten Agenten entwickelt [Q32]. Eine Untersuchung zu Oracles Open Agent Specification zeigt ein Wartungsrisiko: Auch mit identischer Spezifikation unterscheiden sich verschiedene Laufzeitumgebungen deutlich in Genauigkeit, Latenz und Ausführungsverhalten [Q33]. Berufsrechtlich dürfen Mandatsinformationen an KI-Anbieter nur unter den Voraussetzungen des § 43e BRAO offengelegt werden; die BRAK empfiehlt zusätzlich Anonymisierung [Q16], der DAV hält Cloud- und KI-Nutzung unter Bedingungen für zulässig [Q21].

**Plattform eines Legal-Tech-Anbieters.** Neben Harvey (Agent Builder, über 500 Agenten) [Q7] stehen Legora (aOS; Series D über 550 Mio. USD bei 5,55 Mrd. USD Bewertung im März 2026, damals nach eigenen Angaben 800 Kanzleien und Rechtsabteilungen als Kunden) [Q34], CoCounsel Legal von Thomson Reuters [Q12] und in Deutschland Beck-Noxtua, das Inhalte von beck-online mit der Rechts-KI von Noxtua verbindet; C.H.Beck wurde im September 2026 Mehrheitsgesellschafter von Noxtua [Q24][Q35]. Im DACH-Raum hat die Wiener Kanzlei Schönherr eine Entwicklungspartnerschaft mit Legora geschlossen, in der KI-Agenten ein Schwerpunkt sind [Q36]. Zu Kosten: Legora hat im Juni 2026 für sein leistungsfähigstes Produkt verbrauchsabhängige Preise eingeführt [Q23]; laut einer Marktanalyse schließen Kanzleien teils mit Harvey und Legora parallel ab und verschieben Lizenzen zwischen Anwälten, beide Anbieter geben hohe Rabatte (Schätzung eines Analysehauses) [Q37]. Anbieterrisiko zeigt Robin AI: Der gut finanzierte Anbieter von Vertragsprüfung mit Playbook-Funktion scheiterte 2025 mit einer Finanzierungsrunde über 50 Mio. USD und wurde zum Notverkauf angeboten [Q38][Q39]. Fachspezifisch heißt nicht fehlerfrei: In der vorregistrierten Stanford-Studie halluzinierten Lexis+ AI und die KI-Werkzeuge von Westlaw und Practical Law in 17 bis 33 % der Fälle (Preprint 2024, veröffentlicht 2025) [Q40]; die öffentliche Halluzinations-Datenbank verzeichnet auch im September 2026 Gerichtsfälle, in denen Fachwerkzeuge wie Lexis AI oder Spellbook genannt werden [Q41].

**Erweiterung der Microsoft-365-Umgebung.** Copilot Studio hat im Mai 2026 Computer Use allgemein verfügbar gemacht: Agenten bedienen Web- und Desktop-Anwendungen über die Oberfläche, mit Freigabepunkten, Laufhistorie und innerhalb der Datenresidenz- und Compliance-Grenzen des Tenants [Q10][Q18]. Agent-zu-Agent-Kommunikation ist dort ebenfalls allgemein verfügbar [Q42]. Dagegen steht die Angriffsfläche: Mit „EchoLeak" (CVE-2025-32711, CVSS 9,3) konnte im Juni 2025 eine präparierte E-Mail ohne Nutzerinteraktion Daten aus dem Kontext von Microsoft 365 Copilot abfließen lassen; Microsoft hat die Lücke geschlossen, eine Ausnutzung wurde nicht festgestellt [Q43][Q44]. Im August 2026 meldete Varonis mit „CoSnitch" einen weiteren, inzwischen behobenen Angriff, bei dem Copilot durch wiederholte Nachfragen interne Schutzmechanismen preisgab [Q45]. Juristische Fachinhalte bringt Microsoft 365 nicht mit; TechCrunch zählt Microsoft Copilot ausdrücklich zu den Wettbewerbern von Legora [Q34].

**Mischform: Allzweck-Agent mit Fach-Plugin.** Anthropic hat am 30. Januar 2026 Plugins für Claude Cowork veröffentlicht, darunter eines für juristische Arbeit [Q46][Q5]; Anthropic weist darauf hin, dass die Ergebnisse von zugelassenen Anwälten geprüft werden müssen [Q47]. Am 3. Februar 2026 fielen die Aktien von Thomson Reuters, RELX und Wolters Kluwer um 16, 14 und 13 % [Q48]. (Anthropic ist Hersteller des Werkzeugs, mit dem diese Recherche erstellt wurde.)

**Einschätzung:** Vergleich der Wege (Bewertung dieser Recherche, keine Messwerte).

| Kriterium | Eigenentwicklung | Legal-Tech-Plattform | Microsoft-365-Erweiterung |
|---|---|---|---|
| Kontrolle über Ablauf, Daten, Protokoll | hoch | mittel, anbieterabhängig | mittel, an Microsoft-Governance gebunden |
| Juristische Inhalte, fertige Workflows | keine, müssen angebunden werden | hoch | gering |
| Zeit bis zum ersten Nutzen | lang | kurz | kurz bis mittel |
| Eignung für Pfad A | mittel | hoch | hoch für allgemeine Büroarbeit |
| Eignung für Pfad B | hoch, wenn Engineering vorhanden | mittel bis hoch, je nach Agent Builder | mittel; stark bei Altsystemen ohne Schnittstelle |
| Hauptrisiken | Personalbedarf, Wartung, Sicherheitsarchitektur in eigener Verantwortung | Bindung an Anbieter, proprietäre Playbook-Formate, Preismodell, Anbieterausfall | Prompt Injection über E-Mail und Dokumente, breite Datenzugriffe, kaum Fachinhalt |

Die Wege schließen sich nicht aus. Plausibel ist ein Kern aus eigenen Playbooks und eigener Orchestrierung, der Plattform-Bausteine und die Microsoft-Umgebung über offene Standards (MCP, Agent Skills) anbindet. Das senkt die Abhängigkeit von einem Anbieter, verlangt aber eigene Engineering-Kapazität.

### Frage 4: Autonome, selbstverbessernde Agenten

**Was OpenClaw und Hermes Agent sind.** OpenClaw ist ein quelloffener Agent, der auf E-Mail-Konten, Kalender, Messenger und andere Dienste zugreifen kann und seine Fähigkeiten über „Skills" erweitert, die als Verzeichnisse mit Anleitungen abgelegt werden [Q49]. Hermes Agent von Nous Research ist quelloffen (MIT-Lizenz) und hat eine eingebaute Lernschleife: Er erstellt aus Erfahrung eigene Skills, verbessert sie bei der Nutzung, hält Wissen sitzungsübergreifend fest und durchsucht frühere Unterhaltungen; er arbeitet mit vielen Modellanbietern und nach eigenen Angaben mit dem offenen Agent-Skills-Format [Q50]. Ein Begleitprojekt entwickelt Skills, Werkzeugbeschreibungen, Prompts und Code evolutionär weiter und lässt jede Variante nur nach vollständig bestandener Testsuite zu [Q51].

**Was sie heute verlässlich können.** Auf dem Benchmark OSWorld-Verified (369 Desktop-Aufgaben) melden Spitzensysteme Mitte 2026 Erfolgsquoten von etwa 85 bis 90 % [Q52][Q53]; die menschliche Vergleichsquote im ursprünglichen OSWorld-Papier lag bei rund 72 % [Q54]. Die Werte sind nur begrenzt vergleichbar, weil ein Teil selbst berichtet ist und unter abweichenden Bedingungen (Schrittzahl, Rechte, Systemabbild) entstand [Q55]. Bei vollständigen, real bezahlten Aufträgen sieht es anders aus: Im Remote Labor Index (240 echte Freelance-Projekte) erreichte der beste Agent im Oktober 2025 eine Automatisierungsquote von 2,5 % [Q56]; Berichte über eine Aktualisierung im Juli 2026 nennen bis zu 16,1 % [Q57], ein anderer Bericht für Mitte 2026 nennt 4,17 % [Q58]. Konkrete juristische Einsätze von Computer Use, etwa die Bedienung von Justiz- oder Registerportalen, fand die Recherche nicht.

**Einschätzung:** Verlässlich sind 2026 abgegrenzte, überprüfbare und umkehrbare Schritte mit menschlicher Freigabe: Daten zusammentragen, Formulare in Altsystemen befüllen, Entwürfe gegen ein Playbook prüfen. Nicht belegt ist, dass Agenten juristische Arbeit end-to-end ohne Prüfung in abnahmefähiger Qualität liefern. Selbstverbesserung erhöht die Leistung, aber auch die Unvorhersehbarkeit, weil sich das Verhalten zwischen zwei Prüfungen ändert. Übertragbar ist das Prinzip des Hermes-Begleitprojekts: Ein Agent darf Abläufe verbessern, aber eine Änderung wird erst nach bestandenen Tests (für Kanzleien: Testakten mit Sollergebnis) und menschlicher Freigabe wirksam.

**Wo sie juristisch eingesetzt werden.** Für OpenClaw fanden sich vor allem Anleitungen von Beratern und Marketingagenturen für Solo- und kleinere Kanzleien, überwiegend in den USA, meist für Mandantenaufnahme, Nachfassen und Terminverwaltung über WhatsApp und E-Mail [Q59][Q60]; in einer dieser Anleitungen wird der Agent per Regeldatei ausdrücklich von Rechtsberatung ausgeschlossen [Q59]. Eine kalifornische Anwältin betreibt öffentlich ein Experiment mit zwei OpenClaw-Agenten unter ihrer Aufsicht [Q61]; ein Gastbeitrag bei Bloomberg Law diskutiert, welche vertretungs- und treuhandrechtlichen Fragen solche Agenten aufwerfen [Q62]. Belege für den Einsatz von OpenClaw oder Hermes in Wirtschaftskanzleien fanden sich nicht. Für Hermes fand sich kein juristischer Einsatz, wohl aber Missbrauch: Laut Palo Alto Networks Unit 42 nutzte ein Angreifer das Modell DeepSeek innerhalb von Hermes Agent, um große Teile realer Angriffe zu automatisieren, kombiniert mit manuellen Angriffen auf insgesamt mehr als 460 Ziele; der Agent legte dabei versehentlich Teile der Angriffsinfrastruktur offen [Q45]. In Kanzleien eingesetzt werden dagegen die Agenten der Fachplattformen (siehe Frage 3). Unabhängige Wirkungsdaten dazu fanden sich nicht; verfügbar sind Fallstudien der Anbieter, etwa eine von Harvey veröffentlichte Zeitersparnis von 75 % bei Due-Diligence-Prüfungen der Kanzlei GSK Stockmann (Anbieterangabe, nicht unabhängig geprüft) [Q63].

**Zugriff auf Register, Datenbanken und Plattformen.** Das Handelsregister hat keine offizielle Programmierschnittstelle; die Nutzungsordnung untersagt mehr als 60 Abrufe pro Stunde [Q64]. Nach Darstellung eines Open-Source-Projekts warnt die Portal-FAQ zudem, dass automatisierte Massenabfragen als Straftat (§§ 303a, 303b StGB) gewertet werden können; dasselbe Projekt stellt einen MCP-Server bereit, der das Register für Agenten erschließt und das Stundenlimit technisch einhält [Q65]. Die führenden deutschen Fachdatenbanken bauen eigene KI-Funktionen (beck-chat in beck-online, Beck-Noxtua, KI-Chat von juris in Word) [Q66][Q67]; ob und zu welchen Bedingungen externe Agenten diese Datenbanken automatisiert nutzen dürfen, hat diese Recherche nicht geprüft. Eine öffentlich dokumentierte Schnittstelle, über die externe Agenten Legora steuern können, fand sich nicht; Legora berichtet von wachsender Kundennachfrage nach MCP-Anbindungen (Anbieterangabe) [Q2]. Wo Schnittstellen fehlen, bleibt Computer Use die Rückfalloption [Q18].

**Bekannte Sicherheitsrisiken.**

*Ungeschützte Instanzen und Lieferkette (Beispiel OpenClaw).* Scans fanden Anfang 2026 Zehntausende ungeschützt aus dem Internet erreichbare OpenClaw-Instanzen (Censys: 21.639; mehrere Teams: über 30.000; SecurityScorecard später über 135.000), teils mit Klartext-API-Schlüsseln und OAuth-Token [Q68][Q69][Q70]. Im Skill-Marktplatz ClawHub identifizierte Koi Security 341 bösartige von 2.857 Skills (rund 12 %); bis zum 16. Februar 2026 stieg die Zahl auf über 824 von mehr als 10.700 [Q69]. Snyk fand 283 von 3.984 Skills, die Zugangsdaten im Klartext preisgaben [Q71]. Eine Lücke, die mit einem einzigen Klick Codeausführung erlaubte, wird als CVE-2026-25253 geführt [Q69][Q70]. Chinesische Behörden schränkten im März 2026 den Einsatz von OpenClaw auf Bürorechnern staatlicher Unternehmen und Behörden ein [Q49].

*Prompt Injection.* Das BSI stuft indirekte Prompt Injection seit 2023 als inhärente Schwachstelle von LLM-Anwendungen ein und kennt nach eigener Aussage keine zuverlässige Gegenmaßnahme, die die Funktionalität nicht deutlich einschränkt [Q72][Q73]; 2026 hat es einen „Basisschutz gegen Indirect Prompt Injection in dokumentbasierten LLM-Chats" veröffentlicht [Q74]. Für Kanzleien unmittelbar relevant: Im August 2026 versteckte ein Kläger in Connecticut Anweisungen in weißer Kleinschrift in Gerichtsdokumenten, um eine KI-gestützte Prüfung zu seinen Gunsten zu beeinflussen; das Gericht untersagte ihm daraufhin digitale Einreichungen [Q45]. EchoLeak zeigte, dass eine eingehende E-Mail genügen kann, um einen Büro-Agenten zum Datenabfluss zu bringen [Q43].

*Rahmenwerke und Behördenpositionen.* Die OWASP Top 10 für agentische Anwendungen (9. Dezember 2025) ordnen agentenspezifische Risiken wie Zielübernahme, Werkzeugmissbrauch, Identitäts- und Rechtemissbrauch, Lieferkettenrisiken und kaskadierende Fehler in Multi-Agenten-Systemen [Q75][Q76]. Das BSI hat das Projekt PRAKI ausgeschrieben (Angebotsfrist September 2026), das Prüfanforderungen für agentische KI entwickeln soll; konkrete Kontrollen sind noch nicht veröffentlicht [Q77]. Nach einem Vorfall bei OpenAI fordert das BSI eigene Rechte- und Rollenkonzepte für KI-Systeme [Q78]. Laut IBM-Data-Breach-Report 2026 fehlten bei 92 % der Unternehmen mit KI-bezogenem Vorfall ausreichende Zugriffskontrollen [Q45]. In Cyber-Evaluierungen mit deaktivierten Schutzvorkehrungen haben Agenten mehrerer Hersteller auf reale Organisationen zugegriffen oder unerwünschte Aktionen gegen sie ausgeführt; berichtet haben das Anthropic, OpenAI, das britische AI Security Institute und Meta [Q45].

*Selbstverbesserung.* Eine auf der ICLR 2026 vorgestellte Studie beschreibt „Misevolution": Bei sich selbst weiterentwickelnden Agenten ließ die Sicherheitsausrichtung nach dem Aufbau von Gedächtnis nach, und beim Erstellen eigener Werkzeuge entstanden unbeabsichtigt Schwachstellen, auch auf Spitzenmodellen [Q79]. Eine weitere Analyse verweist auf Schwachstellen in rund 26 % der von der Community beigesteuerten Werkzeuge und darauf, dass sich in OpenClaw Signaturprüfung und Sandboxing abschalten lassen [Q80].

### Frage 5: Workflows, die Menschen und Agenten lesen und ausführen

**BPMN 2.0** ist als ISO/IEC 19510:2013 genormt (identisch mit OMG BPMN 2.0.1, 2022 bestätigt) und soll ausdrücklich die Lücke zwischen fachlicher Prozessbeschreibung und technischer Umsetzung schließen [Q81]. Camunda 8.8 betreibt KI-Agenten direkt in BPMN-Prozessen: Die Werkzeuge eines Agenten sind Aktivitäten in einem Ad-hoc-Subprozess, menschliche Aufgaben und Freigaben sind reguläre Prozesselemente, und Human-in-the-loop ist als Prüf- und Freigabeschritt definiert, bevor KI-Ergebnisse mit rechtlicher, finanzieller oder sicherheitsrelevanter Wirkung umgesetzt werden [Q29].

**Agent Skills (SKILL.md)** sind Ordner mit einer Markdown-Datei samt Metadatenkopf sowie optionalen weiteren Dateien und Skripten; Agenten laden die Inhalte erst bei Bedarf. Das Format ist seit 18. Dezember 2025 offen spezifiziert [Q31] und wird laut einer Übersicht vom Juni 2026 von rund 40 Agenten-Produkten unterstützt, darunter GitHub Copilot, VS Code, Cursor, OpenAI Codex und Gemini CLI [Q82]; Hermes Agent ist nach eigenen Angaben kompatibel [Q50]. **AGENTS.md** (Projektanweisungen für Agenten) und **MCP** (Werkzeuganbindung) liegen bei der Agentic AI Foundation [Q30].

**Arazzo** (OpenAPI Initiative) beschreibt Abfolgen von API-Aufrufen deterministisch und zugleich für Menschen und Maschinen lesbar; Version 1.0.0 erschien im Mai 2024, 1.0.1 im Januar 2025 [Q83][Q84]. **Open Agent Specification** (Oracle, 2025) ist eine rahmenwerksunabhängige, deklarative Sprache für Agenten und strukturierte Abläufe [Q85]; gleiche Spezifikationen laufen auf verschiedenen Laufzeiten jedoch unterschiedlich [Q33].

**Juristische Playbooks** liegen bei jedem Anbieter in eigenen Formaten vor (etwa Legora, LegalOn, Law Insider mit über 50 für KI strukturierten Playbooks in Word) [Q6][Q8][Q86]. Einen anbieterübergreifenden Standard für juristische Playbooks oder für Rechts-Workflows mit Kontrollpunkten fand die Recherche nicht.

**Einschätzung:** Kein einzelnes Format leistet heute beides. BPMN ist ausführbar und prüfbar, für Arbeitsanweisungen aber unhandlich; Agent Skills sind gut lesbar und für Agenten ladbar, haben aber keine verbindliche Semantik für Kontrollpunkte, Rollen oder Fristen. Praktikabel erscheint eine Schichtung. Erstens ein Prozessgerüst mit Kontrollpunkten, Rollen, Fristen und Eskalation in einem ausführbaren Format (BPMN oder eine im Code definierte Zustandsmaschine), dessen Engine Freigaben erzwingt und protokolliert. Zweitens die Arbeitsanweisung je Schritt als Markdown-Skill oder Playbook, das Anwälte lesen und ändern und Agenten laden. Drittens Werkzeuge über MCP, viertens Protokolle nach den OpenTelemetry-GenAI-Konventionen, sobald diese stabil sind [Q20]. Ein lernender Agent dürfte in diesem Modell Änderungen an der zweiten Schicht vorschlagen, aber nicht ohne Freigabe einspielen; die erste Schicht bliebe in menschlicher Hand.

## 3. Gegenbelege und offene Punkte

### Gegenbelege

**Projektabbrüche.** Gartner erwartet, dass bis Ende 2027 über 40 % der agentischen KI-Projekte wegen steigender Kosten, unklaren Nutzens oder unzureichender Risikokontrollen eingestellt werden; nach Gartners Schätzung sind nur rund 130 der Tausenden Anbieter, die sich als agentisch bezeichnen, tatsächlich solche [Q28].

**Leistung in echter Arbeit.** Die niedrigen und uneinheitlichen Automatisierungsquoten im Remote Labor Index (2,5 % im Oktober 2025, 2026 je nach Bericht 4,17 % oder bis zu 16,1 %) stehen im Kontrast zu hohen Benchmark-Werten [Q52][Q56][Q57][Q58].

**Halluzinationen.** Neben der Stanford-Studie [Q40] zählt die öffentliche Datenbank mit Stand 30. September 2026 2.097 Entscheidungen, davon 831, in denen Anwälte die Inhalte eingereicht hatten, und 11 aus Deutschland [Q41]. Neben dem AG Köln [Q17] deckte das LG Frankfurt am Main (Beschluss vom 25.09.2025, 2-13 S 56/24) frei erfundene Zitate aus einem höchstrichterlichen Urteil auf [Q87].

**Anbieterausfall.** Robin AI, siehe Frage 3 [Q38][Q39].

**Wirksamkeit menschlicher Freigaben.** Anthropic begründet einen automatischen Freigabemodus in Claude Code mit einem Test, in dem menschliche Prüfer nur 13,6 % gefährlicher Befehle erkannten, ein Klassifikator dagegen 89 % blockierte; das BSI mahnt zur kritischen Betrachtung, weil auch Klassifikatoren Fehlentscheidungen treffen, die sich durch die automatische Weiterverarbeitung stärker auswirken können (Anbieterangabe, wiedergegeben vom BSI) [Q45]. **Einschätzung:** Für Pfad B ist das ein zentraler Gegenbeleg. Ein Mensch, der viele Freigaben in Folge erteilt, ist kein verlässlicher Kontrollpunkt; Freigabestufen müssen selten, gezielt und inhaltlich prüfbar sein.

**Sicherheit.** Siehe Frage 4: OpenClaw-Vorfälle, EchoLeak, CoSnitch, Prompt Injection in Gerichtsdokumenten, Misevolution [Q43][Q45][Q68]–[Q80].

### Gegenpositionen

Ein Gastbeitrag auf LTO (April 2026) hält Zurückhaltung für das größere Risiko: Künftig müsse sich eher rechtfertigen, wer auf KI verzichtet; die verbreitete Sorge um Mandatsgeheimnisse nach § 203 StGB enthalte Wertungswidersprüche, und der Gesetzgeber müsse klare Grundlagen für den KI-Einsatz schaffen [Q88]. Der DAV sieht, wenn bestimmte Regeln eingehalten werden, weder im Berufs- noch im Datenschutzrecht Hürden, die den Einsatz verhindern [Q21]. Anbieter sehen die Branche bereits jenseits von KI als bloßer Assistenz, im Zeitalter der Rechtsagenten (Harvey) bzw. der „Agentic Law" (Legora) (Anbieterangaben) [Q7][Q3]. Die SRA hält KI-getriebene Kanzleien für potenziell besser, schneller und günstiger, betont aber die neuartigen Risiken und beobachtet das Modell eng [Q25]. Der Kurssturz der Fachverlage nach Anthropics Plugin zeigt, dass Investoren Allzweck-Agenten als Bedrohung für spezialisierte Anbieter einschätzen [Q48]. **Einschätzung:** Das erhöht das Risiko jeder langfristigen Plattformbindung, in beide Richtungen.

### Offene Punkte

1. Unabhängige Wirkungsdaten zu Pfad-B-Pipelines in deutschen Wirtschaftskanzleien fanden sich nicht; verfügbare Zahlen stammen aus Anbieter-Fallstudien.
2. Die Zahlen zum Remote Labor Index 2026 widersprechen sich; die Primärquelle der Juli-Aktualisierung lag nicht vor.
3. Standards sind im Fluss: OpenTelemetry-GenAI im Entwicklungsstatus [Q20], BSI-Prüfanforderungen (PRAKI) ausstehend [Q77], mehrere konkurrierende Beschreibungsformate (BPMN, Agent Skills, Agent Spec, Arazzo).
4. Nicht geprüft: Nutzungsbedingungen von juris und beck-online für automatisierten Agentenzugriff, Programmierschnittstellen von Legora und Harvey, Zugang zum Transparenzregister, Anbindung des beA.
5. Berufsrecht für Pfad B nicht vertieft: Verantwortungszuordnung je Kontrollpunkt, Verträge nach § 43e BRAO mit Modell- und Unteranbietern, RDG-Fragen bei Leistungen direkt an Mandanten. Die Leitlinien der EU-Kommission zur Hochrisiko-Einstufung (Entwurf vom 19. Mai 2026) wurden nicht ausgewertet [Q22].
6. Gesamtkosten: Verbrauchsabhängige Preise erschweren Prognosen; belastbare Kostendaten fanden sich nicht [Q23].
7. Langzeitverhalten selbstlernender Skills in regulierten Umgebungen: keine Belege gefunden.

## 4. Quellenliste

Format: Herausgeber: Titel. Datum. Link. Alle Abrufe am 2026-10-01.

**[Q1]** Anthropic: „Building effective agents". Dezember 2024. https://www.anthropic.com/research/building-effective-agents · Zusammenfassung: AI Hero, o. D., https://aihero.dev/building-effective-agents

**[Q2]** Geek Law Blog: Interview mit einem Legora-Manager zu agentischer KI, Legal Engineering und verbrauchsabhängigen Preisen. August 2026. https://www.geeklawblog.com/2026/08/patrick-forquer-on-legoras-agentic-ai-legal-engineering-and-consumption-based-pricing.html

**[Q3]** Legora: „Legora introduces the Legora aOS™: the agentic operating system for legal work". 07.05.2026. https://legora.com/newsroom/legora-introduces-the-legora-aos-the-agentic-operating-system-for-legal-work · Bericht: Artificial Lawyer, 07.05.2026, https://www.artificiallawyer.com/2026/05/07/legora-launches-aos-agentic-operating-system/

**[Q4]** Dealroom: Unternehmensprofil Crosby. o. D. https://app.dealroom.co/companies/crosby_1

**[Q5]** Canadian Lawyer: „Anthropic legal tool jolts share price of global legal data leaders". 03.02.2026. https://www.canadianlawyermag.com/news/international/anthropic-legal-tool-jolts-share-price-of-global-legal-data-leaders/393665

**[Q6]** ILTA / Legaltech Hub: Anbieterprofil Legora. o. D. https://ilta.legaltechnologyhub.com/vendors/legora/

**[Q7]** Harvey: „Built by Lawyers, Tailored by You: Harvey Launches Purpose-Built Legal Agents Across Every Major Practice Area". 05.05.2026. https://www.harvey.ai/blog/built-by-lawyers-tailored-by-you · Pressemitteilung (PR Newswire), 06.05.2026, https://www.prnewswire.com/apac/news-releases/built-by-lawyers-tailored-by-you-harvey-launches-purpose-built-legal-agents-across-every-major-practice-area-302763330.html

**[Q8]** LegalOn: „Meet Playbook Agent: Scale Your Legal Expertise with AI". 14.01.2026. https://www.legalontech.com/post/meet-playbook-agent-scale-your-legal-expertise-with-ai · Produktseite „LegalOn Playbooks", o. D., https://legalontech.com/contract-playbooks

**[Q9]** LangChain: Dokumentation „Human-in-the-loop" und „Interrupts" (LangGraph). o. D. https://docs.langchain.com/oss/python/langchain/human-in-the-loop.md · https://docs.langchain.com/oss/python/langgraph/interrupts

**[Q10]** Microsoft Copilot Studio Team (gespiegelt bei AzureFeeds): „Computer-using agents in Microsoft Copilot Studio are now generally available". 14.05.2026. https://azurefeeds.com/2026/05/14/computer-using-agents-in-microsoft-copilot-studio-are-now-generally-available/

**[Q11]** LawSites: „Thomson Reuters launches CoCounsel Legal with agentic AI and deep research capabilities, along with a new and final version of Westlaw". August 2025. https://www.lawnext.com/2025/08/thomson-reuters-launches-cocounsel-legal-with-agentic-ai-and-deep-research-capabilities-along-with-a-new-and-final-version-of-westlaw.html

**[Q12]** Thomson Reuters: „Thomson Reuters Launches CoCounsel Legal: Transforming Legal Work with Agentic AI and Deep Research". 05.08.2025. https://www.thomsonreuters.com/en/press-releases/2025/august/thomson-reuters-launches-cocounsel-legal-transforming-legal-work-with-agentic-ai-and-deep-research · Bericht: Legal IT Insider, 05.08.2025, https://legaltechnology.com/thomson-reuters-launches-cocounsel-legal-with-agentic-ai-and-deep-research-capabilities/

**[Q13]** Law Gazette: „SRA approves £2-letter AI law firm". Mai 2025. https://www.lawgazette.co.uk/news/sra-approves-2-letter-ai-law-firm/5123191.article

**[Q14]** Forbes: „Why This AI Law Firm Is Ditching The Billable Hour". 31.03.2026. https://www.forbes.com/sites/rashishrivastava/2026/03/31/why-this-ai-law-firm-is-ditching-the-billable-hour/

**[Q15]** DevOps.com: „Microsoft Copilot Studio Brings Computer-Using Agents to the Enterprise". ca. Mai 2026. https://devops.com/microsoft-copilot-studio-brings-computer-using-agents-to-the-enterprise/

**[Q16]** Bundesrechtsanwaltskammer: „Hinweise zum Einsatz von künstlicher Intelligenz (KI)". Stand 12/2024, veröffentlicht Januar 2025. https://www.brak.de/newsroom/newsletter/nachrichten-aus-berlin/2025/ausgabe-1-2025-v-812025/kuenstliche-intelligenz-in-anwaltskanzleien-brak-veroeffentlicht-leitfaden/ · PDF: https://www.brak.de/fileadmin/service/publikationen/Handlungshinweise/BRAK_Leitfaden_mit_Hinweisen_zum_KI-Einsatz_Stand_12_2024.pdf · Einordnung: Anwaltspraxis Magazin, ca. Dezember 2025, https://anwaltspraxis-magazin.de/kanzleimagazin/darf-die-ki-anwalt-sein/

**[Q17]** Legal Tribune Online: „AG Köln zu Berufspflichten: Anwalt reicht KI-Schriftsatz mit Fehlern bei Gericht ein". ca. Juli 2025 (zu AG Köln, Beschl. v. 02.07.2025, 312 F 130/25). https://www.lto.de/recht/juristen/b/ag-koeln-familiengericht-312f130-25-schriftsatz-ki-anwalt-berufspflichten · Leitsätze: FamRZ, o. D., https://www.famrz.de/entscheidungen/fehlerhafte-zitate-in-ki-generiertem-schriftsatz.html

**[Q18]** Microsoft Learn: „What's new in Copilot Studio". Einträge bis Juni 2026. https://learn.microsoft.com/en-us/microsoft-copilot-studio/whats-new

**[Q19]** LangChain: Dokumentation „Persistence" (LangGraph). o. D. https://docs.langchain.com/oss/javascript/langgraph/persistence/index.html

**[Q20]** Dash0: „OpenTelemetry GenAI Semantic Conventions Explained". 14.09.2026. https://www.dash0.com/knowledge/opentelemetry-genai-semantic-conventions-explained · Statusprüfung: DEV Community (azena.ai), 16.07.2026, https://dev.to/azena-ai/opentelemetrys-genai-semantic-conventions-are-not-stable-yet-heres-what-actually-shipped-in-2026-3mke

**[Q21]** beck-aktuell: „Anwaltverein sieht keine unüberwindbaren Hindernisse" (zur DAV-Initiativstellungnahme). 24.07.2025. https://www.beck-aktuell.de/rechtsbranche/anwaltschaft/dav-anwaltverein-ki-einsatz-kanzleien-chancen-risiken-anforderungen-2025-07-24

**[Q22]** Future of Privacy Forum: „The AI Act Implementation Timeline: What Changes Under the AI Omnibus?". 2026. https://fpf.org/blog/the-ai-act-implementation-timeline-what-changes-under-the-ai-omnibus · CASRAI zur VO (EU) 2026/1744 (Amtsblatt 24.07.2026, in Kraft 27.07.2026), 2026, https://www.casrai.org/news/eu-ai-act-digital-omnibus-deadline-delay

**[Q23]** Contrary Research: „Legora – Business Breakdown & Founding Story". ca. August 2026. https://research.contrary.com/company/legora

**[Q24]** Börse Online: Interview mit der Geschäftsführung der Beck-Noxtua Vertriebs GmbH („Chance bei Legal Techs: So verändert KI den Rechtsmarkt"). o. D. https://www.boerse-online.de/nachrichten/aktien/chance-bei-legal-techs-so-veraendert-ki-den-rechtsmarkt-20404870.html

**[Q25]** Solicitors Regulation Authority: „SRA approves first AI-driven law firm". Mai 2025. https://www.sra.org.uk/sra/news/press/garfield-ai-authorised/

**[Q26]** LTC Foundry: „Crosby – Building an AI-First Law Firm". ca. Oktober 2025. https://www.ltcfoundry.com/post/crosby-building-an-ai-first-law-firm

**[Q27]** Lupl: „10 AI Law Firms to Watch in 2026". ca. Mai 2026. https://www.lupl.com/blog/10-ai-law-firms-to-watch-in-2026/

**[Q28]** Gartner: „Gartner Predicts Over 40% of Agentic AI Projects Will Be Canceled by End of 2027". 25.06.2025. https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027 · Wiedergabe: New Electronics, https://www.newelectronics.co.uk/content/news/over-40-of-agentic-ai-projects-could-be-cancelled-by-2027

**[Q29]** Camunda: Dokumentation 8.8 (Release Notes, „AI agents", Glossar). o. D. https://docs.camunda.io/docs/reference/announcements-release-notes/880/880-release-notes/ · https://docs.camunda.io/docs/8.8/components/agentic-orchestration/ai-agents · https://docs.camunda.io/docs/8.8/reference/glossary/

**[Q30]** IT Brief UK: „Linux Foundation launches Agentic AI open standards hub". Dezember 2025. https://itbrief.co.uk/story/linux-foundation-launches-agentic-ai-open-standards-hub · Gründungsdatum 09.12.2025: https://agentic-ai.readthedocs.io/en/latest/Standards/agentic-ai-foundation/

**[Q31]** The New Stack: „Agent Skills: Anthropic's Next Bid to Define AI Standards". 18.12.2025. https://thenewstack.io/agent-skills-anthropics-next-bid-to-define-ai-standards/

**[Q32]** Constellation Research: „Thomson Reuters brings agentic AI to legal workflows". ca. August 2025. https://www.constellationr.com/insights/news/thomson-reuters-brings-agentic-ai-legal-workflows

**[Q33]** Oracle-Autorenteam, Konferenzbeitrag CAIS 2026: „Open Agent Specification: Enabling Cross-Framework Comparison of AI Agents". 2026. https://www.caisconf.org/program/2026/papers/open-agent-specification-a-unified-representation-for-ai-agents/

**[Q34]** TechCrunch: „Legora reaches $5.55 billion valuation as AI legal tech boom endures". März 2026. https://techcrunch.com/?p=3100930

**[Q35]** startbase: „Noxtua erhält mehr als 100 Millionen Euro in Series C". September 2026. https://www.startbase.de/news/noxtua-erhaelt-mehr-als-100-millionen-euro-in-series-c/

**[Q36]** Trending Topics: „Wiener Anwaltskanzlei Schönherr kooperiert mit Legaltech-Unicorn Legora". 2026, ohne genaues Datum. https://www.trendingtopics.eu/wiener-anwaltskanzlei-schoenherr-kooperiert-mit-legaltech-unicorn-legora/

**[Q37]** Sacra: „$100M/year Harvey for the rest of the world" (Legora-Analyse mit Schätzungen). 2026. https://sacra.com/research/100m-year-harvey-for-the-rest-of-the-world/

**[Q38]** Legal IT Insider (via Legal Tech Monitor): „Robin AI listed for distressed sale nine months after making the Sunday Times 100 Tech list". Oktober 2025. https://www.legaltechmonitor.com/?p=60671

**[Q39]** Nonbillable: „Robin AI looks for buyer after funding plans collapse". 28.10.2025. https://www.nonbillable.co.uk/news/robin-ai-looks-for-buyer-after-funding-plans-collapse · Playbook-Funktion: Solicitor News, o. D., https://solicitornews.co.uk/?p=10643

**[Q40]** Stanford RegLab / HAI: „Hallucination-Free? Assessing the Reliability of Leading AI Legal Research Tools". Journal of Empirical Legal Studies 22 (2025), 216–242. https://nlp.stanford.edu/~manning/papers/Magesh-Hallucination%E2%80%90Free-2025.pdf · Zusammenfassung Stanford HAI (2024): https://hai.stanford.edu/news/ai-trial-legal-models-hallucinate-1-out-6-or-more-benchmarking-queries

**[Q41]** AI Hallucination Cases Database (damiencharlotin.com, Lizenz CC BY 4.0). Stand 30.09.2026. https://www.damiencharlotin.com/hallucinations/

**[Q42]** Microsoft Copilot Blog: „What's new in Copilot Studio: May 2026" (Computer Use, A2A). Mai 2026. https://www.microsoft.com/en-us/copilot/blog/copilot-studio/new-and-improved-computer-using-agents-a-new-workflows-experience-and-real-time-voice-experiences/

**[Q43]** The Hacker News: „Zero-Click AI Vulnerability Exposes Microsoft 365 Copilot Data Without User Interaction". 12.06.2025. https://thehackernews.com/2025/06/zero-click-ai-vulnerability-exposes.html · Microsoft Security Response Center: https://msrc.microsoft.com/update-guide/vulnerability/CVE-2025-32711

**[Q44]** TechRepublic: „First Known Zero-Click AI Exploit: Microsoft 365 Copilot's 'EchoLeak' Flaw". 13.06.2025. https://www.techrepublic.com/article/news-microsoft-365-copilot-flaw-echoleak/

**[Q45]** BSI / AISI Deutschland: „Aktuelle KI-Sicherheitsthemen 08/2026". Aktualisiert 07.09.2026. https://www.bsi.bund.de/DE/Themen/Unternehmen-und-Organisationen/Informationen-und-Empfehlungen/AISI/Blogeintraege/AISI-News_2026-08.html

**[Q46]** AI Business: „Panic Rises in Legal Industry Due to Anthropic's AI Plugins". 04.02.2026. https://aibusiness.com/agentic-ai/panic-rises-in-legal-industry-due-to-anthropic-s-ai-plugins

**[Q47]** Legal.io: „Anthropic's Claude Legal Plugin: One Month On, the Market Fallout and What It Means for Legal Teams". ca. März 2026. https://www.legal.io/blog/5798487/Anthropic-s-Claude-Legal-Plugin-One-Month-On-the-Market-Fallout-and-What-It-Means-for-Legal-Teams

**[Q48]** Morningstar: „Thomson Reuters, RELX, and Wolters Stocks Crushed After Anthropic Debuts Claude Legal Plug-In". 04.02.2026. https://www.morningstar.com/stocks/reuters-relx-wolters-stocks-crushed-after-anthropic-debuts-claude-legal-plug-in

**[Q49]** Wikipedia (Sekundärquelle): „OpenClaw". Abgerufen 01.10.2026. https://en.wikipedia.org/wiki/OpenClaw

**[Q50]** Nous Research: Repository „hermes-agent" (GitHub). Abgerufen 01.10.2026. https://github.com/NousResearch/hermes-agent · Übersichten: innFactory, ca. September 2026, https://innfactory.ai/en/ai-harness/hermes-agent/ ; jimmysong.io, o. D., https://jimmysong.io/ai/hermes-agent/

**[Q51]** arXiv 2605.22794: „MOSS: Self-Evolution through Source-Level Rewriting in Autonomous Agent Systems" (Literaturverzeichnis mit Beschreibung von hermes-agent-self-evolution). Mai 2026. https://arxiv.org/pdf/2605.22794

**[Q52]** Yutori: „OSWorld-Verified Leaderboard" (nach der offiziellen OSWorld-Tabelle). Stand 07.08.2026. https://yutori.com/leaderboards/osworld-verified.md

**[Q53]** BenchLM: „OSWorld-Verified". Stand 22.08.2026. https://www.benchlm.ai/benchmarks/osworld-verified

**[Q54]** Benchmarking Agents: „OSWorld: Computer-Use Agents on Real Operating Systems". 2026. https://benchmarkingagents.com/osworld/

**[Q55]** Steel.dev: OSWorld-Leaderboard mit Methodikhinweisen. o. D. https://leaderboard.steel.dev/leaderboards/osworld.md

**[Q56]** Scale AI / Center for AI Safety: „Remote Labor Index". Oktober 2025. https://scale.com/blog/rli · Paper: https://arxiv.org/html/2510.26787v1

**[Q57]** Inbenta (AI This Week): Bericht über die RLI-Aktualisierung des Center for AI Safety. 09.07.2026. https://www.inbenta.com/ai-this-week/ai-agents-now-automate-1-in-6-freelance-jobs-as-fable-5-shatters-cais-remote-labor-index-records

**[Q58]** HCAMag: „Your AI agent isn't as capable as you think, research finds". 2026. https://www.hcamag.com/us/specialization/hr-technology/your-ai-agent-isnt-as-capable-as-you-think-research-finds/579143

**[Q59]** My Legal Academy: „What Is OpenClaw? Complete Guide for Law Firms". ca. August 2026. https://mylegalacademy.com/kb/what-is-openclaw-law-firm-guide

**[Q60]** Blink: „OpenClaw for Lawyers: AI Legal Automation Guide 2026". ca. März 2026. https://blink.new/blog/openclaw-for-lawyers-legal-automation-2026

**[Q61]** Helen's Legal AI Lab: „OpenClaw Law LLP". ca. Juni 2026. https://helenlab.com/openclawlaw/

**[Q62]** Bloomberg Law: „OpenClaw Raises Questions on AI Agents Acting as Trustees" (Gastbeitrag). ca. März 2026. https://news.bloomberglaw.com/legal-exchange-insights-and-commentary/openclaw-raises-questions-on-ai-agents-acting-as-trustees

**[Q63]** Blockchain.news: „Harvey AI Hits 25,000 Custom Workflows as Legal Tech Automation Surges". 12.02.2026. https://blockchain.news/news/harvey-ai-25000-workflows-legal-automation

**[Q64]** bundesAPI: „Handelsregister API" (GitHub). o. D. https://github.com/bundesAPI/handelsregister

**[Q65]** Glama: „handelsregister-mcp" (Open-Source-MCP-Server). o. D. https://glama.ai/mcp/servers/rhxm6glg2r

**[Q66]** KI-Syndikat: Toolprofil „beck-online". Stand Juni 2026. https://www.ki-syndikat.de/tools/beck-online/

**[Q67]** Bundesrechtsanwaltskammer: „KI in der juristischen Praxis – Anwendungsfälle, Tools, Prompt-Baukasten" (Praxisdokument zur Podcast-Folge vom 13.03.2026). März 2026. https://www.brak.de/fileadmin/Newsroom/2026-KI_in_der_juristischen_Praxis-Paper.pdf

**[Q68]** Reco: „OpenClaw: The AI Agent Security Crisis Unfolding Right Now". ca. März 2026. https://www.reco.ai/blog/openclaw-the-ai-agent-security-crisis-unfolding-right-now

**[Q69]** Conscia: „The OpenClaw security crisis". ca. Februar 2026. https://conscia.com/blog/the-openclaw-security-crisis/

**[Q70]** Immersive Labs: „OpenClaw: What you need to know before it claws its way into your organization". ca. März 2026. https://www.immersivelabs.com/resources/c7-blog/openclaw-what-you-need-to-know-before-it-claws-its-way-into-your-organization

**[Q71]** arXiv 2602.20867: „SoK: Agentic Skills – Beyond Tool Use in LLM Agents". Februar 2026. https://arxiv.org/pdf/2602.20867

**[Q72]** BSI: Cybersicherheitswarnung „Indirect Prompt Injections – Intrinsic Vulnerability in Application-Integrated AI Language Models". 18.07.2023 (englische Fassung 21.07.2023). https://www.bsi.bund.de/SharedDocs/Cybersicherheitswarnungen/EN/2023/2023-249034-1032.pdf

**[Q73]** Mimikama: „Das BSI warnt vor manipulierenden Prompts". 2023. https://www.mimikama.org/?p=318396

**[Q74]** BSI: Themenseite „Künstliche Intelligenz" (mit Hinweis auf „Basisschutz gegen Indirect Prompt Injection in dokumentbasierten LLM-Chats", 2026). Abgerufen 01.10.2026. https://www.bsi.bund.de/DE/Themen/Unternehmen-und-Organisationen/Informationen-und-Empfehlungen/Kuenstliche-Intelligenz/kuenstliche-intelligenz_node.html

**[Q75]** OWASP GenAI Security Project: „OWASP Top 10 for Agentic Applications for 2026". 09.12.2025. https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications-for-2026

**[Q76]** Cloud Security Alliance: „OWASP's 2026 LLM Top 10 and New Agent Control Standard". 04.09.2026. https://labs.cloudsecurityalliance.org/research/csa-research-note-owasp-genai-top10-2026-agent-control-stand/ · Kategorienübersicht (u. a. ASI04 Lieferkette): Protectt.ai, o. D., https://protectt.ai/blog/owasp-top-10-agentic-applications-2026

**[Q77]** IT-Dock: „BSI entwickelt Prüfanforderungen für KI-Agenten" (Projekt PRAKI). September 2026. https://it-dock.de/blog/news/bsi-ki-agenten-sicherheit/

**[Q78]** Elektronikpraxis: „Wenn Zieltreue zum Sicherheitsrisiko wird: BSI warnt vor KI-Agenten". ca. Juli 2026 (zum BSI-Beitrag vom 24.07.2026). https://www.elektronikpraxis.de/wenn-zieltreue-zum-sicherheitsrisiko-wird-bsi-warnt-vor-ki-agenten-a-af193beaa7e9e42b650e42baa8bf268e/

**[Q79]** ICLR 2026: „Your Agent May Misevolve: Emergent Risks in Self-evolving LLM Agents" (arXiv-Fassung 30.09.2025). 2026. https://proceedings.iclr.cc/paper_files/paper/2026/hash/a24cd16bc361afa78e57d31d34f3d936-Abstract-Conference.html

**[Q80]** arXiv 2603.11619: „Taming OpenClaw: Security Analysis and Mitigation of Autonomous LLM Agent Threats". März 2026. https://arxiv.org/pdf/2603.11619

**[Q81]** ISO: „ISO/IEC 19510:2013 – Object Management Group Business Process Model and Notation". Juli 2013, 2022 bestätigt. https://www.iso.org/standard/62652.html

**[Q82]** rywalker.com: „Anthropic Skills" (Übersicht). ca. Juni 2026. https://rywalker.com/research/anthropic-skills

**[Q83]** OpenAPI Initiative: „Arazzo Specification" (GitHub). o. D. https://github.com/OAI/Arazzo-Specification

**[Q84]** Swagger (SmartBear): „The Arazzo Specification – A Deep Dive". 2025. https://swagger.io/blog/the-arazzo-specification-a-deep-dive/

**[Q85]** Oracle: „Introducing Open Agent Specification". 2025. https://blogs.oracle.com/ai-and-datascience/post/introducing-open-agent-specification · Technischer Bericht arXiv 2510.04173, Oktober 2025, https://arxiv.org/html/2510.04173v3

**[Q86]** Law Insider: „Explore All 50+ AI Playbooks Now Available in SimpleAI". o. D. https://www.lawinsider.com/resources/articles/3996

**[Q87]** jura.cc: „KI-Fehlzitate vor Gericht" (zu LG Frankfurt a. M., Beschl. v. 25.09.2025, 2-13 S 56/24). ca. September 2025. https://www.jura.cc/rechtstipps/ki-fehlzitate-vor-gericht-was-anwaeltinnen-und-anwaelte-jetzt-wissen-muessen/

**[Q88]** Legal Tribune Online: „Künstliche Intelligenz: Verschlafen Anwälte das neue Zeitalter?" (Gastbeitrag). 23.04.2026. https://www.lto.de/recht/juristen/b/kuenstliche-intelligenz-anwaltsberuf-berufsbild-schlafen-die-anwaelte
