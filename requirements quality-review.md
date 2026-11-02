Requirement-ID: REQ-001
Qualitätsaspekt: Inhalt
Qualitätskriterium: Überprüfbarkeit und Eindeutigkeit.
Fehlerbeschreibung: Die Anforderung ist zu vage formuliert. Was genau bedeutet „aktiv“ im Online Campus? Zählt bereits ein reiner Login, der Aufruf einer Kursseite oder das Abgeben einer Aufgabe? Außerdem ist unklar, wie die Benachrichtigung erfolgen soll (per E-Mail?, per Push-Nachricht?, per SMS?) und zu welcher Uhrzeit bzw. nach wie vielen Stunden Inaktivität exakt der Trigger greift.
Mögliche Konsequenz: Entwickler und Tester können nicht eindeutig überprüfen, ob das System die Anforderung erfüllt. Das führt zu Fehlinterpretationen bei der Umsetzung und zu Frust bei den Nutzern (z. B. wenn Studierende trotz des Logins fälschlicherweise eine Benachrichtigung erhalten oder wichtige Nachrichten zu spät kommen).
Fehlende Informationen:
Definition von „Aktivität“ (Welche Aktionen setzen den Inaktivitäts-Timer zurück?).
Festlegung des Kommunikationskanals (E-Mail, In-App-Benachrichtigung, SMS).
Timing-Spezifikation (Exakter Zeitpunkt am siebten Tag, z. B. morgens um 08:00 Uhr oder genau nach 168 Stunden).


Requirement-ID: REQ-002
Qualitätsaspekt: Inhalt 
Qualitätskriterium: Prüfbarkeit und Eindeutigkeit
Fehlerbeschreibung: Die Anforderung enthält reine Buzzwords und subjektive Qualitätsbegriffe. Begriffe wie „schnell“ oder „benutzerfreundlich“ sind nicht messbar, da jeder Mensch sie anders empfindet.
Mögliche Konsequenz: Die Anforderung ist absolut nicht testbar. Weder Entwickler noch Tester können objektiv nachweisen oder überprüfen, ob das System „benutzerfreundlich“ oder „schnell“ genug ist. Dies führt unweigerlich zu Streitpunkten.
Fehlende Informationen:
Konkrete Messwerte für die Performance.
Messbare Kriterien für die Usability.


Requirement-ID: REQ-003
Qualitätsaspekt: Inhalt 
Qualitätskriterium: Eindeutigkeit & Vollständigkeit / Atomarität
Fehlerbeschreibung: Hier liegt ein klassischer „Mischmasch“-Fehler vor. In einem einzigen Satz werden vier komplett unterschiedliche Kernfunktionen des Systems vermischt: Die Anzeige von Abgaben, das versenden von Erinnerungen, die Lernfortschrittsanalyse und die Benachrichtigung von Lehrenden. Außerdem ist das Wort „Schwierigkeiten“ sehr vage.
Mögliche Konsequenz: Die Anforderung lässt sich nicht sauber aufteilen, testen oder umsetzen. Wenn beispielsweise Feature 1 und 2 fertig sind, aber Feature 4  aufgrund von Datenschutzbedenken oder technischer Komplexität scheitert, kippt oft das gesamte Requirement. Bei Fehlern im Test ist unklar, welcher Teilbereich genau betroffen ist.
Fehlende Informationen:
Aufteilung in eigenständige, atomare Requirements.
Präzise Definition des Begriffs „Schwierigkeiten“ .
Spezifikation der Bedingungen für Erinnerungen.


Requirement-ID: REQ-004
Qualitätsaspekt: Inhalt 
Qualitätskriterium: Realisierbarkeit und Eindeutigkeit / Messbarkeit
Fehlerbeschreibung: Die Anforderung enthält gleich zwei massive Probleme:
Absolutheit & unrealistischer Anspruch: Das Wort „zuverlässig“ suggeriert eine Fehlerquote von 0 %. Eine KI-basierte Vorhersage über den Studienerfolg ist immer nur eine Wahrscheinlichkeit
Unklare Definition & Kriterien: Es ist völlig offen, anhand welcher Indikatoren die KI diesen Zustand feststellen soll und wann genau diese Vorhersage getroffen werden muss.
Mögliche Konsequenz:
Wirtschaftlich/Technisch: Das Ziel ist technologisch nicht erreichbar, was zu gescheiterten Projekten führt.
Ethisch/Rechtlich: Falsch-positive Vorhersagen können zu Stigmatisierung, unberechtigtem Druck oder Datenschutzverstößen führen.
Fehlende Informationen:
Angabe einer akzeptablen Mindestgenauigkeit muss mindestens X % betragen“).
Definition des genauen Zeitpunkts der Prognose .
Festlegung der Datenbasis.


