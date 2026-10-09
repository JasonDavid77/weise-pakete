# Agentisches Rechtsabteilungs-Werkzeug einer Wirtschaftskanzlei: Wo die These „nur Software" trägt und wo nicht (Stand: 1. Oktober 2026)

**Die These trägt nur für den reinen Softwarebetrieb ohne Bezug zum Einzelfall. Sobald die Kanzlei für ein bestimmtes Unternehmen Arbeitsanleitungen schreibt, Agenten auf dessen konkrete Anfragen ansetzt und das System laufend nachsteuert, ist sie mit hoher Wahrscheinlichkeit selbst rechtsberatend tätig, und es greifen Anwaltsvertrag, BRAO-Pflichten und Anwaltshaftung.** Hinzu kommen eigene, von der Anwaltseigenschaft unabhängige Pflichtenkreise: Die Kanzlei ist Anbieterin nach der KI-Verordnung, wird ab dem 9. Dezember 2026 Herstellerin im Sinne der neuen Produkthaftung und ist datenschutzrechtlich mindestens Auftragsverarbeiterin.

## TL;DR

- **RDG und Berufsrecht:** Der BGH hat Smartlaw (Urteil vom 9.9.2021 – I ZR 113/20) freigegeben, weil der Generator auf typisierten Fällen beruht und kein konkreter Sachverhalt geprüft wird. Ein Werkzeug, das auf mandantenspezifischen Arbeitsanleitungen beruht und konkrete Anfragen bearbeitet, liegt deutlich näher an der „konkreten fremden Angelegenheit". Die Kanzlei darf zwar Rechtsdienstleistungen erbringen, das eigentliche Risiko liegt woanders: Durch die Einordnung als Rechtsdienstleistung greifen Anwaltshaftung, die Pflichten nach §§ 43a, 43e BRAO, § 203 StGB, die Regeln zu Interessenkonflikten und das Versicherungsrecht. Unternehmensjuristen ohne Zulassung, die das Werkzeug in eigenen Angelegenheiten des Arbeitgebers nutzen, sind vom RDG nicht berührt.
- **KI-Verordnung:** Die Kanzlei ist Anbieterin (Art. 3 Nr. 3), das Unternehmen Betreiber (Art. 3 Nr. 4). Seit dem 2.8.2026 gelten die Transparenzpflichten nach Art. 50 und die abgeschwächte Pflicht zur KI-Kompetenz nach Art. 4 in der Fassung der Verordnung (EU) 2026/1744. Diese ist seit dem 27.7.2026 in Kraft und verschiebt die Hochrisiko-Pflichten auf den 2.12.2027 (Anhang III) bzw. den 2.8.2028 (Anhang I). Die Rechtsabteilung ist regelmäßig kein Hochrisiko-Bereich. Das kann sich ändern, wenn das Werkzeug in Personalentscheidungen eingesetzt wird.
- **Haftung, Versicherung, Datenschutz:** Die Berufshaftpflicht nach § 51 BRAO deckt Programmierfehler typischerweise nicht. Bei Software droht außerdem die Serienschadenklausel. Ein eigener IT-Haftpflichtschutz ist daher Pflichtprogramm. Die neue Produkthaftung (RL (EU) 2024/2853, deutscher RegE BT-Drs. 21/4297) erfasst Software, ersetzt aber nur Schäden natürlicher Personen und keine reinen Vermögensschäden von Unternehmen. Im Datenschutz entscheidet die Ausgestaltung über die Rolle: Auftragsverarbeiter, eigener Verantwortlicher oder gemeinsam Verantwortlicher. Der Daten-Teil des Digital Omnibus (DSGVO-Änderungen) ist im Oktober 2026 **nicht** verabschiedet.

---

## 1. Kurzfassung

Die These trägt, soweit die Kanzlei nur eine generische, mandatsneutrale Software bereitstellt und die Unternehmensjuristen die Ergebnisse eigenverantwortlich in eigenen Angelegenheiten des Arbeitgebers verwenden. Sie trägt nicht, sobald die Kanzlei unternehmensspezifische Arbeitsanleitungen verfasst oder das System auf konkrete Fälle hin nachsteuert. Dann liegt nach dem Maßstab des BGH-Smartlaw-Urteils voraussichtlich eine Rechtsdienstleistung der Kanzlei vor, und Anwaltshaftung, Verschwiegenheit, Konfliktprüfung und Versicherungspflichten greifen. Unabhängig davon trifft die Kanzlei als Anbieterin die KI-Verordnung (u. a. Art. 4, Art. 50, seit 2.8.2026 anwendbar). Als Softwareherstellerin unterliegt sie ab dem 9.12.2026 der neuen Produkthaftung, und datenschutzrechtlich braucht sie mindestens einen Vertrag nach Art. 28 DSGVO samt § 43e-BRAO-Vereinbarung. „Keine besonderen Probleme" ist deshalb falsch: Die Probleme sind beherrschbar, müssen aber vertraglich, organisatorisch und versicherungsseitig gezielt gelöst werden.

---

## 2. Befunde

*Kennzeichnung: **[GR]** = geltendes Recht / Rechtsprechung; **[hM]** = herrschende bzw. überwiegende Meinung; **[EM]** = Einzel- oder Mindermeinung; **[offen]** = ungeklärt.*

### 2.1 Rechtsdienstleistungsgesetz

**a) Maßstab [GR].** Nach § 2 Abs. 1 RDG ist Rechtsdienstleistung „jede Tätigkeit in konkreten fremden Angelegenheiten, sobald sie eine rechtliche Prüfung des Einzelfalls erfordert".\[1\]\[2\] Nicht erfasst ist nach § 2 Abs. 3 Nr. 6 RDG die Erledigung von Rechtsangelegenheiten innerhalb verbundener Unternehmen (§ 15 AktG).\[3\] Selbständige außergerichtliche Rechtsdienstleistungen sind nur zulässig, soweit ein Gesetz sie erlaubt (§ 3 RDG).\[4\]\[5\] Für Rechtsanwälte und anwaltliche Berufsausübungsgesellschaften ergibt sich die Erlaubnis aus der BRAO.

**b) BGH Smartlaw [GR].** Mit Urteil vom 9.9.2021 – I ZR 113/20 (Vertragsdokumentengenerator) hat der BGH die Unterlassungsklage der Hanseatischen Rechtsanwaltskammer gegen Wolters Kluwer abgewiesen.\[6\]\[7\]\[8\] Die Leitlinien:
- Eine „Tätigkeit" liegt auch beim Einsatz von Software vor.\[7\] Maßgeblich sind Programmierung und Bereitstellung des Generators, die technischen Mittel sind unerheblich.\[9\]
- Es fehlt aber an einer **konkreten** fremden Angelegenheit. Die Klauseln wurden „im Vorgriff" auf typisierte Antworten entwickelt, und die Generierung erfolgt nicht auf Grundlage eines der Beklagten unterbreiteten konkreten Sachverhalts. Das Werkzeug ist insofern einem Formularhandbuch vergleichbar.\[10\]\[11\]\[12\]
- Für den Nutzer ist erkennbar, dass keine Prüfung seines individuellen Falls stattfindet.\[13\]
- Vorinstanzen: Das LG Köln (Urteil vom 8.10.2019 – 33 O 35/19) hatte der Kammer noch recht gegeben; das OLG Köln (Urteil vom 19.6.2020 – 6 U 263/19, AnwBl Online 2020, 404) änderte dieses Urteil ab, wobei beide Aktenzeichen durch BRAK-News und Anwaltsblatt bestätigt sind. Das Werbeverbot („Rechtsdokumente in Anwaltsqualität", „Günstiger und schneller als der Anwalt") wurde laut MIR 2020, Dok. 051 rechtskräftig, weil die Berufung insoweit zurückgenommen worden war.

**c) Übertragung auf das agentische Werkzeug [offen; eigene Bewertung].** Drei Merkmale unterscheiden das Modell deutlich von Smartlaw:
1. **Mandantenspezifische Arbeitsanleitungen.** Die Kanzlei schreibt Prüfprogramme für ein bestimmtes Unternehmen, etwa für dessen Vertragstypen, Risikoappetit und Eskalationsschwellen. Das ist bereits für sich genommen Rechtsberatung in dessen Angelegenheiten, also anwaltliche Tätigkeit und Gegenstand eines Anwaltsvertrags.
2. **Bearbeitung konkreter Anfragen.** Die Agenten verarbeiten keine typisierten Multiple-Choice-Antworten, sondern freie Sachverhalte und erzeugen dazu Einzelfallausgaben.\[14\] Damit fällt das Smartlaw-Argument „kein konkreter Sachverhalt" weitgehend weg.
3. **Zurechnung.** Das OLG Hamm hat mit Urteil vom 12.5.2026 – 4 UKl 3/25 einer Schönheitsklinik die erfundenen Aussagen ihres KI-Chatbots als eigene geschäftliche Handlung im Sinne des § 2 Abs. 1 Nr. 2 UWG zugerechnet. Der Chatbot sei ein technisches Hilfsmittel, über das der Betreiber hinreichende Steuergewalt besitze.\[9\]\[15\] Dem stehe nicht entgegen, dass er „gänzlich ohne menschliches Zutun" antworte. Verbraucher vertrauten zudem „in besonderer Weise" auf maschinelle Antworten. Das ist ein Wettbewerbsurteil, **kein RDG-Urteil**, und es ist nicht rechtskräftig, weil die Revision zugelassen wurde.\[16\]\[17\] Remmertz (legal-tech-verzeichnis.de, 10.6.2026) überträgt die Zurechnungsgrundsätze auf die „Tätigkeit" nach § 2 Abs. 1 RDG\[9\] **[EM, aber einflussreich: Vorsitzender des BRAK-Ausschusses RDG]**.\[9\]

