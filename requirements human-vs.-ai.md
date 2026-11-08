Runde 1
REQ-002 Fast and Friendly: Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein.

Identifizierte Mängel:
Die Anforderung ist sehr oberflächlich formuliert. Begriffe wie schnell, intuitiv und besonders benutzerfreundlich werden nicht näher definiert und lassen sich auch nicht objektiv prüfen.

Strategie: INVESTIGATE

Die Benutzeroberfläche des Study Buddys soll verständlich und seitens der Studierenden effizient nutzbar sein. Um geeignete Messgrößen sowie Akzeptanzkriterien definieren zu können werden Befragungen mit den Studierenden durchgeführt. 

Offene Fragen:

- Welche Funktionen müssen besonders schnell reagieren?
- Welche Antwortzeiten sind akzeptabel?
- Woran soll die Benutzerfreundlichkeit gemessen werden?

REQ-004 The Perfect Prediction: Das System muss zuverlässig erkennen, welche Studierenden ihr Studium nicht erfolgreich abschließen werden. 

Identifizierte Mängel:
Der Begriff zuverlässig lässt sich schwer messbar definieren. Weiters wird gefordert, dass ein zukünftiger Studienabbruch anhand vorhandener Daten genau vorhergesagt werden kann. 

Strategie: RECONSIDER

Es soll geprüft werden, ob sich ein Unterstützungsbedarf anhand der verfügbaren Informationen ableiten lässt. Die ursprüngliche Anforderung, dass eine genaue Vorhersage getroffen werden soll, wird in dieser Form folglich nicht übernommen.

Offene Fragen:

- Anhand welcher Indikatoren lässt sich Unterstützungsbedarf ableiten?
- Wie zuverlässig lassen sich solche Hinweise erkennen?
- Dürfen die verfügbaren Informationen in dieser Form verwendet und verarbeitet werden?

REQ-007 The Notification Paradox: Studierende müssen sämtliche Benachrichtigungen jederzeit deaktivieren können.

Identifizierte Mängel:
Diese Anforderung steht in direktem Widerspruch zu REQ-008, welche besagt, dass die Studierenden über kritische Studienereignisse informiert werden müssen, ungeachtet ihrer Einstellungen. 

Strategie: INVESTIGATE

Der Study Buddy soll Studierenden die Möglichkeit bieten Benachrichtungseinstellungen selbstständig festzulegen. Dazu muss definiert werden welche Kategorien von Benachrichtigungen es gibt und welche davon deaktiviert werden dürfen. Weiters ist zu definieren, welche Benachrichtungen zwingend zugestellt werden müssen. 

Offene Fragen:

- Welche Kategorien von Benachrichtungen gibt es?
- Welche Benachrichtigungen sollen deaktivierbar sein?
- Welche Benachrichtungen sollen zwingend zugestellt werden?

REQ-009: The Secret Dashboard: Die Studiengangsleitung muss jederzeit auf sämtliche individuellen Lernaktivitäten aller Studierenden zugreifen können.

Identifizierte Mängel:

Es wird nicht definiert wozu ein so weitreichender Zugriff auf die Informationen der Studierenden notwendig ist. Ein uneingeschränkter Zugriff auf die Lernaktivitäten der Studierenden könnte gegebenenfalls zu Verletzungen von DSGVO.

Strategie: RECONSIDER

Es muss zunächst geprüft werden, welche Informationen grundsätzlich benötigt werden und wie sich das rechtlich vereinbaren lässt. Dafür ist in weiterer Folge ein Berechtigungskonzept mit klar definierten Rollen und Zugriffsberechtigungen festzulegen. 

Offene Fragen:

- Welche Informationen werden benötigt?
- Wofür werden diese Informationen benötigt?
- Wie soll der Zugriff auf diese Informationen gestaltet werden ohne gegen die DSGVO zu verstoßen?