Requirement-ID: REQ-005
Qualitätsaspekt: Inhalt und Dokumentation
Qualitätskriterium: Realisierbarkeit, Konsistenz & Robustheit
Fehlerbeschreibung: Die Anforderung ist auf den ersten Blick zwar sehr konkret, ignoriert jedoch völlig technische Realitäten und Systemgrenzen:
Performance-Flaschenhals: Wenn alle Studierenden exakt zur gleichen Sekunde eine personalisierte E-Mail erhalten sollen, führt das zu einer massiven Lastspitze auf dem E-Mail-Server. Das System droht abzustürzen oder Mails stark verzögert auszuliefern.
Fehlende Ausnahmefälle: Es wird nicht definiert, was mit Studierenden passiert, die exmatrikuliert oder länger krank sind, oder ob Studierende diese E-Mails überhaupt abbestellen können.
Mögliche Konsequenz:
Der E-Mail-Server wird vom Spam-Filter anderer Anbieter geblockt, weil Tausende E-Mails gleichzeitig eintrudeln.
Rechtliche Probleme bei fehlender Abbestellmöglichkeit.
Technische Überlastung des Systems zu Wochenbeginn.
Fehlende Informationen:
Festlegung eines Zeitfensters statt eines harten Punkts.
Definition eines Opt-out-Mechanismus für Studierende, die diesen wöchentlichen Report nicht erhalten möchten.
Umgang mit Sonderstatus.


Requirement-ID: REQ-006
Qualitätsaspekt: Inhalt
Qualitätskriterium: Eindeutigkeit und Vollständigkeit
Fehlerbeschreibung: Die Anforderung enthält gleich zwei undefinierte Begriffe:
Kritischer Lernrückstand: Es ist absolut unklar, ab welchem Schwellenwert ein Rückstand als „kritisch“ gilt.
„Geeignete Maßnahmen“: Es wird komplett offen gelassen, was das System in diesem Fall tun soll.
Mögliche Konsequenz: Die Anforderung ist unbrauchbar für die Umsetzung. Entwickler können keine Programmlogik schreiben, wenn weder die Bedingungen noch die Aktionen definiert sind.
Fehlende Informationen:
Präzise Definition und Messbarkeit des „kritischen Lernrückstands“.
Exakte Festlegung der automatisierten Maßnahmen.
Klärung, ob und wer diesen Maßnahmen zustimmen muss, bevor diese greifen.


Requirement-ID: REQ-007
Qualitätsaspekt: Inhalt & Abgestimmtheit
Qualitätskriterium: Konsistenz und Vollständigkeit
Fehlerbeschreibung:
Logischer Widerspruch: Die Anforderung fordert absolut. Wenn jedoch sicherheitsrelevante oder systemkritische Nachrichten ebenfalls komplett abgeschaltet werden können, führt das zu massiven organisatorischen Problemen.
Fehlende Granularität: Es wird nicht unterschieden zwischen verschiedenen Benachrichtigungskategorien.
Mögliche Konsequenz:
Studierende schalten alle Benachrichtigungen aus und verpassen dadurch wichtige Fristen oder Prüfungsänderungen und machen anschließend die FH oder das System dafür verantwortlich.
Rechtliche oder hochschulrechtliche Konflikte, da wichtige Informationen den Studierenden nachweisbar erreicht haben müssen.
Fehlende Informationen:
Ausnahmen: Welche Benachrichtigungen sind von der Deaktivierung ausgeschlossen?
Spezifikation der Benachrichtigung-Einstellungen. 


Requirement-ID: REQ-008
Qualitätsaspekt: Inhalt & Abgestimmtheit
Qualitätskriterium: Konsistenz und Eindeutigkeit
Fehlerbeschreibung:
Direkter Widerspruch zu REQ-007: In REQ-007 wurde gefordert, dass Studierende sämtliche Benachrichtigungen jederzeit deaktivieren können. Nun besagt REQ-008 das genaue Gegenteil für bestimmte Fälle. Ohne eine genaue Definition spielen diese Anforderungen gegeneinander.
Unklare Begrifflichkeit: Der Begriff „kritische Studienereignisse“ ist nicht definiert.
Mögliche Konsequenz:
Entwicklungs- und Testkonflikt: Entwickler wissen nicht, welche Logik im Benachrichtigungscenter Vorrang hat.
Datenschutz- / Akzeptanzrisiko: Wenn das System trotz deaktivierter Benachrichtigungen Nachrichten sendet, ohne dass klar definiert ist, was ein „kritisches Ereignis“ rechtfertigt, führt das zu Verwirrung und Beschwerden der Studierenden.
Fehlende Informationen:
Explizite Definition und Liste dessen, was rechtlich/organisatorisch als „kritisches Studienereignis“ gilt.
Klare Regelung des Verhältnisses zu REQ-007.
Festlegung des Kommunikationskanals für diese Notfall-Benachrichtigungen.