**Gegenposition [EM].** Ein im Anwaltsblatt veröffentlichter Beitrag („Zukunft des Rechtsdienstleistungsrechts im Zeitalter von Legal Tech und KI") meint, beim KI-Rechtsrat sei nach geltendem Recht „keines der Tatbestandsmerkmale des § 2 Abs. 1 RDG … sicher erfüllt". Begründet wird das damit, dass ein Sprachmodell keine „rechtliche Prüfung des Einzelfalls" leiste, sondern Wahrscheinlichkeiten berechne, und dass das RDG „kein spezielles Produkthaftungsgesetz" sei.\[14\] In diese Richtung argumentiert auch Hartung.\[18\] Zur Rechtsberatung durch KI-Chatbots gibt es **keine** höchstrichterliche Entscheidung,\[9\] und eine RDG-Entscheidung gegen einen KI-Anbieter konnte ich für 2023–2026 nicht finden.\[9\]\[17\]

**Ergebnis zu (c).** Für die Kanzlei ist die Erlaubnisfrage zweitrangig, weil sie als Anwaltskanzlei befugt ist. Entscheidend ist die **Folgefrage**: Wer als Kanzlei für einen bestimmten Mandanten fallbezogen tätig wird, kann sich nicht auf die Rolle des Softwarelieferanten zurückziehen. Wahrscheinlicher ist ein gemischter Vertrag aus SaaS-Lizenz und Anwaltsdienstvertrag (§§ 611, 675 BGB) mit anwaltlichem Pflichtenprogramm. Die Kontrollpunkte beim Unternehmen ändern daran wenig. Sie sind ein Mitverschuldens- und Sorgfaltsargument, beseitigen aber nicht die eigene Tätigkeit der Kanzlei.

**Wichtige Falle.** Würde das Werkzeug zur Haftungsvermeidung in eine nicht-anwaltliche Software-GmbH ausgelagert, die dennoch mandantenspezifische Arbeitsanleitungen liefert, drohte dieser GmbH ein Verstoß gegen § 3 RDG. Ein solcher Verstoß ist nach § 3a UWG als Marktverhaltensregel abmahnfähig, und Verträge können nach § 134 BGB nichtig sein.\[7\] Das Smartlaw-Verfahren zeigt, dass Rechtsanwaltskammern solche Modelle gerichtlich angreifen.\[19\]

**d) Andere Legal-Tech-Rechtsprechung [GR].** Die Inkasso-Entscheidungen BGH 27.11.2019 – VIII ZR 285/18 (wenigermiete.de), BGH 13.7.2021 – II ZR 84/20 (Airdeal) und BGH 13.6.2022 – VIa ZR 418/21 (financialright) gingen sämtlich **zugunsten** der Anbieter aus.\[20\]\[21\]\[22\] Sie betreffen jedoch die Inkassobefugnis nach § 2 Abs. 2 RDG und taugen für das hier geprüfte Modell nur als Hinweis auf eine eher liberale Linie des BGH. Bei Überschreitung der Befugnis droht die Nichtigkeit nach § 134 BGB i. V. m. § 3 RDG.\[4\]\[23\]

**e) Gesetzgebung [GR].** Ein KI-spezifischer RDG-Entwurf existiert nicht. Der Regierungsentwurf zur Neuordnung aufsichtsrechtlicher Verfahren der rechtsberatenden Berufe (BT-Drs. 21/4298 vom 25.2.2026; 1. Lesung 25.3.2026, Anhörung 22.4.2026) enthält nach meiner Recherche keine KI-Regel.\[24\]\[25\]\[26\] Der Legal Tech Verband fordert eine Klarstellung, dass KI-gestützte Systeme keine unbefugte Rechtsberatung darstellen.\[27\] Beck-aktuell hält am 18.3.2026 fest, zum Themenkomplex KI und RDG höre man von BRAK und DAV „wenig bis gar nichts".\[28\]

**f) Unternehmensjuristen ohne Zulassung [hM].** Wer den eigenen Arbeitgeber in dessen Rechtsangelegenheiten berät, wird nicht in einer *fremden* Angelegenheit tätig. Das RDG ist dann schon tatbestandlich nicht einschlägig.\[29\] Konzernangelegenheiten sind über § 2 Abs. 3 Nr. 6 RDG ausgenommen.\[30\] Ob die Juristen dabei ein KI-Werkzeug einsetzen, ändert daran nichts. **Grenze:** Beantwortet die Rechtsabteilung über das Werkzeug Anfragen von Kunden, Lieferanten oder nicht verbundenen Gesellschaften, liegt eine fremde Angelegenheit vor, und es bedarf einer Erlaubnis.\[31\]

**g) Syndikusrechtsanwälte [GR].** Ihre Befugnis beschränkt sich nach § 46 Abs. 5 BRAO auf Rechtsangelegenheiten des Arbeitgebers, einschließlich verbundener Unternehmen.\[32\] Die Beratung von Kunden des Arbeitgebers steht der Zulassung entgegen, selbst wenn sie nur vereinzelt erfolgt (BGH, Urteil vom 22.6.2020 – AnwZ (Brfg) 23/19; zuvor BGH, Oktober 2018 – AnwZ (Brfg) 58/17).\[33\]\[34\] Das BVerfG hat das Drittberatungsverbot gebilligt und die Verfassungsbeschwerde gegen BGH 5.10.2020 – AnwZ (Brfg) 43/18 nicht zur Entscheidung angenommen (Kammerbeschluss des Ersten Senats vom 27.4.2021 – 1 BvR 2649/20, AnwBl Online 2021, 700; die Kammer wird in den Quellen unterschiedlich als 1. bzw. 3. Kammer bezeichnet); eine Beschränkung von Art. 12 Abs. 1 GG sieht das Gericht laut BRAK, Nachrichten aus Berlin 13/2021, darin nicht. Für die interne Nutzung des Werkzeugs bestehen danach keine RDG-Probleme. Über § 46c Abs. 1 BRAO unterliegen Syndikusrechtsanwälte aber dem anwaltlichen Berufsrecht, also auch §§ 43a, 43e BRAO (siehe 2.2).\[35\]

### 2.2 Berufsrecht (BRAO, BORA) und Verschwiegenheit

**a) Technologieneutralität [hM].** Die BRAK-„Hinweise zum Einsatz von künstlicher Intelligenz" (Stand Dezember 2024, Verfasser Remmertz) halten fest: BRAO und BORA sind technologieneutral. KI darf nur unterstützen. Erforderlich ist eine „eigenverantwortliche Überprüfung und Endkontrolle der KI-Ergebnisse" (§ 43 BRAO, § 613 BGB), und die Sorgfaltsanforderungen steigen mit dem Grad der Automatisierung.\[36\]\[37\]\[38\]\[39\] Eine allgemeine berufsrechtliche Pflicht, Mandanten über den KI-Einsatz zu informieren, sieht die BRAK nicht.\[38\]\[40\] Die DAV-Initiativ-Stellungnahme Nr. 32/2025 (Juli 2025) hält die Vorgaben für „durchweg bewältigbar" und „beherrschbar".\[41\] **Folge für das Modell:** Die festen Kontrollpunkte entsprechen der berufsrechtlichen Erwartung, und zwar sowohl bei Syndikusrechtsanwälten des Unternehmens als auch bei der Kanzlei, soweit sie selbst anwaltlich tätig wird.

**b) Kanzlei als IT-Dienstleisterin des Syndikus: § 43e BRAO [GR].** Gibt ein Syndikusrechtsanwalt der Kanzlei als Betreiberin Zugang zu Tatsachen, die der Verschwiegenheit nach § 43a Abs. 2 BRAO unterliegen, muss er Folgendes sicherstellen:\[42\]
- Die Offenlegung geht nur so weit, wie die Dienstleistung es **erfordert** (§ 43e Abs. 1).\[43\]\[44\]
- Der Dienstleister ist sorgfältig auszuwählen, und die Zusammenarbeit ist bei Defiziten unverzüglich zu beenden (Abs. 2).\[44\]
- Der Vertrag bedarf der **Textform** und muss die Verpflichtung zur Verschwiegenheit unter Belehrung über die strafrechtlichen Folgen, die Kenntnisnahme nur im erforderlichen Umfang und eine Regelung zu Subunternehmern samt deren Verpflichtung in Textform enthalten (Abs. 3).\[44\]
- Bei Leistungserbringung im Ausland muss ein vergleichbarer Geheimnisschutz bestehen (Abs. 4).\[45\]

Zu den Subunternehmern gehören beim agentischen Werkzeug **insbesondere der LLM-API-Anbieter und der Cloud-Hoster**. Nach § 43e Abs. 3 Satz 2 BRAO entfällt das Erfordernis nach Satz 2, soweit der Dienstleister „hinsichtlich der zu erbringenden Dienstleistung gesetzlich zur Verschwiegenheit verpflichtet ist".\[45\] Ob das für eine Kanzlei gilt, die *als Softwarebetreiberin* tätig wird, ist **[offen]**. Empfehlung: einen vollständigen § 43e-Vertrag abschließen.

**c) Strafrecht: § 203 StGB [GR].** Rechtsanwälte und Syndikusrechtsanwälte gehören zu den Geheimnisträgern (§ 203 Abs. 1 Nr. 3 StGB).\[42\] Die Offenbarung an „mitwirkende Personen" ist nach § 203 Abs. 3 Satz 2 StGB nur befugt, soweit sie erforderlich ist.\[46\] Die Mitarbeiter der Kanzlei und ihrer Subunternehmer werden selbst strafrechtlich verpflichtet (§ 203 Abs. 4 StGB). Ein Geheimnisträger macht sich nach § 203 Abs. 4 Satz 2 Nr. 1 StGB strafbar, wenn er nicht dafür sorgt, dass der Mitwirkende zur Geheimhaltung verpflichtet wurde. Bei Unternehmensjuristen **ohne** Zulassung greift § 203 StGB insoweit nicht. Vertraulichkeit ist dann über Vertrag, Arbeitsrecht und GeschGehG zu sichern.