REQ-015 The AI Knows Best: Ein KI-Modell muss anhand Nutzungsdaten automatisch entscheiden, welche Studierenden zusätzliche Betreuung benötigen. 

Identifizierte Mängel:
Es ist abzuklären, ob eine solche Übermittelung an die KI datenschutzkonform ist. Weiters muss ermittelt werden, ob die Informationen korrekt oder gegebenenfalls falsch sind. Zusätzlich fehlt in der Anforderung die menschliche Instanz, welche bspw. die Datenqualität kontrollieren kann. 

Strategie: RECONSIDER

Es muss geprüft werden, ob die Anforderung zum einen in dieser Form umsetzbar ist und zum anderen ob die Anforderung rechtlich möglich ist. Weiters muss eine menschliche Kontrollinstanz implementiert werden und zusätzlich muss abgestimmt werden in welcher Form die Empfehlung zur zusätzlichen Betreuung umgesetzt werden soll.

Offene Fragen:

- Wie wird die Empfehlung zur Betreuung umgesetzt?
- Dürfen solche Informationen ohne weiteres an die KI übermittelt werden?
- Welche menschliche Kontrollinstanz gibt es?

Runde 2

Dokumentation

KI-System: ChatGPT

Modell: GPT-6

Datum: 07.11.2026

Untersuchungsgegenstand: REQ siehe oben

Vorgehensweise: Einheitlicher Prompt

Bearbeitung: KI-generiert

Verwendeter Prompt:
Du bist Requirements Engineer und überprüfst Anforderungsentwürfe für den Digital Study Buddy, ein digitales Unterstützungssystem für Studierende einer Fernhochschule. Analysiere jede Anforderung anhand der Qualitätsaspekte Inhalt, Dokumentation und Abgestimmtheit. 1. Identifiziere konkrete Qualitätsmängel und begründe sie. 2. Formuliere eine verbesserte Anforderung, soweit die vorliegenden Informationen dies erlauben. 3. Erfinde keine Stakeholderbedürfnisse, Interviewergebnisse, rechtlichen Freigaben oder technischen Rahmenbedingungen. 4. Kennzeichne fehlende Informationen, unbegründete Annahmen und notwendige Abstimmungen ausdrücklich. 5. Schlage geeignete Akzeptanzkriterien nur vor, wenn diese fachlich begründbar sind. 6. Gib für jede Anforderung den Status REWRITE, INVESTIGATE oder RECONSIDER an. Hier sind die Anforderungen:
- REQ-002 Fast and Friendly: Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein
- EQ-004 The Perfect Prediction: Das System muss zuverlässig erkennen, welche Studierenden ihr Studium nicht erfolgreich abschließen werden.
- REQ-007 The Notification Paradox: Studierende müssen sämtliche Benachrichtigungen jederzeit deaktivieren können.
- REQ-009: The Secret Dashboard: Die Studiengangsleitung muss jederzeit auf sämtliche individuellen Lernaktivitäten aller Studierenden zugreifen können.
- REQ-015 The AI Knows Best: Ein KI-Modell muss anhand Nutzungsdaten automatisch entscheiden, welche Studierenden zusätzliche Betreuung benötigen.

KI Version – REQ-002
1. Qualitätsmängel

Die Anforderung enthält subjektive und nicht operationalisierte Qualitätsbegriffe. Ohne festgelegte Leistungskennzahlen und Kriterien zur Gebrauchstauglichkeit ist keine objektive Abnahme möglich.

2. Verbesserte Anforderung

Der Study Buddy muss eine Benutzeroberfläche bereitstellen, deren Gebrauchstauglichkeit und Reaktionsverhalten anhand definierter Nutzungsszenarien überprüft werden können. Für die relevanten Funktionen sind messbare Antwortzeitgrenzen und Usability-Akzeptanzkriterien festzulegen, bevor die Anforderung als vollständig spezifiziert gilt.

3. Offene Fragen

