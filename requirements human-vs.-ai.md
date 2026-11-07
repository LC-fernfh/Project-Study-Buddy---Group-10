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



  