**d) Pflichten der Kanzlei selbst [GR/offen].**
- **Verschwiegenheit:** Was die Kanzlei „in Ausübung ihres Berufes" erfährt, unterliegt § 43a Abs. 2 BRAO. Bei mandatsbezogener Pflege der Arbeitsanleitungen ist das unproblematisch der Fall. Bei rein technischem Betrieb ist es **[offen]**. Das spricht ebenfalls für eine klare Mandatsstruktur.
- **Interessenkonflikte (§ 43a Abs. 4 BRAO, § 3 BORA):** Werden die Arbeitsanleitungen als anwaltliche Leistung erstellt, ist vor Vertragsschluss und laufend zu prüfen, ob die Kanzlei Gegner des Unternehmens vertritt. Zudem braucht es Informationsbarrieren gegenüber Kanzleiteams, die systemseitig Zugriff auf Unternehmensdaten hätten.
- **Werbung (§ 43b BRAO, § 5 UWG):** Aussagen wie „anwaltlich geprüft" oder „Anwaltsqualität" sind heikel. Das LG Köln hat Smartlaw 2019 auch wegen irreführender Werbung verurteilt; dieses Werbeverbot wurde laut MIR 2020, Dok. 051 rechtskräftig, weil die Berufung insoweit zurückgenommen worden war. Die Werbeaussagen sollten mit der tatsächlichen Leistung übereinstimmen.
- **Gewerbliche Tätigkeit der Berufsausübungsgesellschaft [offen].** Ob die Lizenzierung von Software als eigenständiges Geschäft vom Gegenstand einer anwaltlichen Berufsausübungsgesellschaft gedeckt ist, habe ich nicht abschließend verifiziert. Das gilt besonders nach der BRAO-Reform 2022 (§§ 59b ff. BRAO). Die Frage sollte mit der zuständigen Rechtsanwaltskammer geklärt werden.

**e) Beschlagnahmeschutz [offen].** Hostet die Kanzlei die Rechtsabteilungsdaten des Unternehmens als bloße IT-Dienstleisterin, ist zweifelhaft, ob diese Daten als ihr im Mandat „anvertraut" gelten und damit den Schutz der §§ 53, 97 StPO genießen. Für Syndikusrechtsanwälte ist das Zeugnisverweigerungsrecht nach § 53 Abs. 1 Satz 1 Nr. 3 StPO zudem eingeschränkt (Wortlaut hier nicht gesondert geprüft). Für interne Untersuchungen ist das ein erhebliches praktisches Risiko.

### 2.3 KI-Verordnung (Verordnung (EU) 2024/1689 i. d. F. der Verordnung (EU) 2026/1744)

**a) Verfahrensstand Digital Omnibus zur KI [GR].** Die Kommission legte den Vorschlag am 19.11.2025 vor. Die politische Einigung im Trilog erfolgte am 7.5.2026, nachdem ein erster Trilog am 28.4.2026 gescheitert war.\[47\]\[48\] Das Europäische Parlament stimmte am 16.6.2026 zu, der Rat am 29. bzw. 30.6.2026 (die Quellen nennen unterschiedliche Daten).\[49\]\[50\] Die Verordnung (EU) 2026/1744 vom 8.7.2026 wurde am 24.7.2026 im ABl. L verkündet und ist **seit dem 27.7.2026 in Kraft**.\[51\]\[52\]\[53\]

**b) Zeitplan nach Art. 113 in der geänderten Fassung [GR].**

| Pflicht | Gilt ab | Quelle/Hinweis |
|---|---|---|
| Verbote (Art. 5), KI-Kompetenz (Art. 4) | 2.2.2025 | Art. 4 seit 27.7.2026 neu gefasst |
| GPAI-Modellpflichten (Art. 51 ff.) | 2.8.2025 | unverändert |\[54\]
| Allgemeine Geltung, Transparenz (Art. 50 Abs. 1, 3, 4) | **2.8.2026** | unverändert |\[48\]
| Kennzeichnung nach Art. 50 Abs. 2 für vor dem 2.8.2026 in Verkehr gebrachte Systeme | 2.12.2026 | viermonatiger Übergang (ErwG 38 VO 2026/1744)\[53\] |\[49\]
| Neues Verbot (nicht einvernehmliche intime Inhalte/CSAM) | 2.12.2026 | laut Sekundärquelle |\[52\]\[55\]
| Hochrisiko Anhang III (eigenständig) | **2.12.2027** | statt 2.8.2026 (ErwG 40)\[53\] |
| Hochrisiko Anhang I (Produkte) | **2.8.2028** | statt 2.8.2027\[53\] |\[49\]

**c) Rollen [GR, Subsumtion eigene Bewertung].**
- **Kanzlei = Anbieterin** (Art. 3 Nr. 3): Sie entwickelt das System oder lässt es entwickeln und bringt es unter eigenem Namen in Verkehr bzw. stellt es bereit, wobei es auf Entgeltlichkeit nicht ankommt.\[56\] Nutzt sie ein fremdes Basismodell per API, bleibt dessen Hersteller GPAI-Modellanbieter. Die Kanzlei wird Anbieterin des darauf aufbauenden *Systems*.\[57\] GPAI-Modellanbieterin würde sie erst durch erhebliche eigene Modellveränderung, deren Schwellen hier nicht geprüft sind.
- **Unternehmen = Betreiber** (Art. 3 Nr. 4): Es verwendet das System in eigener Verantwortung.\[56\] Nutzt die Kanzlei das Werkzeug selbst im Mandat, ist sie zusätzlich Betreiberin.\[58\]
- **Rollenwechsel (Art. 25):** Er greift nur bei Hochrisiko-Systemen, etwa wenn das Unternehmen das System unter eigener Marke führt, wesentlich verändert oder seine Zweckbestimmung so ändert, dass es zum Hochrisiko-System wird.\[56\]\[59\]

**d) Hochrisiko? [hM, eigene Bewertung].** Anhang III Nr. 8 lit. a erfasst KI, die von oder im Auftrag von Justizbehörden (bzw. in der alternativen Streitbeilegung) zur Ermittlung und Auslegung von Sachverhalt und Recht eingesetzt wird. Eine Unternehmensrechtsabteilung fällt nicht darunter.\[60\] **Achtung:** Werden die Agenten für Personalentscheidungen eingesetzt, etwa zur Bewertung von Kündigungsfällen, zur Leistungsbeurteilung oder zur Aufgabenzuweisung, kommt Anhang III Nr. 4 (Beschäftigung) in Betracht. Dann wäre das Werkzeug ab dem 2.12.2027 ein Hochrisiko-System mit Anbieterpflichten nach Art. 16 ff. (Risikomanagement, Daten-Governance, technische Dokumentation, Logging, menschliche Aufsicht, Konformitätsbewertung, Registrierung) und Betreiberpflichten nach Art. 26. Die Zweckbestimmung sollte deshalb **vertraglich und technisch** solche Einsätze ausschließen.

**e) Pflichten im Nicht-Hochrisiko-Fall [GR].**
- **Art. 4 (n. F.):** Anbieter und Betreiber „ergreifen Maßnahmen, um die Entwicklung der KI-Kompetenz ihres Personals … zu unterstützen". Ein bestimmtes Kompetenzniveau muss nicht mehr garantiert werden.\[52\]\[53\] Die Pflicht trifft beide Seiten, also auch die Unternehmensjuristen als Betreiberpersonal.
- **Art. 50 Abs. 1 (Anbieter):** Systeme, die mit natürlichen Personen interagieren, müssen so gestaltet sein, dass die Personen erkennen, dass sie mit KI interagieren, sofern das nicht offensichtlich ist. Das betrifft etwa Mitarbeitende, die Anfragen an die Agenten richten.
- **Art. 50 Abs. 2 (Anbieter):** Synthetische Textausgaben sind maschinenlesbar zu kennzeichnen. Eine Ausnahme gilt u. a. für bloß unterstützende Standardbearbeitung. Für vor dem 2.8.2026 in Verkehr gebrachte Systeme gilt die Pflicht erst ab dem 2.12.2026.\[53\]
- **Art. 50 Abs. 4 (Betreiber):** Diese Pflicht betrifft KI-Texte zu Angelegenheiten von öffentlichem Interesse ohne redaktionelle Kontrolle\[61\] und ist für interne Rechtsarbeit regelmäßig nicht einschlägig.
- **Art. 4a (neu):** Er erlaubt ausnahmsweise die Verarbeitung besonderer Kategorien personenbezogener Daten zur Erkennung und Korrektur von Verzerrungen, unter engen Bedingungen und auch für Nicht-Hochrisiko-Systeme.\[62\] Art. 2 Abs. 7 stellt klar, dass die DSGVO im Übrigen unberührt bleibt.\[53\]
- **Sanktionen:** Verstöße gegen Art. 50 können nach Art. 99 Abs. 4 mit bis zu 15 Mio. € oder 3 % des weltweiten Jahresumsatzes geahndet werden.\[61\]

**f) Nationale Durchführung [GR].** Das KI-Marktüberwachungs- und Innovationsförderungsgesetz (KI-MIG) wurde vom Bundestag am 11.6.2026 beschlossen\[62\] (RegE BT-Drs. 21/4594, Ausschussfassung 21/6407); der Bundesrat befasste sich am 10.7.2026 damit.\[63\]\[64\]\[65\] Nach der Pressemitteilung der Bundesnetzagentur trat es am 29.7.2026 in Kraft.\[66\] Die **Bundesnetzagentur** ist zentrale Marktüberwachungs-, Anlauf- und Beschwerdestelle, bei ihr ist das KoKIVO eingerichtet.\[67\]