Welche Nutzungsszenarien sind relevant? Welche Leistungsgrenzen gelten? Mit welchen Methoden soll die Gebrauchstauglichkeit geprüft werden?

4. Empfohlene Strategie: INVESTIGATE
KI Version – REQ-004
1. Qualitätsmängel

Die Anforderung enthält ein nicht definiertes Zuverlässigkeitsziel und setzt die Vorhersagbarkeit zukünftiger Studienergebnisse voraus. Die Datenbasis, die Zielvariable und die akzeptablen Fehlerraten sind unbekannt.

2. Verbesserte Anforderung

Vor einer Implementierung ist zu prüfen, ob der Study Buddy anhand zulässiger Daten statistisch belastbare Hinweise auf möglichen Unterstützungsbedarf erkennen kann. Eine entsprechende Funktion darf erst nach fachlicher Validierung und Festlegung geeigneter Qualitäts- und Kontrollkriterien spezifiziert werden.

3. Offene Fragen

Welche Daten sind verfügbar? Wie wird Unterstützungsbedarf definiert? Welche Fehlerquoten wären vertretbar? Welche Konsequenzen hätte eine fehlerhafte Einschätzung?

4. Empfohlene Strategie: RECONSIDER
KI Version – REQ-007
1. Qualitätsmängel

Der Begriff „sämtliche Benachrichtigungen“ ist zu weit gefasst. Es besteht ein direkter Konflikt mit REQ-008. Ohne eine Klassifizierung der Benachrichtigungen kann die Anforderung nicht widerspruchsfrei umgesetzt werden.

2. Verbesserte Anforderung

Der Study Buddy muss Studierenden die Verwaltung ihrer Benachrichtigungseinstellungen ermöglichen. Die Deaktivierbarkeit einzelner Benachrichtigungskategorien ist auf Grundlage einer abgestimmten Klassifizierung festzulegen. Verpflichtende Benachrichtigungen sind, sofern fachlich oder rechtlich erforderlich, gesondert zu behandeln.

3. Offene Fragen

Welche Kategorien existieren? Welche Mitteilungen sind verpflichtend? Welche Zustellkanäle werden verwendet? Wie wird der Konflikt mit REQ-008 aufgelöst?

4. Empfohlene Strategie: INVESTIGATE
KI Version – REQ-009
1. Qualitätsmängel

Die Anforderung berücksichtigt weder das Prinzip der Datenminimierung noch die Zweckbindung und rollenbasierte Zugriffsbeschränkung. Die Notwendigkeit des vollständigen Zugriffs ist nicht nachgewiesen.

2. Verbesserte Anforderung

Ein Zugriff der Studiengangsleitung auf personenbezogene Lernaktivitätsdaten darf nur für festgelegte, rechtmäßige Zwecke und im erforderlichen Umfang vorgesehen werden. Vor der Umsetzung sind ein Berechtigungskonzept, die zulässigen Datenkategorien sowie die rechtlichen Voraussetzungen der Verarbeitung festzulegen.

3. Offene Fragen

Welche Daten werden benötigt? Welche Rechtsgrundlage ist anwendbar? Welche Rollen benötigen welche Berechtigungen? Können aggregierte Daten verwendet werden?

4. Empfohlene Strategie: RECONSIDER
KI Version – REQ-015
1. Qualitätsmängel

Die Anforderung legt eine vollständig automatisierte Entscheidung fest, ohne die Entscheidungsgrundlagen, die fachliche Validierung und die Auswirkungen auf Studierende zu definieren. Menschliche Kontrollmöglichkeiten und Anforderungen an Transparenz fehlen.

2. Verbesserte Anforderung

Vor dem Einsatz eines KI-Modells zur Erkennung möglichen Betreuungsbedarfs sind die fachliche Eignung, die rechtliche Zulässigkeit und die Qualität der verwendeten Daten zu prüfen. Es ist festzulegen, ob das System ausschließlich Entscheidungshilfen bereitstellen darf und welche menschlichen Kontroll- und Korrekturmechanismen erforderlich sind.