Requirement-ID: REQ-009
Qualitätsaspekt: Inhalt & Dokumentation
Qualitätskriterium: Konformität und Vollständigkeit
Fehlerbeschreibung:
Datenschutzrechtlicher Verstoß: Die Forderung, dass die Studiengangsleitung jederzeit auf sämtliche individuellen Lernaktivitäten aller Studierenden zugreifen kann, verstößt gegen die Grundsätze der Datenminimierung und den Schutz personenbezogener Daten. Eine lückenlose Überwachung des Lernverhaltens ist rechtlich unzulässig.
Unklare Zweckbindung: Es ist nicht definiert, aus welchem Grund und mit welchen Berechtigungsstufen dieser Zugriff erfolgen soll.
Mögliche Konsequenz:
Das Projekt scheitert an der Freigabe durch den/die Datenschutzbeauftragte:n.
Rechtliche Konsequenzen aufgrund der Verletzung der Privatsphäre der Studierenden.
Kompletter Vertrauensverlust der Studierenden in das Study-Buddy-System.
Fehlende Informationen:
Einschränkung des Zugriffs auf anonymisierte oder aggregierte Daten.
Definition von strikten Berechtigungskonzepten und rechtlichen Grundlagen.
Transparenzhinweis für Studierende, welche Daten erfasst und wem zugänglich gemacht werden.


Requirement-ID: REQ-010
Qualitätsaspekt: Inhalt & Dokumentation
Qualitätskriterium: Eindeutigkeit, Vollständigkeit und Technische Realisierbarkeit
Fehlerbeschreibung:
Unpräzise Quellenangabe: Der Begriff „bestehende Systeme“ ist sehr vage. Welche Systeme sind konkret gemeint? Es wird offengelassen, ob diese Systeme überhaupt über funktionierende Schnittstellen verfügen.
Unklare Datenhoheit und Synchronisation: Es ist nicht definiert, wie oft diese automatische Übernahme stattfinden soll und was passiert, wenn Daten in den Quellsystemen fehlerhaft sind oder sich kurzfristig ändern.
Mögliche Konsequenz:
Entwickler stehen vor einem unlösbaren Rätsel, da unklar ist, welche Schnittstellen angebunden werden müssen.
Sollten an den Altsystemen keine geeigneten APIs existieren, kann die „automatische Übernahme“ zu massiven, unvorhersehbaren Mehraufwänden oder zum technischen Scheitern der Integration führen.
Fehlende Informationen:
Nennung der konkreten Quellsysteme inklusive technischer Dokumentation oder Schnittstellen-Spezifikationen.
Definition des Synchronisationsintervalls.
Festlegung der Datenpriorität.


Requirement-ID: REQ-011
Qualitätsaspekt: Inhalt & Abgestimmtheit 
Qualitätskriterium: Konsistenz und Benutzerfreundlichkeit / Wirtschaftlichkeit
Fehlerbeschreibung:
Konstruktionswiderspruch: In REQ-010 wurde gefordert, dass Daten vollautomatisch aus den bestehenden Systemen übernommen werden. Wenn Studierende sich nun einen separaten Account mit eigenem Passwort anlegen müssen, gibt es keine verlässliche ID-Verknüpfung zu den bestehenden Hochschulsystemen.
Mögliche Konsequenz:
Massive Akzeptanzprobleme bei den Studierenden, da ein weiterer Account verwaltet werden muss.
Hoher administrativer Aufwand und Sicherheitsrisiken.
Technische Probleme bei der Datenzusammenführung aus dem Altsystemen.
Fehlende Informationen:
Prüfung, ob stattdessen eine Single-Sign-On-Anbindung verwendet werden kann/muss.
Spezifikation, wie die Identität bei einem separaten Konto verifiziert wird.


Requirement-ID: REQ-012
Qualitätsaspekt: Inhalt
Qualitätskriterium: Eindeutigkeit, Realisierbarkeit und Messbarkeit
Fehlerbeschreibung:
Überhöhter Anspruch: Das Wort „optimal“ gibt an, dass es für jede Person zu jedem Zeitpunkt exakt einen perfekten, unfehlbaren Lernpfad gibt. Lernen ist jedoch subjektiv.
Unklare Parameter & Intransparenz: Es wird völlig offen gelassen, auf Basis die Daten berechnet werden und wie transparent dies für die Studierenden sein muss.
Mögliche Konsequenz:
Akzeptanz- und Vertrauensproblem: Wenn das System pauschale oder unpassende Lerntipps gibt, verlieren Studierende das Vertrauen in die KI.
Technisches Risiko: Entwickler können kein System bauen, das ein Konzept einer „optimalen Lernstrategie“ abbildet.
Fehlende Informationen:
Präzisierung des Begriffs: Was  ist eine Strategie?
Festlegung der Kriterien, wann welche Empfehlung ausgesprochen werden soll.
Angaben, ob Studierende diesen Empfehlungen widersprechen oder eigene Präferenzen einstellen können.