**g) Folge für die These.** Die KI-Verordnung behandelt das Werkzeug gerade *als Software*. Das bestätigt die These formal, löst aber eigene Anbieterpflichten aus, die bei „gewöhnlicher" Kanzleisoftware nicht bestehen.

### 2.4 Haftung

**a) Vertraglich gegenüber dem Unternehmen [GR/hM].**
- **Softwareteil:** Die Überlassung auf Zeit (SaaS/ASP) wird nach h. M. mietrechtlich eingeordnet (BGH, Urteil vom 15.11.2006 – XII ZR 120/04, ASP-Vertrag; hier nicht im Volltext geprüft). Die Folgen sind Mängelgewährleistung nach §§ 535 ff. BGB und für anfängliche Mängel die verschuldensunabhängige Garantiehaftung nach § 536a Abs. 1 Alt. 1 BGB, die im B2B-Bereich formularmäßig abbedungen werden kann und sollte. Die Verbraucherregeln der §§ 327 ff. BGB greifen nicht.
- **Arbeitsanleitungen und laufende Pflege:** Hier liegt ein Anwaltsdienstvertrag vor (§§ 611, 675 BGB) mit Haftung nach § 280 Abs. 1 BGB nach dem strengen Maßstab der Anwaltshaftung. Eine Begrenzung ist nach § 52 Abs. 1 BRAO möglich: durch Individualvereinbarung bis zur Mindestversicherungssumme, durch vorformulierte Bedingungen bei einfacher Fahrlässigkeit bis zum Vierfachen, jeweils bei entsprechender Versicherung.
- **Kontrollpunkte:** Prüfen die Unternehmensjuristen an festen Punkten, begründet ihr Prüfversäumnis Mitverschulden (§ 254 BGB). Es entlastet die Kanzlei aber nicht vollständig, wenn der Fehler in der von ihr verantworteten Arbeitsanleitung angelegt war.

**b) Außervertraglich [GR].**
- **§ 823 Abs. 1 BGB** schützt keine reinen Vermögensschäden, und das sind die typischen Schäden aus Rechtsfehlern. Daneben kommen § 823 Abs. 2 BGB i. V. m. Schutzgesetzen und § 826 BGB in Betracht.
- **UWG:** Fehlerhafte KI-Aussagen werden dem Betreiber als eigene geschäftliche Handlung zugerechnet (OLG Hamm 12.5.2026 – 4 UKl 3/25, nicht rechtskräftig).\[9\]\[15\]\[68\]
- **Neue Produkthaftung.** Die RL (EU) 2024/2853 vom 23.10.2024 ist bis zum **9.12.2026** umzusetzen.\[69\] Software gilt unabhängig von der Art ihrer Bereitstellung als Produkt, auch als SaaS und KI.\[70\]\[71\]\[72\]\[73\] Die Kanzlei wäre als Entwicklerin Herstellerin. Ersatzfähig sind aber nur Schäden **natürlicher Personen**:\[74\] Tod, Körper- und Gesundheitsschäden, Sachschäden an nicht ausschließlich beruflich genutzten Sachen sowie Vernichtung oder Beschädigung nicht beruflich genutzter Daten. Reine Vermögensschäden des Unternehmens fallen nicht darunter. Für ein B2B-Rechtswerkzeug ist das Risiko deshalb begrenzt, aber nicht null, etwa bei der Vernichtung privater Daten von Beschäftigten. Zudem gelten Offenlegungspflichten und Vermutungen zur Beweislast.\[71\]\[75\] Nach dem RegE haftet der Hersteller auch für fehlende Sicherheitsupdates, solange er die Kontrolle über das Produkt behält.\[72\]\[73\]
- **Deutsche Umsetzung:** Die Bundesregierung beschloss den Entwurf am 17.12.2025 (BR-Drs. 775/25, Stellungnahme des Bundesrats am 30.1.2026; BT-Drs. 21/4297 vom 25.2.2026). Die 1. Lesung fand am 4.3.2026 statt,\[76\]\[77\]\[78\]\[79\]\[80\] die Anhörung im Rechtsausschuss am 13.4.2026.\[81\]\[82\] **Zum Stand August 2026 standen nach Sekundärquellen die 2./3. Lesung und der zweite Durchgang im Bundesrat noch aus.\[82\] Eine Verabschiedung bis zum 1.10.2026 konnte ich nicht belegen.**\[83\] Geplantes Inkrafttreten ist der 9.12.2026.\[81\] Für vorher in Verkehr gebrachte Produkte bleibt das ProdHaftG 1989 anwendbar.\[76\]\[77\]\[80\] Wird die Frist verfehlt, gilt bis zur Verkündung das alte Recht,\[69\] denn eine Richtlinie wirkt zwischen Privaten nicht unmittelbar.
- **KI-Haftungsrichtlinie:** Die Kommission setzte sie mit dem Arbeitsprogramm 2025 (11.2.2025) auf die Rücknahmeliste. Die förmliche Rücknahme erfolgte nach einer Sekundärquelle im Oktober 2025.\[84\]\[85\] Sie entfällt also als zusätzliche Haftungsgrundlage.
- **Art. 82 DSGVO:** Bei Datenschutzverstößen kommt Schadensersatz auch für immaterielle Schäden in Betracht.

**c) Haftung der Unternehmensjuristen [hM].**
- **Angestellte, auch Syndikusrechtsanwälte im Innenverhältnis:** Es gelten die Grundsätze des innerbetrieblichen Schadensausgleichs (BAG GS, Beschluss vom 27.9.1994 – GS 1/89 (A)). Bei leichter Fahrlässigkeit haften sie nicht, bei mittlerer anteilig, bei grober Fahrlässigkeit und Vorsatz in der Regel voll. Wer an einem Kontrollpunkt KI-Ergebnisse ungeprüft freigibt, riskiert den Vorwurf grober Fahrlässigkeit. Die BRAK verlangt gerade eine *eigenverantwortliche* Endkontrolle.\[86\]
- **Organmitglieder (General Counsel im Vorstand oder in der Geschäftsführung):** Hier gilt die Organhaftung (§ 93 AktG, § 43 GmbHG). Relevant ist zudem die Auswahl- und Überwachungsverantwortung für das Werkzeug.
- **Syndikusrechtsanwälte und Versicherung:** Für ihre Syndikustätigkeit unterliegen sie nicht der Pflichtversicherung nach § 51 BRAO: Nach § 46a Abs. 4 Nr. 1 BRAO ist der Nachweis einer Berufshaftpflichtversicherung „nicht erforderlich", und nach § 46c Abs. 3 BRAO finden auf die Tätigkeit von Syndikusrechtsanwälten u. a. „die §§ 51 bis 55 keine Anwendung".

**d) Versicherbarkeit [hM/Praxis].**
- **§ 51 BRAO:** Pflicht-Vermögensschadenhaftpflicht mit 250.000 € Mindestversicherungssumme je Fall. Für Berufsausübungsgesellschaften mit Haftungsbeschränkung verlangt § 59o Abs. 1 BRAO „für jeden Versicherungsfall 2 500 000 Euro", bei höchstens zehn anwaltlich tätigen Personen 1 Mio. € (Abs. 2), ohne Haftungsbeschränkung 500.000 € (Abs. 3); die Jahreshöchstleistung beträgt mindestens das Vierfache.
- **Deckungsgrenzen:**
  - Gedeckt ist nur die *anwaltliche* Berufstätigkeit. Programmierfehler gehören nach Fachstimmen nicht dazu (Versicherungsmakler von Lauff & Bolz; Anwaltsblatt-Beitrag „Reicht die Berufshaftpflichtversicherung noch im Hinblick auf KI?").\[38\]\[87\]\[88\]
  - Ersatzansprüche wegen wissentlicher Pflichtverletzung können ausgeschlossen werden (§ 51 Abs. 3 Nr. 1 BRAO). Die ungeprüfte Übernahme von KI-Ergebnissen „legt den Vorwurf der wissentlichen Pflichtverletzung nah" (Anwaltsblatt).\[87\]\[89\]
  - Die **Serienschadenklausel** ist bei Software besonders gefährlich: Ein fehlerhafter Baustein führt zu vielen Schäden, die als ein Versicherungsfall gelten und nur einmal die Versicherungssumme auslösen (Anwaltsblatt, „Legal Tech und Serienschäden").\[90\]
  - Datenschutz- und Urheberrechtsverletzungen sind regelmäßig nicht gedeckt.\[91\]
- **Ergänzend nötig:** IT-/Technologie-Haftpflicht (Tech E&O) mit offener Vermögensschadendeckung, eine Cyberversicherung und gegebenenfalls ein Exzedent.\[87\]\[92\] Beim Unternehmen kommt D&O für die Organe hinzu. Spezifische KI-Ausschlüsse sind nach einer Anbieterquelle 2026 noch selten.\[93\] Das sollte mit dem Versicherer **vor Vertriebsstart schriftlich** geklärt werden.

### 2.5 Datenschutz (DSGVO)

**a) Rollen [GR/hM, offen im Einzelfall].**
- Das **Unternehmen** ist Verantwortlicher (Art. 4 Nr. 7) für die Verarbeitung der Daten von Beschäftigten, Vertragspartnern und Gegnern in seinen Rechtsangelegenheiten.
- Die **Kanzlei als Betreiberin der Plattform** ist Auftragsverarbeiterin (Art. 28) mit Vertrag nach Art. 28 Abs. 3 und genehmigten Unterauftragsverarbeitern nach Art. 28 Abs. 2 und 4, etwa LLM-Anbieter und Hoster. Diesen Vertrag sinnvollerweise mit der § 43e-BRAO-Vereinbarung kombinieren.
- **Spannung:** Soweit die Kanzlei *anwaltlich* tätig wird (Arbeitsanleitungen, Einzelfallsteuerung), ist sie eigenverantwortlich: Das DSK-Kurzpapier Nr. 13 (Stand 17.12.2018) sieht bei Rechtsanwälten „keine Auftragsverarbeitung, sondern die Inanspruchnahme fremder Fachleistungen bei einem eigenständig Verantwortlichen", und nach den BRAK-FAQ zur DS-GVO (19.12.2019) können Rechtsanwälte keine Auftragsverarbeiter sein, weil sie als Organe der Rechtspflege nicht weisungsgebunden sind. Das ergibt eine Doppelrolle, die vertraglich sauber getrennt werden muss.
- **Gemeinsame Verantwortlichkeit oder eigene Verantwortlichkeit:** Verwendet die Kanzlei Unternehmensdaten für eigene Zwecke, etwa zur mandantenübergreifenden Verbesserung oder zum Training der Agenten, droht gemeinsame Verantwortlichkeit (Art. 26) oder eigene Verantwortlichkeit mit eigener Rechtsgrundlage. Das sollte ohne ausdrückliche Vereinbarung ausgeschlossen werden.

**b) Rechtsgrundlagen [GR].** In Betracht kommen Art. 6 Abs. 1 lit. b, c, f DSGVO. Für Beschäftigtendaten ist die Rechtsgrundlage seit EuGH, Urteil vom 30.3.2023 – C-34/21, unsicher: Das Urteil betraf § 23 HDSIG, der wortgleich mit § 26 Abs. 1 Satz 1 BDSG ist. Empfehlung: Verarbeitungen direkt auf Art. 6 DSGVO stützen. In Rechtsabteilungen fallen häufig Gesundheitsdaten (Art. 9) und Daten über Straftaten (Art. 10) an, etwa in arbeitsrechtlichen Streitigkeiten und Compliance-Untersuchungen. Für sie gelten erhöhte Anforderungen, z. B. Art. 9 Abs. 2 lit. f (Rechtsansprüche).