3. Offene Fragen

Welche Daten werden verwendet? Wie wird Betreuungsbedarf definiert? Wer trägt die Entscheidungsverantwortung? Wie werden Fehlentscheidungen erkannt und korrigiert?

4. Empfohlene Strategie: RECONSIDER

Runde 3

Bewertungskriterien Human REQ-002
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 4
- Vollständigkeit und Überprüfbarkeit: 3 
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 4
  Gesamt: 21/25

Bewertungskriterien KI REQ-002
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 4
  Gesamt: 23/25

Begründung:
In beiden Versionen wird darauf eingegangen, dass die Definition der Begriffe schnell, intuitiv und benutzerfreundlich fehlt. In der menschlichen Version wird auf die Einbindung der Studierenden eingegangen, wohingegen sich die KI eher auf die Dokumentationsqualität konzentriert. Die KI schneidet allerdings etwas besser ab, da die Qualitätsmerkmale genauer beschrieben sind. 

Bewertungskriterien Human REQ-004
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 4
  Gesamt: 23/25

  Bewertungskriterien KI REQ-002
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 4
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 4
  Gesamt: 22/25

Begründung:
In beiden Versionen wird die Zuverlässigkeit der Vorhersage kritisch hinterfragt. Die humane Version schneidet jedoch etwas besser ab, da konkret darauf eingegangen wird, dass die Anforderung in dieser Form nicht umsetzbar ist. 

Bewertungskriterien Human REQ-007
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 5
  Gesamt: 24/25

Bewertungskriterien KI REQ-007
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 5
  Gesamt: 24/25

Begründung:
Beide Versionen erkennen, dass die Anforderung aus REQ-007 derer aus REQ-008 inhaltlich widerspricht und daher kritisch zu betrachten und zu hinterfragen ist. In beiden Versionen wird die aufgezeigt, dass es wichtig ist, dass Mitteilungen kategorisiert werden sollen und klar definiert werden soll, welche Mitteilungen sich deaktivieren lassen und welche nicht. Da in beiden Versionen auf den Widerspruch sowie die notwendigen Schritte eingegangen wird, sind beide gleich zu bewerten. 

Bewertungskriterien Human REQ-009
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 5
  Gesamt: 24/25
  
Bewertungskriterien KI REQ-009
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 5
  Gesamt: 24/25

Begründung:
In beiden Versionen wird der uneingeschränkte Zugriff auf Lernaktivitäten höchst kritisch betrachtet. In beiden Versionen wird darauf eingegangen, dass sowohl der Grund als auch die rechtlichen Grundlagen von essentieller Wichtigkeit sind, bei der Umsetzung dieser Anforderungen. In der KI Version werden zwar präzisere Fachbegriffe verwendet, allerdings unterstreicht die humane Version die Wichtigkeit von transparenter Vorgehensweise und deutlicher Begründung. 

Bewertungskriterien Human REQ-015
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 5
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 5
  Gesamt: 24/25

Bewertungskriterien KI REQ-015
- Fachliche Angemessenheit: 5
- Eindeutigkeit und Verständlichkeit: 4
- Vollständigkeit und Überprüfbarkeit: 4
- Umgang mit Annahmen: 5
- Abstimmung und Konflikte: 5
  Gesamt: 23/25

Begründung:
Beide Versionen bertrachten einen voll automatisierten Prozess über den Betreuungsbedarf kritisch. In der humanen Version wird vor allem der menschliche Aspekt in Form einer Kontrollinstanz betont. Die KI-Version bleibt hierbei eher oberflächlicher. Daher der kleine Vorsprung für die humane Version. 

Gesamtergebnis:
Humane Version: 23,2 Punkte
KI-Version: 23,2 Punkte

Runde 4

Finale Version REQ-002

Strategie: INVESTIGATE