Requirement-ID: REQ-013
Qualitätsaspekt: Inhalt & Abgestimmtheit
Qualitätskriterium: Konsistenz, Zuverlässigkeit und Nachvollziehbarkeit
Fehlerbeschreibung:
Fehlende Transparenz & Risiko von „stummen“ Fehlern: Wenn Abgabetermine im Hintergrund geändert werden, ohne dass der Studierende oder das System diese in irgendeiner Form aktiv markiert oder hervorhebt, besteht die Gefahr, dass Friständerungen übersehen werden.
Fehlende Protokollierung: Es ist nicht definiert, ob für diese automatischen Änderungen eine Änderungshistorie geführt werden muss, damit Studierende im Streitfall nachvollziehen können, warum sich ein Termin verschoben hat.
Mögliche Konsequenz:
Studierende verpassen Abgaben oder Prüfungen, weil sich ein Termin im Hintergrund verschoben hat und diese nicht darauf aufmerksam gemacht wurden.
Bei fehlerhaften Daten aus den Quellsystemen übernimmt der Study Buddy ungeprüft falsche Fristen und kann damit den Studierenden schaden.
Fehlende Informationen:
Festlegung, ob trotz automatischer Übernahme eine Benachrichtigung erfolgen muss.
Definition eines Protokolls oder einer Historie, in der automatische Änderungen für den Studierenden einsehbar sind.


Requirement-ID: REQ-014
Qualitätsaspekt: Inhalt & Dokumentation
Qualitätskriterium: Eindeutigkeit, Messbarkeit und Realisierbarkeit
Fehlerbeschreibung:
Absolutheitsanspruch & undefinierter Standard: Die Formulierung „vollständig barrierefrei“ ist ein kaum messbarer Begriff. Es wird offengelassen, welcher genaue Barrierefreiheitsstandard eingehalten werden muss.
Unklare Gerätespezifikation: „Alle Geräte“ ist zu weit gefasst und technisch kaum realistisch.
Mögliche Konsequenz:
Rechtliches & vertragliches Risiko: Da „vollständig barrierefrei“ im Streitfall oder Abnahmetest nicht absolut nachgewiesen werden kann, können rechtliche Probleme drohen.
Entwicklungsaufwand: Entwickler wissen nicht, welche spezifischen Hilfstechnologien unterstützt werden müssen.
Fehlende Informationen:
Nennung eines verbindlichen Standards.
Definition der Ziel-Geräte und -Browser, die offiziell unterstützt werden müssen.
Spezifikation, welche Barrierefreiheits-Features priorisiert umgesetzt werden.


Requirement-ID: REQ-015
Qualitätsaspekt: Inhalt & Dokumentation
Qualitätskriterium: Eindeutigkeit, Realisierbarkeit und Verantwortlichkeit
Fehlerbeschreibung:
Vollautomatisierte Entscheidung ohne menschliche Kontrolle: Das System soll laut Formulierung automatisch entscheiden, wer zusätzliche Betreuung benötigt. Das entzieht Lehrenden die Entscheidungsgewalt und übergibt sensible, pädagogische Maßnahmen vollständig an eine Black-Box-KI.
Verstoß gegen Datenschutzvorgaben: Vollautomatisierte Entscheidungen, die rechtliche oder ähnlich schwerwiegende Beeinträchtigungen für Einzelpersonen zur Folge haben und ist rechtlich unzulässig.
Fehlende Erklärbarkeit: Es wird nicht spezifiziert, ob und wie die KI begründen muss, warum eine Person Betreuung braucht.
Mögliche Konsequenz:
Rechtliches Risiko: Das Projekt scheitert an rechtlichen Hürden bezüglich automatisierter Entscheidungsfindung und Datenschutz.
Pädagogischer Schaden: Falsche Einschätzungen der KI führen zu Frust, Fehlbetreuung und Vertrauensverlust.
Fehlende Informationen:
Definition eines „Human-in-the-Loop“-Prinzips.
Spezifikation der genauen Datenbasis und der Erklärbarkeit der KI-Entscheidung.
Einhaltung rechtlicher Rahmenbedingungen und Einwilligungserklärungen der Studierenden.