**c) Automatisierte Entscheidungen (Art. 22) [GR].** Die festen Kontrollpunkte sprechen gegen eine „ausschließlich automatisierte" Entscheidung. Nach EuGH, Urteil vom 7.12.2023 – C-634/21 (SCHUFA), genügt jedoch schon ein maßgeblich prägendes maschinelles Ergebnis. Eine nur formale Abzeichnung schützt nicht. Die Kontrollen müssen deshalb echte inhaltliche Prüfungen sein und so dokumentiert werden.

**d) Weitere Pflichten [GR].** Dazu gehören:
- eine Datenschutz-Folgenabschätzung (Art. 35), die beim Einsatz neuer Technologie auf Beschäftigten- und Gegnerdaten regelmäßig naheliegt;
- Datenschutz durch Technikgestaltung (Art. 25) und Sicherheit der Verarbeitung (Art. 32);
- ein Löschkonzept, auch für Prompts, Logs und Agenten-Speicher;
- Informationspflichten (Art. 13/14), ein Verarbeitungsverzeichnis (Art. 30) und Garantien für Drittlandtransfers (Art. 44 ff.).

Der EuGH (Urteil vom 4.9.2025 – C-413/23 P, EDSB/SRB) bestätigt den **relativen Personenbezug**: Pseudonymisierte Daten können für einen Empfänger ohne Zuordnungsmittel nicht personenbezogen sein, bleiben es aber für den Verantwortlichen.\[94\]\[95\] Über Empfänger ist **bereits bei der Erhebung** zu informieren.\[96\] Für das Werkzeug heißt das: Eine Pseudonymisierung vor der Übergabe an den LLM-Anbieter kann dessen Rolle entschärfen, befreit Unternehmen und Kanzlei aber nicht von ihren Pflichten.

**e) Digital Omnibus, Daten-Teil (COM(2025) 837) [Verfahrensstand].** Er ist **im Oktober 2026 nicht verabschiedet**.\[50\]\[97\]
- Die gemeinsame Stellungnahme von EDSA und EDSB stammt vom 20.1.2026. Im Parlament (LIBE/ITRE) wurde im Juni 2026 ein Entwurf des Ausschussberichts vorgelegt.\[98\]
- Im Rat liegt ein Kompromisstext der irischen Präsidentschaft vor (Ratsdok. 12535/26), außerdem deutsche Formulierungsvorschläge (WK 11020/2026 ADD 4 vom 17.8.2026). Beide sind als LIMITE eingestuft und wurden am 21.9.2026 von noyb veröffentlicht.\[97\] Ich kenne sie nur aus Sekundärberichterstattung.
- Diskutiert werden u. a.:
  - eine **subjektive bzw. relative Definition personenbezogener Daten** in Art. 4 Nr. 1;\[97\]\[99\]\[100\]\[101\]
  - ein neuer Art. 88c (im Ratstext „88bis"), der die Verarbeitung für Entwicklung **und Betrieb** von KI-Systemen auf das berechtigte Interesse stützt, nach dem deutschen Vorschlag sogar als gesetzliche Vermutung;\[97\]\[100\]
  - ein Missbrauchseinwand gegen Auskunftsersuchen (Art. 12 Abs. 5);\[97\]
  - eine Meldefrist von 96 Stunden nur bei hohem Risiko.\[102\]\[103\]
- Ein Abschluss gilt frühestens Anfang 2027 als realistisch (Prognose einer Sekundärquelle).\[97\]

**Folge:** Für die hier behandelten Fragen gilt heute die **unveränderte DSGVO**. Ein künftiger Art. 88c würde den *Betrieb* des Werkzeugs rechtlich erleichtern, ist aber hoch umstritten und darf nicht in die Planung eingepreist werden.

---

## 3. Offene Rechtsfragen und Gegenpositionen

1. **„Tätigkeit" bei generativer KI (§ 2 Abs. 1 RDG).** Pro Zurechnung: OLG Hamm 12.5.2026 (UWG), Remmertz. Contra: der Anwaltsblatt-Beitrag (KI leiste keine „rechtliche Prüfung"), Hartung und der Legal Tech Verband. Ungeklärt ist auch, ob die Revision im Hamm-Verfahren eingelegt wurde.
2. **Konkretheit bei mandantenspezifischen Arbeitsanleitungen.** Ob das Smartlaw-Argument „Formularhandbuch" trägt, wenn die Kanzlei die Anleitungen für *ein* Unternehmen schreibt und laufend nachsteuert, ist ungeklärt. Nach meiner Einschätzung trägt es nicht. Die Gegenposition stellt darauf ab, dass die Kanzlei den Einzelfall nie sieht und die rechtliche Prüfung beim Unternehmensjuristen liegt.
3. **Verkehrserwartung und Disclaimer.** Der BGH stellte bei Smartlaw auf die erkennbare Erwartung des Nutzers ab.\[1\] Das OLG Hamm verneint einen Erfahrungssatz, dass Nutzer KI-Antworten misstrauen.\[9\]\[104\] Bei professionellen Nutzern wie einer Rechtsabteilung spricht mehr für die Erkennbarkeit. Im B2B-Kontext ist das ein Argument *für* die These.
4. **Reichweite von § 43e Abs. 3 Satz 2 BRAO** bei einer Kanzlei, die als Softwarebetreiberin tätig wird, sowie Beschlagnahme- und Zeugnisverweigerungsschutz für bei ihr gehostete Unternehmensdaten.
5. **Gewerbliche Softwarelizenzierung durch eine anwaltliche Berufsausübungsgesellschaft** (§§ 59b ff. BRAO). Hier besteht ein Zielkonflikt: Eine Auslagerung in eine Software-GmbH entschärft das Berufsrecht, verschärft aber das RDG-Risiko.
6. **Deckungslücken der Berufshaftpflicht** bei technischen Fehlern, die Serienschadenklausel und das Abgrenzungsrisiko zwischen „wissentlicher Pflichtverletzung" und bloßer Fahrlässigkeit bei unkritischer KI-Übernahme.
7. **Produkthaftung:** Unsicher sind der Umsetzungsstand zum 9.12.2026 und die Abgrenzung zwischen „Software" (Produkt) und „Information" bzw. Inhalt (kein Produkt). Die Arbeitsanleitungen als Rechtsinhalt dürften eher Information sein (ErwG der RL 2024/2853; hier nicht im Wortlaut geprüft).
8. **Datenschutzrolle der Kanzlei:** Auftragsverarbeitung, Eigenverantwortung oder Art. 26? Hinzu kommt die Zukunft des Art. 88c DSGVO im Omnibus.
9. **Berufsverbände:** Eine gezielte BRAK- oder DAV-Stellungnahme zu „KI und RDG" ließ sich nicht finden.\[28\] Die BRAK hat sich am 2.3.2026 zum KI-Omnibus geäußert und dort u. a. eine zu starke Verschiebung der Hochrisiko-Regeln abgelehnt.\[105\]\[106\]

---

## Empfehlungen

1. **Geschäftsmodell offen festlegen und nicht verschleiern.** Am belastbarsten ist das *anwaltliche* Modell: ein Mandatsvertrag für die Arbeitsanleitungen und ihre Pflege, kombiniert mit einer SaaS-Lizenz. Dazu gehören Konfliktprüfung, § 52-BRAO-Haftungsbegrenzung und Vergütungsvereinbarung. Die Alternative „reine Software" gelingt nur mit generischen, nicht mandantenspezifischen Arbeitsanleitungen, ohne Einzelfallzugriff und ohne fallbezogene Nachsteuerung.
2. **Vertragspaket:** SaaS-Vertrag (Ausschluss von § 536a Abs. 1 Alt. 1 BGB, SLA), Auftragsverarbeitungsvertrag nach Art. 28 DSGVO samt § 43e-BRAO-Anlage mit Belehrung nach § 203 StGB und Subunternehmerliste (LLM, Cloud), Zweckbestimmung mit ausdrücklichem Ausschluss von Anhang-III-Einsätzen (insbesondere HR), Regelung der Kontrollpunkte als Pflicht des Unternehmens, Trainingsverbot für Kundendaten.
3. **KI-Verordnung sofort umsetzen:** Rollendokumentation, Transparenz nach Art. 50 Abs. 1, technische Kennzeichnung nach Art. 50 Abs. 2 (spätestens zum 2.12.2026 für Altsysteme), Schulungskonzept nach Art. 4 für beide Seiten, Monitoring der Hochrisiko-Schwelle bis zum 2.12.2027.
4. **Versicherung vor Vertriebsstart:** schriftliche Deckungsbestätigung des Berufshaftpflichtversicherers für das Modell, eine Tech-E&O- und eine Cyberpolice, eine Prüfung der Serienschadenklausel und ein Exzedent.
5. **Datenschutz:** Datenschutz-Folgenabschätzung durch das Unternehmen mit Unterstützung der Kanzlei, Pseudonymisierung vor dem LLM-Aufruf, EU-Hosting, Löschkonzept für Logs und Agenten-Speicher, dokumentierte echte menschliche Prüfung (Art. 22).
6. **Klärung mit der Rechtsanwaltskammer** zur gewerblichen Tätigkeit der Berufsausübungsgesellschaft und zur Werbung.