Anforderung:
Die Benutzeroberfläche des Study Buddys soll benutzerfreundlich sein und effizientes Arbeiten ermöglichen. Die Anforderungen im Hinblick auf Antwortzeiten, Bedienbarkeit und Benutzerfreundlichkeit werden im Rahmen von Befragungen der Studierenden eingeholt. 

Offene Fragen:
- Welche Funktionen müssen besonders schnell reagieren?
- Welche Antwortzeiten sind akzeptabel?
- Woran soll die Benutzerfreundlichkeit gemessen werden?

Status: 
Offen weil Konkretisierungsbedarf.

Finale Version REQ-004

Strategie: RECONSIDER  

Anforderung:
Die Anforderung wird in dieser Form nicht angenommen und folglich auch nicht umgesetzt. Alternativ soll untersucht werden, ob die vorhandenen Learning-Analytics-Daten zum einen rechtmäßig verwendbar sind und zum anderen ob sich Hinweise auf Betreuungsunterstützung ableiten lassen.  

Offene Fragen:
- Welche Daten stehen zur Verfügung?
- Wie lässt sich der Unterstützungsbedarf definieren?
- Wie wird mit Fehleinschätzungen umgegangen?

Status: 
Zurückgestellt, da essentielle Teile der Anforderung überarbeitet werden müssen. 

Finale Version REQ-007

Strategie: INVESTIGATE    

Anforderung:
Die Mitteilungseinstellungen sollen grundsätzlich von den Studierenden selbst verwaltet werden. Dabei sollen die Benachrichtigungen kategorisiert werden, da die Deaktivierung nicht bei allen Kategorien möglich sein soll. Dabei gilt es insbesondere den Widerspruch zwischen REQ-007 und REQ-008 abzustimmen.  

Offene Fragen:
- Welche Benachrichtigungskategorien sollen definiert werden?
- Welche Kategorien sollen nicht deaktivierbar sein?

Status: 
Offen, da die Kategorien definert werden müssen und der Widerspruch zwischen REQ-007 und REQ-008 abgestimmt werden muss. 

Finale Version REQ-009

Strategie: RECONSIDER  

Anforderung:
Die Anforderung in ihrer ursprünglichen Form wird nicht umgesetzt. Vor einer neuen Anforderungsdefintion muss abgestimmt werden, welche Informationen in welchem Umfang und in welcher Form verarbeitet werden dürfen - und warum?   

Offene Fragen:
- Welche Daten sind erforderlich?
- Welche Begründung gibt es für den Zugriff auf die Lernaktivität der Studierenden?
- Wie sieht die Berechtigungsmatrix aus?

Status: 
Zurückgestellt, da essentielle Teile der Anforderung überarbeitet werden müssen. 

Finale Version REQ-015

Strategie: RECONSIDER  

Anforderung:
Die Anforderung wird in dieser Form nicht angenommen und folglich auch nicht umgesetzt. Zuerst ist zu prüfen wie sinnvoll eine solche KI-gestützte Analyse tatsächlich ist und ob diese überhaupt rechtskonform und technisch umsetzbar ist. Alternativ könnten im Study Buddy Hinweise angezeigt werden, welche auf Unterstützungsbedarf hindeuten und welche dann von den zuständigen Persinen geprüft wird. 

Offene Fragen:
- Welche Daten dürfen verwendet werden?
- Wer übernimmt die Verantwortung für die Überprüfung der Datenqualität?
- Wie werden falsche Einschätzungen gehandhabt und korrigiert?

Status: 
Zurückgestellt, da essentielle Teile der Anforderung überarbeitet werden müssen. 


## Teil 5 - Reflexion: Wer hat gewonnen?

**Ergebnis Runde 3:** Unentschieden. Beide Versionen kommen im Schnitt auf **23,2 von 25 Punkten** (je 116/125).
| REQ | Human | KI | Vorsprung |
|---|---|---|---|
| REQ-002 | 21 | 23 | KI |
| REQ-004 | 23 | 22 | Human |
| REQ-007 | 24 | 24 | – |
| REQ-009 | 24 | 24 | – |
| REQ-015 | 24 | 23 | Human |

Die KI hat bei allen fünf Requirements dieselbe Strategie gewählt wie wir (INVESTIGATE für REQ-002 und REQ-007, RECONSIDER für REQ-004, REQ-009 und REQ-015).
### 1. Bei welchen Qualitätskriterien war die KI besonders hilfreich, wo weniger zuverlässig?
**Hilfreich:**
- **Eindeutigkeit und Fachsprache:** Die KI hat Mängel präzise benannt, z. B. bei REQ-002 „subjektive und nicht operationalisierte Qualitätsbegriffe“ oder bei REQ-009 „Datenminimierung“, „Zweckbindung“ und „rollenbasierte Zugriffsbeschränkung“. Bei REQ-002 war die KI-Version deshalb klarer als unsere (5 vs. 4 Punkte).
- **Überprüfbarkeit:** Bei REQ-002 hat die KI explizit festgehalten, dass die Anforderung erst als vollständig spezifiziert gilt, wenn Antwortzeitgrenzen und Usability-Akzeptanzkriterien festgelegt sind. Das ist eine gute Abnahmebedingung (4 vs. 3 Punkte).
- **Zusätzliche offene Fragen:** Die KI hat Aspekte ergänzt, die wir nicht hatten, z. B. die Frage nach den **Zustellkanälen** (REQ-007), nach **aggregierten Daten** (REQ-009) und danach, ob das System bei REQ-015 **ausschließlich Entscheidungshilfen** bereitstellen soll.

**Weniger zuverlässig:**
- **Verständlichkeit bei RECONSIDER-Fällen:** Bei REQ-004 und REQ-015 sind die „verbesserten Anforderungen“ der KI eigentlich Prüfaufträge („Vor einer Implementierung ist zu prüfen, ob …“). Sie klingen verbindlich, beschreiben aber keine Systemfunktion. Begriffe wie „statistisch belastbare Hinweise“ oder „fachliche Validierung“ bleiben unbestimmt (jeweils nur 4 Punkte bei Eindeutigkeit).
- **Vage Einschränkungen:** Formulierungen wie „sofern fachlich oder rechtlich erforderlich“ (REQ-007) oder „für festgelegte, rechtmäßige Zwecke“ (REQ-009) verschieben die Unklarheit nur, statt sie offen als Frage zu markieren.
- **Projektkontext:** Die KI kannte weder unsere Stakeholder-Analyse (D2) noch die Rahmenbedingungen aus 02b. Sie konnte daher keine Stakeholder für die offenen Fragen benennen und keine konkreten Konflikte (z. B. Studierendenvertretung vs. Studiengangsleitung) aufzeigen.
### 2. Hat die KI Informationen ergänzt, die aus der Aufgabenstellung nicht hervorgingen?

Nein, nicht im kritischen Sinn. Die KI hat **keine Zahlen, Zielwerte, Technologien oder Stakeholder-Entscheidungen erfunden**. Bei REQ-002 hat sie z. B. keine konkrete Antwortzeit gesetzt, und bei REQ-004 keine Mindestgenauigkeit, sondern nach „akzeptablen Fehlerraten“ gefragt.

Wir führen das stark auf unseren Prompt zurück, der ausdrücklich verlangt hat: „Erfinde keine Stakeholderbedürfnisse, Interviewergebnisse, rechtlichen Freigaben oder technischen Rahmenbedingungen.“ Unsere Erkenntnis ist daher: **Die Qualität der KI-Antwort hängt stark davon ab, wie genau man ihr die Grenzen vorgibt.** Ob die KI ohne diese Einschränkung ebenfalls so vorsichtig gewesen wäre, haben wir nicht getestet.