## Caveats

- Mehrere Stände Mitte 2026 (Omnibus-Daten-Teil, ProdHaftG-Verfahren, KI-MIG-Daten) stützen sich teils auf Fachblogs und Kanzlei- oder Beraterseiten. Amtlich geprüft habe ich die Verordnung (EU) 2026/1744 (EUR-Lex), die BT-Drs. 21/4297, die BGH-Entscheidung I ZR 113/20, die Pressemitteilungen von Bundestag und Bundesnetzagentur sowie die Curia-Pressemitteilung zu C-413/23 P.
- Nicht im Volltext verifiziert sind: LG Köln 33 O 35/19, BGH XII ZR 120/04, BAG GS 1/89 (A) und § 53 StPO zum Syndikus.
- Die Ratsdokumente zum Daten-Omnibus sind geleakte LIMITE-Dokumente und nur aus Sekundärberichterstattung bekannt.
- Beck-online und juris waren nicht zugänglich. Kommentarliteratur (z. B. Remmertz, Legal Tech-Strategien für die Rechtsanwaltschaft, 2. Aufl. 2025) wird nur nach Sekundärangaben genannt.

---

## 4. Verzeichnis der ausgewerteten Rechtsquellen, Entscheidungen und Stellungnahmen (mit Datum)

**Normen (amtlich):** RDG §§ 1–3 (gesetze-im-internet.de, abgerufen Okt. 2026); BRAO §§ 43, 43a, 43b, 43e, 46, 46a, 46c, 51, 52, 59b ff., 59o; BORA § 3; StGB § 203; BGB §§ 254, 280, 535 ff., 611, 675, 823; Verordnung (EU) 2024/1689 (ABl. L vom 12.7.2024, in Kraft 1.8.2024); Verordnung (EU) 2026/1744 vom 8.7.2026 (ABl. L vom 24.7.2026, in Kraft 27.7.2026); Richtlinie (EU) 2024/2853 vom 23.10.2024 (ABl. L vom 18.11.2024); Verordnung (EU) 2016/679 (DSGVO); KI-MIG (Bundestag 11.6.2026; in Kraft laut BNetzA 29.7.2026).

**Gesetzgebungsmaterialien:** Regierungsentwurf Produkthaftungsrecht, Kabinett 17.12.2025, BR-Drs. 775/25 (19.12.2025), BR-Stellungnahme 30.1.2026, BT-Drs. 21/4297 (25.2.2026), 1. Lesung 4.3.2026, Anhörung 13.4.2026; RegE KI-Durchführungsgesetz BT-Drs. 21/4594, Ausschussfassung 21/6407; RegE Neuordnung aufsichtsrechtlicher Verfahren BT-Drs. 21/4298 (25.2.2026); Kommissionsvorschlag Digital Omnibus COM(2025) 837 (19.11.2025); Kommissionsarbeitsprogramm 2025 (11.2.2025, Rücknahme der KI-Haftungsrichtlinie).

**Rechtsprechung:** BGH 9.9.2021 – I ZR 113/20 (Smartlaw); OLG Köln 19.6.2020 – 6 U 263/19; LG Köln 8.10.2019 – 33 O 35/19; BGH 27.11.2019 – VIII ZR 285/18; BGH 13.7.2021 – II ZR 84/20; BGH 13.6.2022 – VIa ZR 418/21; OLG Hamm 12.5.2026 – 4 UKl 3/25; BGH 22.6.2020 – AnwZ (Brfg) 23/19; BGH Oktober 2018 – AnwZ (Brfg) 58/17; BGH 5.10.2020 – AnwZ (Brfg) 43/18; BVerfG 27.4.2021 – 1 BvR 2649/20; BGH 15.11.2006 – XII ZR 120/04; BAG GS 27.9.1994 – GS 1/89 (A); EuGH 30.3.2023 – C-34/21; EuGH 7.12.2023 – C-634/21; EuGH 4.9.2025 – C-413/23 P.

**Stellungnahmen und Hinweise:** BRAK, Hinweise zum Einsatz von KI (Stand Dezember 2024); BRAK, Stellungnahme zum KI-Omnibus (2.3.2026); BRAK-Stellungnahme Nr. 53/2025 zur Berufsrechtsreform (November 2025); BRAK-FAQ zur DS-GVO (19.12.2019); DSK-Kurzpapier Nr. 13 (Stand 17.12.2018); DAV-Initiativ-Stellungnahme Nr. 32/2025 zum Einsatz von KI in der Anwaltschaft (Juli 2025); EDSA/EDSB, Gemeinsame Stellungnahme (20.1.2026); Legal Tech Verband, Stellungnahme zum Neuordnungsgesetz (2025/2026).

**Fachbeiträge:** Remmertz, „Rechtsberatung durch KI-Chatbot – Was ein Urteil zur Schönheitschirurgie mit dem RDG zu tun hat", legal-tech-verzeichnis.de (10.6.2026); Anwaltsblatt, „Zukunft des Rechtsdienstleistungsrechts im Zeitalter von Legal Tech und KI" (undatiert abgerufen); Anwaltsblatt, „Reicht die Berufshaftpflichtversicherung noch im Hinblick auf KI?"; Anwaltsblatt, „Legal Tech und Serienschäden"; Anwaltsblatt, „BGH erlaubt Vertragsgenerator Smartlaw" (AnwBl Online 2021, 264); beck-aktuell, „Neue KI-Regeln in New York: Was sollten Chatbots in der Rechtsberatung dürfen?" (18.3.2026); beck-aktuell, „Darf ChatGPT Jura?" (11.11.2025); Grams, „Digital Omnibus: Ihre Daten als Trainingsfutter für KI?" (23.9.2026, Sekundärquelle zu den Ratsdokumenten); Bird & Bird, „Ein Update für die DSGVO?" (2026).

## Quellen

1. [BGH erlaubt Vertragsgenerator Smartlaw: Legal Tech hat Zukunft - Anwaltsblatt](https://anwaltsblatt.anwaltverein.de/de/themen/recht-gesetz/bgh-erlaubt-smartlaw)
2. [Neue Nutzungsbedingungen: Keine Rechtsberatung mehr von ChatGPT?](https://www.lto.de/recht/nachrichten/n/chatpgt-openai-aenderung-nutzungsbedingungen-keine-rechtsberatung)
3. [§ 2 RDG - Begriff der Rechtsdienstleistung - Gesetze - JuraForum.de](https://www.juraforum.de/gesetze/rdg/2-begriff-der-rechtsdienstleistung)
4. [Branchenverbände: Wann die Erbringung von Rechtsdienstleistungen zulässig ist](https://winheller.com/blog/branchenverband-erbringung-rechtsdienstleistungen/)
5. [Ein Service des Bundesministeriums der Justiz sowie des Bundesamts für](https://www.gesetze-im-internet.de/rdg/RDG.pdf)
6. [BGH: Vertragsgenerator Smartlaw ist zulässig](https://www.lto.de/recht/juristen/b/bgh-izr11320-vertragsgenerator-smartlaw-legal-tech-keine-unzulaessige-rechtsdienstleistung-rdg-rechtsberatung)
7. [BGH: Darum ist der Vertragsgenerator Smartlaw zulässig](https://www.lto.de/recht/juristen/b/bgh-urteil-izr11320-vertragsgenerator-smartlaw-keine-unzulaessige-rechtsdienstleistung-rak-hamburg-rdg-legal-tech)
8. [Künstliche Intelligenz in der Rechtsberatung](https://www.justitai.de/blog/ki-rechtsberatung)
9. [Rechtsberatung durch KI-Chatbot – Was ein Urteil zur Schönheitschirurgie mit dem RDG zu tun hat](https://legal-tech-verzeichnis.de/fachartikel/rechtsberatung-durch-ki-chatbot-was-ein-urteil-zur-schoenheitschirurgie-mit-dem-rdg-zu-tun-hat/)
10. [Legal Tech](https://www.iww.de/ak/kanzleiorganisation/legal-tech-der-digitale-vertragsgenerator-smartlaw-verstoesst-nicht-gegen-das-rechtsdienstleistungsgesetz-b155014)
11. [BGH: Digitaler Vertragsdokumentengenerators "Smartlaw" rechtlich zulässig - Kanzlei Dr. Bahr](https://www.dr-bahr.com/news/digitaler-vertragsdokumentengenerators-smartlaw-rechtlich-zulaessig.html)
12. ["Tut mir leid, ich kann Dir keine individuelle Rechtsberatung geben": Darf ChatGPT Jura?](https://www.beck-aktuell.de/rechtsbranche/legal-tech-digitalisierung/chatgpt-individuelle-rechtsberatung-ki-jura-rechtsdienstleistung-2025-11-11)
13. [BGH: Vertragsdokumente-Generator smartlaw zulässig](https://www.brak.de/newsroom/news/bgh-vertragsdokumente-generator-smartlaw-zulaessig/)
14. [Zukunft des Rechtsdienstleistungsrechts im Zeitalter von Legal Tech und KI - Anwaltsblatt](https://anwaltsblatt.anwaltverein.de/de/themen/recht-gesetz/rechtsdienstleistungsrecht-legal-tech-ki)
15. [OLG Hamm lässt Unternehmen für Aussagen seines Chatbots haften, Volltext verfügbar - Wettbewerbszentrale](https://www.wettbewerbszentrale.de/olg-hamm-laesst-unternehmen-fuer-aussagen-seines-chatbots-haften-volltext-verfuegbar/)
16. [Oberlandesgericht Hamm: Urteil in Verbraucherzentrale Nordrhein-Westfalen e.V. gegen Aesthetify GmbH](https://www.olg-hamm.nrw.de/behoerde/presse/Pressemitteilungen/16_26_PE_KI-Chatbot/index.php)
17. [KI-Rechtsberatung: Was die Jura-KI kann und was sie kostet](https://anwaltguru.de/ki-rechtsberatung)
18. [Erbringen KI Chatbots unerlaubte Rechtsberatung iSd RDG?](https://legal-tech-verzeichnis.de/legal-tech-videos/erbringen-ki-chatbots-unerlaubte-rechtsberatung-isd-rdg-interview-mit-markus-hartung/)
19. [RDG-Verstoß: LG verbietet Legal-Tech-Unternehmen](https://www.lto.de/recht/juristen/b/lg-koeln-urteil-33o3519-smartlaw-vertragsgenerator-legal-tech-modell-verboten-rdg)
20. [BGH: Legal-Tech-Anbieter Financialright GmbH kann Schadensersatzansprüche eines Schweizers im VW-Dieselskandal auf Grundlage einer deutschen Inkassolizenz nach Abtretung einklagen](https://www.beckmannundnorda.de/serendipity/index.php?%2Farchives%2F5995-BGH-Legal-Tech-Anbieter-Financialright-GmbH-kann-Schadensersatzansprueche-eines-Schweizers-im-VW-Dieselskandal-auf-Grundlage-einer-deutschen-Inkassolizenz-nach-Abtretung-einklagen.html=)
21. [Richtungswechsel perfekt: Erfolgshonorare für Anwälte](https://www.lto.de/recht/juristen/b/anwaelte-erfolgshonorar-prozesskosten-rdg-bmjv-referentenentwurf-brak-berufsrecht-legaltech)
22. [Eil: BGH billigt Legal-Tech-Modell auf Inkassobasis](https://www.lto.de/recht/juristen/b/bgh-viii-zr-285-18-legal-tech-wenigermiete-de-inkassodienstleister-abtretung-rechtsdienstleistungsgesetz)
23. [Berufsrecht](https://www.iww.de/fmp/forderungsrecht/berufsrecht-bgh-legal-tech-als-inkassodienstleistung-ist-echte-rechtsdienstleistung-f125532)
24. [Regierung will Anpassungen im Berufsrecht der rechtsberatenden Berufe](https://www.datev-magazin.de/nachrichten-steuern-recht/recht/regierung-will-anpassungen-im-berufsrecht-der-rechtsberatenden-berufe-145647)
25. [21\. Wahlperiode Ausschuss für Recht und Verbraucherschutz](https://www.bundestag.de/resource/blob/1166908/Stellungnahme_79e_Uwer.pdf)
26. [Deutscher Bundestag - Regierung will Anpassungen im Berufsrecht der rechtsberatenden Berufe](https://www.bundestag.de/dokumente/textarchiv/2026/kw13-de-rechtsberatende-berufe-1156682)
27. [Stellungnahme des Legal Tech Verband Deutschland zum Gesetz zur Neuordnung aufsichtsrechtlicher Verfahren](https://www.legaltechverband.de/aktivitaeten/stellungnahme-des-legal-tech-verband-deutschland-zum-gesetz-zur-neuordnung-aufsichtsrechtlicher-verfahren/)
28. [Neue KI-Regeln in New York: Was sollten Chatbots in der Rechtsberatung dürfen?](https://www.beck-aktuell.de/rechtsbranche/legal-tech-digitalisierung/ki-regeln-new-york-chatbots-rechtsberatung-bias-rdg-2026-03-18)
29. [Justiziar: Lohnen sich Gehalt & Arbeit ohne Kanzlei?](https://www.jurahilfe.de/blog/justiziar)
30. [Unerlaubte Rechtsberatung: RDG, Haftung & höflich absagen](https://www.jurahilfe.de/blog/unerlaubte-rechtsberatung)
31. [FAQ-Liste zum Recht der Syndikusanwälte - Syndikusanwaelte](https://www.syndikusanwaelte.de/de/berufsrecht-befreiung/faq-liste-zum-recht-der-syndikusanwaelte)
32. [§ 46 BRAO](https://lxgesetze.de/brao/46)
33. [BGH, Urteil v. 22.06.2020 - AnwZ (Brfg) 23/19 - NWB Urteile](https://datenbank.nwb.de/Dokument/831243/)
34. [723 Rechtsprechung Anwaltsrecht AnwBl Online 2020 723 AnwaltsWissen](https://anwaltsblatt.anwaltverein.de/files/anwaltsblatt.de/anwaltsblatt-online/2020-723.pdf)
35. [Digitales Vertragsmanagement in Kanzleien: was § 43e BRAO verlangt](https://legal-tech-verzeichnis.de/fachartikel/digitales-vertragsmanagement-in-kanzleien-was-paragraph-43e-brao-verlangt/)
36. [Künstliche Intelligenz](https://www.iww.de/kp/berufsrecht/kuenstliche-intelligenz-leitfaden-der-brak-zum-einsatz-von-ki-in-der-beratungspraxis-f165486)
37. [KI in Anwaltskanzleien (BRAK) - NWB Livefeed](https://datenbank.nwb.de/Dokument/1060545/)
38. [Darf die KI Anwalt sein? - Anwaltspraxis Magazin](https://anwaltspraxis-magazin.de/kanzleimagazin/darf-die-ki-anwalt-sein/)
39. [Bundesrechtsanwaltskammer Büro Berlin](https://www.brak.de/fileadmin/service/publikationen/Handlungshinweise/BRAK_Leitfaden_mit_Hinweisen_zum_KI-Einsatz_Stand_12_2024.pdf)
40. [KI in der Anwaltskanzlei - Leitlinien der BRAK (Dezember 2024)](https://www.get-aimax.de/ki-in-der-anwaltskanzlei-leitlinien-der-bundesrechtsanwaltskammer-brak)
41. [Deutscher Anwaltverein Littenstraße 11, 10179 Berlin Tel.: +49 30 726152-0](https://anwaltverein.de/newsroom/sn-32-25-einsatz-von-ki-in-der-anwaltschaft?file=files%2Fmedia%2Fnews%2Freplicator%2Fstellungnahmen%2Fdav-sn-32-25.pdf)
42. [DAV-Stellungnahme: KI-Einsatz mit dem Anwaltsberuf vereinbar](https://www.pylehound.com/de/news/28-07-2025-DAV-stellungnahme-ki-einsatz.html)
43. [BRAO-konforme KI für Kanzleien 2026](https://ironum.com/de/ressourcen/blog/ki-in-der-kanzlei-dsgvo-verschwiegenheit-brao/)
44. [§ 43e BRAO](https://lxgesetze.de/brao/43e)
45. [§ 43e BRAO — Inanspruchnahme von Dienstleistungen](https://www.lulius.ai/gesetze/brao/43e)
46. [KI und Berufsgeheimnis: § 203 StGB und § 43e BRAO](https://www.agentifizierung.de/softwarekosten-senken/ki-berufsgeheimnistraeger-mandantendaten)
47. [Digital Omnibus on AI: Was sich 2026 im EU AI Act ändert](https://me-ctc.de/itsv/digital-omnibus-on-ai-2026/)
48. [KI-Verordnung: Was ab dem 2. August 2026 gilt](https://www.unternehmensnachrichten.com/archives/83748)
49. [Digital-Omnibus zur KI-Verordnung: Mehr Zeit für Hochrisiko-KI](https://scheja-partners.de/insights/trends-and-takeaways/digital-omnibus-zur-ki-verordnung-mehr-zeit-fuer-hochrisiko-ki/)
50. [Digital Omnibus: Was der Stand vom 20. Juli 2026 für Ihr Cross-Framework-Inventar bedeutet · Brain-Media.de](https://www.brain-media.de/blog/digital-omnibus-stand-und-folgen.html)
51. [Digital Omnibus AI Act 2027: Was die Fristverschiebung jetzt bedeutet](https://skill-sprinters.de/blog/compliance/digital-omnibus-ai-act-fristverschiebung-2027/)
52. [Änderungen der KI-Verordnung durch den Digitalen Omnibus](https://www.activemind.legal/de/guides/aenderungen-ki-verordnung/)
53. [L\_202601744DE.000101.fmx.xml](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=OJ%3AL_202601744)
54. [EU AI Act im Trilog: 1-Jahres-Verschiebung möglich, was Mittelstand trotzdem jetzt tun sollte](https://skill-sprinters.de/blog/compliance/eu-ai-act-trilog-verschiebung-mai-2026-was-mittelstand-jetzt-tun-sollte/)
55. [EU AI Act Gesetzestext (EU 2024/1689): Die KI-Verordnung auf Deutsch](https://www.eu-ai-act.info/gesetz.html)
56. [KI-Verordnung für Unternehmen einfach erklärt](https://www.windweiss.de/ratgeber/ai-act-ki-verordnung/)
57. [Vorsicht vor dem Quasi-Anbieter](https://www.aitava.com/insights/vorsicht-vor-dem-quasi-anbieter-art-25-ai-act-im-praxistest/)
58. [Anbieter oder Betreiber? Deine Rolle laut der EU-KI-Verordnung](https://medien-bayern.de/eu-ai-act-anbieter-betreiber-medien)
59. [Avatar an Endkunden weitergeben, Rolle und Vertrag](https://aidentical.de/ki-avatar-fuer-it-dienstleister-und-msps-kunden-onboarding-und-self-service-automatisieren/)
60. [Die EU-KI-Verordnung und ihre Folgen für Kanzleien](https://berufsrecht-anwaelte.de/ki-im-anwaltsberuf/ki-verordnung/)
61. [KI-Verordnung: bis zu 3 Prozent vom Konzernumsatz](https://www.digital-chiefs.de/art-50-transparenzpflichten-rollen-review/)
62. [KI-Verordnung 2026: Was ab 2. August wirklich gilt](https://einfach-digital.de/aktuelles/ki-verordnung-was-jetzt-gilt)
63. [Durchführung der KI-Verordnung](https://www.inkasso.de/newsdetail/durchfuehrung-der-ki-verordnung)
64. [KI-Aufsicht Bundesnetzagentur: Das KI-MIG im Überblick](https://cortina-consult.com/ki-compliance/wissen/ki-aufsicht-bundesnetzagentur/)
65. [KI-Verordung und die Durchführung - Datenschutz mit System](https://kt-datenschutz.de/ki-verordung-und-die-durchfuehrung/)
66. [Bundesnetzagentur - Presse - Bundesnetzagentur übernimmt zentrale Rolle bei der Umsetzung der KI-Verordnung](https://www.bundesnetzagentur.de/SharedDocs/Pressemitteilungen/DE/2026/20260729_KI_VO.html)
67. [KI-MIG 2026: Das deutsche AI-Act-Gesetz im Überblick - CASIS Unternehmensgruppe](https://casis.de/ki-mig-deutschlands-durchfuehrungsgesetz-zum-ai-act-ist-da/)
68. [OLG Hamm: Unternehmen haften für Halluzinationen ihres KI-Chatbots](https://petersenpartners.de/de/news/olg-hamm-unternehmen-haften-fuer-halluzinationen-ihres-ki-chatbots/)
69. [Produkthaftungsgesetz neu: Software & KI haften ab 2026](https://www.yagemi.de/blog/recht-compliance/produkthaftungsgesetz/)
70. [Referentenentwurf des Bundesministeriums der Justiz und für Verbraucherschutz](https://www.bmjv.de/SharedDocs/Downloads/DE/Gesetzgebung/RefE/RefE_Produkthaftung.pdf?__blob=publicationFile&amp=&v=2)
71. [Deutscher Bundestag - Produkthaftungsrecht soll umfassend modernisiert werden](https://www.bundestag.de/presse/hib/kurzmeldungen-1150966)
72. [Modernisierung des Produkthaftungsrechts (Bundestag)](https://www.bbh-fortbildungen.de/2026/05/15/modernisierung-des-produkthaftungsrechts-bundestag/)
73. [Deutscher Bundestag Drucksache 21/4297 21. Wahlperiode 25.02.2026](https://dserver.bundestag.de/btd/21/042/2104297.pdf)
74. [\- 38 - Erläuterung, 1061. BR, 30.01.26 ... TOP 38: Entwurf eines Gesetzes zur](https://www.bundesrat.de/SharedDocs/TO/1061/erl/38.pdf?__blob=publicationFile&v=1)
75. [Modernisierung des Produkthaftungsrechts (Bundestag) - NWB Livefeed](https://datenbank.nwb.de/Dokument/1089256/)
76. [Neues Produkthaftungsgesetz ab Dezember 2026: Was ändert sich?](https://www.marsh.com/de/services/casualty/insights/new-product-liability.html)
77. [Bundesrat Drucksache 775/25 19.12.25 R - U - Wi](https://dserver.bundestag.de/brd/2025/0775-25.pdf)
78. [Erste Lesung zur Modernisierung des Produkthaftungsrechts - Deutscher Bundestag](https://www.bundestag.de/dokumente/textarchiv/2026/kw10-de-produkthaftungsrecht-1150448)
79. [Update: Novelle zum Produkthaftungsrecht im Bundestag - NWB Experten-Blog](https://www.nwb-experten-blog.de/update-novelle-zum-produkthaftungsrecht-im-bundestag/)
80. [Neues Produkthaftungsgesetz ab 9. Dezember 2026: Was Hersteller, Importeure und Umrüster jetzt prüfen müssen](https://industrie-fachwissen.de/data/neues-produkthaftungsgesetz-2026-hersteller-importeure-software-haftung)
81. [Neues Produkthaftungsgesetz: Handlungsbedarf für Software-, KI- und Digitalanbieter - Was die Reform des Produkthaftungsrechts für Hersteller, Importeure, Plattformen und digitale Anbieter bedeutet.](https://www.ebnerstolz.de/de/unser-angebot/leistungen/rechtsberatung/produktsicherheit-und-produkthaftung/neues-produkthaftungsgesetz-110227.html)
82. [Neues Produkthaftungsgesetz für Software & digitale Produkte - Checkmate Experts](https://www.checkmate.expert/produkthaftungsgesetz-digitale-produkte.html)
83. [BTZusFas: Gesetz zur Modernisierung des Produkthaftungsrechts](https://bundestagszusammenfasser.de/details?docid=1052)
84. [Europäische Kommission hat KI-Haftungsrichtlinie zurückgezogen - FEEI](https://www.feei.at/aktuelles/europaeische-kommission-hat-ki-haftungsrichtlinie-zurueckgezogen/)
85. [Aufsicht Mit Dem Falschen Werkzeug - Flaschenpost](https://die-flaschenpost.de/2026/09/01/aufsicht-mit-dem-falschen-werkzeug/)
86. [KI in der Kanzlei - BRAK gibt Leitfaden als Orientierungshilfe - datenschutzticker.de](https://www.datenschutzticker.de/2025/03/ki-in-der-kanzlei-brak-gibt-leitfaden-als-orientierungshilfe/)
87. [Reicht die Berufshaftpflichtversicherung noch im Hinblick auf KI? - Anwaltsblatt](https://anwaltsblatt.anwaltverein.de/de/themen/markt-chancen/berufshaftpflichtversicherung-im-hinblick-auf-ki)
88. [Legal Tech und Künst­liche Intelligenz im Kontext der Berufs­haftpflicht](https://vonlauffundbolz.de/legal-tech-und-kuenstliche-intelligenz-im-kontext-der-berufshaftpflicht/)
89. [§ 51 BRAO](https://lxgesetze.de/brao/51)
90. [Legal Tech und Serienschäden - Anwaltsblatt](https://anwaltsblatt.anwaltverein.de/de/themen/recht-gesetz/legal-tech-und-serienschaeden?full=1)
91. [KI und anwaltliche Berufshaftpflicht](https://www.behrschmidtkollegen.de/ki-und-anwaltliche-berufshaftpflicht/)
92. [Berufshaftpflichtversicherung im Zeitalter von Künstlicher Intelligenz (KI)](https://www.gewerbeversicherung-vergleich.com/blog/2024/11/berufshaftpflichtversicherung-im-zeitalter-von-kuenstlicher-intelligenz-ki/)
93. [Berufshaftpflicht KI: Was Ihre Police wirklich abdeckt — Lulius](https://www.lulius.ai/blog/berufshaftpflicht-ki-kanzlei)
94. [EuGH bestätigt relativen Personenbezug von personenbezogenen Daten - Verlag Dr. Otto Schmidt](https://www.otto-schmidt.de/blog/it-recht-blog/eugh-bestatigt-relativen-personenbezug-von-personenbezogenen-daten-ITBLOG0008001.html)
95. [EuGH bestätigt relativen Personenbezug von ...](https://www.skwschwarz.de/en/news/ecj-confirms-concept-of-relative-personal-data)
96. [Informationspflichten auch bei pseudonymisierten Daten?](https://www.activemind.legal/de/guides/urteil-pseudonymisierung/)
97. [Digital Omnibus: Ihre Daten als Trainingsfutter für KI?](https://blog.grams-it.com/2026/09/23/digital-omnibus-ihre-daten-als-trainingsfutter-fuer-ki/)
98. [Bedeutet der Digital Omnibus das Ende der DSGVO, wie wir sie kennen?](https://www.e-recht24.de/datenschutz/13548-digital-omnibus.html)
99. [Ein Update fr die Datenschutz-Grundverordnung (DSGVO) - Bird & Bird](<https://www.twobirds.com/de/insights/2026/germany/ein-update-fr-die-datenschutz-grundverordnung-(dsgvo)>)
100. [Digital Omnibus: Neue Regeln für Datenschutz und Compliance](https://www.iubenda.com/de/blog/digital-omnibus-neue-regeln-fuer-datenschutz-und-compliance/)
101. [Parlamentarische Materialien](https://www.parlament.gv.at/dokument/XXVIII/A/724/fnameorig_1742072.html)
102. [Digitaler Omnibus: Neue EU-Pläne für KMU-Datenschutz](https://www.proliance.ai/blog/eu-omnibus-datenschutz-kmu)
103. [Digital Omnibus](https://betriebs-berater.com/40349/2026/bb_2026_01-02_b4/)
104. [KI-Bot auf einer Website informiert falsch](https://www.anwalt.de/rechtstipps/ki-bot-auf-einer-website-informiert-falsch-wer-haftet-273864.html)
105. [Stellungnahme zum KI-Omnibus](https://www.brak.de/newsroom/newsletter/nachrichten-aus-bruessel/2026/ausgabe-04-2026-v-26022026/stellungnahme-zum-ki-omnibus-brak/)
106. [künstliche Intelligenz (KI)](https://www.brak.de/schlagwort/kuenstliche-intelligenz/)