Ergänzt hat die KI lediglich Fachbegriffe und Konzepte (Zielvariable, Berechtigungskonzept, Korrekturmechanismen). Diese sind fachlich passend, aber ebenfalls nicht durch Stakeholder bestätigt.

### 3. Hat die KI nur sprachlich verbessert oder auch die Notwendigkeit hinterfragt?

Sie hat auch die **Notwendigkeit hinterfragt**. Bei REQ-004, REQ-009 und REQ-015 hat sie RECONSIDER empfohlen. Bei REQ-009 schreibt sie ausdrücklich, dass die Notwendigkeit des vollständigen Zugriffs nicht nachgewiesen ist. Bei REQ-004 hat sie, wie wir, das Ziel von „Abbruch vorhersagen“ auf „Unterstützungsbedarf erkennen“ verschoben.

Der Unterschied liegt in der Konsequenz: Wir haben klar formuliert, dass die Anforderung **in dieser Form nicht übernommen** wird. Die KI liefert trotzdem eine „verbesserte Anforderung“, die wie ein Ersatz-Requirement wirkt. Das kann in der Praxis dazu verleiten, eine eigentlich zurückgestellte Anforderung doch in die Entwicklung zu geben.

### 4. Gab es Fälle, in denen unsere Human Version überzeugender war? Warum?

Ja, bei **REQ-004** und **REQ-015**:
- **REQ-004:** Unsere Version hält eindeutig fest, dass die Anforderung in dieser Form nicht umsetzbar ist, und begründet dies (Prognose ist immer nur eine Wahrscheinlichkeit). Die KI-Version bleibt bei einem allgemeinen Prüfauftrag.
- **REQ-015:** Wir haben die **menschliche Kontrollinstanz** als zentrales Problem herausgearbeitet und konkret gefragt, wer sie ist und wer die Datenqualität prüft. Die KI nennt Kontrollmechanismen nur allgemein.

Der Hauptgrund: Wir kannten den Projektkontext aus D2 (z. B. die Forderung von Datenschutz, dass Studierende nicht automatisch als gefährdet eingestuft werden, und die Bedenken der Lehrendenvertretung zu Verantwortung). Die KI hatte nur den Anforderungstext.

Selbstkritisch: Bei **REQ-002** war die KI besser. Unsere Version formuliert „werden Befragungen mit den Studierenden durchgeführt“ als feststehende Tatsache, obwohl das noch nicht entschieden ist. Außerdem fehlte eine klare Abnahmebedingung.

### 5. Welche Rolle sollte generative KI künftig bei der Qualitätssicherung von Requirements spielen?

Generative KI ist als **zweiter Prüfer** sinnvoll, nicht als Entscheidungsinstanz:
- **Geeignet für:** Erkennen vager Begriffe, präzisere Fachsprache, Vorschläge für Akzeptanzkriterien und zusätzliche offene Fragen, die man selbst übersehen hat.
- **Nicht geeignet für:** Entscheidungen über Notwendigkeit oder Zulässigkeit, Festlegen von Zielwerten, Auflösen von Stakeholder-Konflikten.

Voraussetzungen für einen sinnvollen Einsatz:
1. Ein **klarer Prompt**, der das Erfinden von Informationen ausdrücklich verbietet (bei uns entscheidend).
2. Möglichst **Projektkontext mitgeben** (Stakeholder-Analyse, Rahmenbedingungen), sonst bleiben Abstimmungsfragen allgemein.
3. **Menschliche Prüfung jeder KI-Ausgabe**, besonders bei Formulierungen, die verbindlich klingen, aber offen sind.

### Fazit

Punktemäßig gibt es keinen Sieger. Inhaltlich hat jede Seite eigene Stärken: Die KI formuliert präziser und denkt an zusätzliche Aspekte, wir bringen den Projektkontext ein und ziehen bei problematischen Anforderungen klarere Konsequenzen. Die besten Ergebnisse entstanden in der Kombination, wie die finalen Versionen in Runde 4 zeigen.  









