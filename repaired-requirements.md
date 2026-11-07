## REQ-001 – The Seven-Day Rule

**Original:**
> „Das System muss Studierende automatisch benachrichtigen, wenn sie sieben Tage lang nicht im Online Campus aktiv waren.“

**Qualitätsmangel:**
- **Eindeutigkeit:** Es ist nicht definiert, was „aktiv“ bedeutet (Login, Aufruf von Kursseiten, Abgaben …).
- **Unbegründete Annahme:** Die Anforderung setzt voraus, dass fehlende Aktivität im Online Campus bedeutet, dass nicht gelernt wird. Die Studierendenvertretung hat in D2 genau davor gewarnt: Berufsbegleitend Studierende lernen oft geblockt und offline.
- **Fehlende Begründung:** Woher die Schwelle von sieben Tagen kommt und ob sie für alle Studiengänge und Semesterphasen passt, ist nicht belegt.
- **Vollständigkeit:** Kanal, Inhalt und Abschaltbarkeit der Benachrichtigung fehlen. Ob die Benachrichtigung abschaltbar ist, hängt außerdem mit REQ-007/008 zusammen.
- **Abgestimmtheit:** Hier besteht ein Zielkonflikt zwischen Studiengangsleitung (Frühwarnung) und Studierendenvertretung (keine Überwachung, keine Erinnerungsflut).

**Strategie:** **INVESTIGATE**

**Offene Fragen:**
1. Welche Aktionen gelten als „Aktivität“, und welche Aktivitätsdaten stellt der Online Campus überhaupt zur Verfügung? → *IT & Online-Campus-Team*
2. Ist es zulässig, Aktivitätsdaten für diesen Zweck auszuwerten, und auf welcher Rechtsgrundlage? → *Datenschutz & Informationssicherheit*
3. Wie lange lernen Studierende typischerweise, ohne den Online Campus zu öffnen? Ist eine Erinnerung nach Inaktivität für sie hilfreich oder störend? → *Studierende / Studierendenvertretung* (Fragebogen, siehe `elicitation`)
4. Welches Ziel verfolgt die Studiengangsleitung mit der Regel, und woher stammt der Wert von sieben Tagen? → *Studiengangsleitung*
5. Gibt es Lehrveranstaltungen, deren didaktischer Aufbau längere Phasen ohne Online-Aktivität vorsieht? → *Lehrendenvertretung*
6. Über welchen Kanal wird erinnert, und darf die Erinnerung deaktiviert werden (Bezug REQ-007)? → *Studierendenvertretung, IT*

**Ergebnis:**
Eine endgültige Neuformulierung ist noch nicht möglich, weil weder der Begriff „Aktivität“ noch die Schwelle noch die Zulässigkeit geklärt sind.
Strukturvorschlag für die spätere Formulierung (*Vorschlag – nicht validiert*):

---

## REQ-002 – Fast and Friendly

**Original:**
> „Der Study Buddy muss schnell, intuitiv und besonders benutzerfreundlich sein.“

**Qualitätsmangel:**
- **Prüfbarkeit / Eindeutigkeit:** „schnell“, „intuitiv“ und „besonders benutzerfreundlich“ sind subjektiv und nicht messbar. Kein Abnahmetest kann die Anforderung bestätigen oder widerlegen.
- **Atomarität:** Die Anforderung mischt Performance (schnell) und Usability (intuitiv, benutzerfreundlich).

**Strategie:** **INVESTIGATE** (die Struktur lässt sich schon verbessern, die Messwerte fehlen aber)

**Strukturierte Aufteilung (*Vorschlag – Werte offen*):**
- **REQ-002a (Performance):** „Das System muss `[OFFEN: welche Aktionen, z. B. Aufruf der Übersichtsseite]` innerhalb von `[OFFEN: Zeitwert]` unter `[OFFEN: Lastannahme]` ausführen.“
- **REQ-002b (Usability):** „Das System muss Studierenden die Möglichkeit bieten, `[OFFEN: Kernaufgaben]` ohne vorherige Schulung zu erledigen.“ Nachweis über `[OFFEN: Prüfmethode, z. B. Usability-Test mit Zielgruppe und Erfolgskriterium]`.

**Offene Fragen:**
1. Welche Aktionen müssen „schnell“ sein, und welche Antwortzeiten sind in der bestehenden Systemlandschaft realistisch? → *IT & Online-Campus-Team*
2. Was sind die Kernaufgaben, die Studierende mit dem Study Buddy erledigen wollen? → *Studierende / Studierendenvertretung*
3. Mit welcher Methode und welchem Erfolgskriterium soll Benutzerfreundlichkeit abgenommen werden? → *Studiengangsleitung (Auftraggeberin), Qualitätsmanagement*

**Ergebnis:**
Wir haben die Anforderung in zwei atomare Anforderungen aufgeteilt. Konkrete Zielwerte setzen wir bewusst **nicht** ein, weil dafür keine Grundlage vorliegt. Die Anforderung bleibt offen, bis Kernaufgaben und Messkriterien mit den Stakeholder*innen geklärt sind.

---

## REQ-003 – The All-in-One Feature

**Original:**
> „Das System muss bevorstehende Abgaben anzeigen, personalisierte Erinnerungen versenden, Lernfortschritte analysieren und Lehrende über Schwierigkeiten informieren.“

**Qualitätsmangel:**
- **Atomarität:** Vier unabhängige Funktionen stehen in einem Satz. Sie lassen sich nicht einzeln priorisieren, testen oder streichen.
- **Eindeutigkeit:** „bevorstehend“, „personalisiert“, „Lernfortschritt“ und „Schwierigkeiten“ sind undefiniert.
- **Abgestimmtheit:** Der vierte Teil (Lehrende informieren) berührt Datenschutz und die Rolle der Lehrenden. Die Lehrendenvertretung hat in D2 Bedenken zu Mehraufwand und Verantwortung geäußert.

**Strategie:** **REWRITE** (Aufteilung). Für die Teile b–d ist zusätzlich **INVESTIGATE** nötig.

**Überarbeitete Anforderungen:**

| Neue ID | Formulierung | Status |
|---|---|---|
| **REQ-003a** | „Das System muss Studierenden die Abgabetermine ihrer belegten Lehrveranstaltungen anzeigen, die innerhalb von `[OFFEN: Zeitraum]` fällig sind.“ | REWRITE. Die Funktion ist unstrittig; nur der Zeitraum ist offen. Datenquelle siehe REQ-010. |
| **REQ-003b** | „Das System muss Studierenden Erinnerungen an `[OFFEN: Ereignistypen]` senden.“ | INVESTIGATE. Was „personalisiert“ heißt, ist offen. Abhängig von REQ-007/008. |
| **REQ-003c** | „Das System muss Studierenden ihren Lernfortschritt in `[OFFEN: Lehrveranstaltung/Studium]` anzeigen, gemessen an `[OFFEN: Definition Lernfortschritt]`.“ | INVESTIGATE. Wie „Fortschritt“ definiert wird, bestimmen die Lehrenden je LV. |
| **REQ-003d** | „Lehrende über Schwierigkeiten informieren“ | RECONSIDER. Wir übernehmen das nicht ohne Klärung (siehe unten). |

**Offene Fragen:**
1. Welcher Vorlaufzeitraum macht eine Abgabe „bevorstehend“? → *Studierende, Studienadministration*
2. Was bedeutet „Lernfortschritt“ fachlich, und lässt er sich bei didaktisch unterschiedlich aufgebauten LVs einheitlich messen? → *Lehrendenvertretung*
3. REQ-003d: Was sind „Schwierigkeiten“? Dürfen Lehrende darüber personenbezogen informiert werden? Wer muss dann reagieren? → *Datenschutz, Lehrendenvertretung, Studiengangsleitung, Studierendenvertretung*

**Ergebnis:**
REQ-003a ist bis auf einen Parameter umsetzbar. Die Teile b und c bleiben offen. Teil d wird wegen seiner Nähe zu REQ-009 und REQ-015 (Überwachung, automatische Einstufung) vorerst zurückgestellt.

---

## REQ-004 – The Perfect Prediction

**Original:**
> „Das System muss zuverlässig erkennen, welche Studierenden ihr Studium nicht erfolgreich abschließen werden.“

**Qualitätsmangel:**
- **Realisierbarkeit:** Eine „zuverlässige“ Vorhersage des Studienabbruchs ist nicht möglich. Prognosen sind immer Wahrscheinlichkeiten und mit Fehlklassifikationen verbunden.
- **Prüfbarkeit:** Es fehlen Indikatoren, Zeitpunkt und Datenbasis.
- **Zulässigkeit / Angemessenheit:** Die Anforderung verlangt eine automatisierte Einstufung von Personen. Datenschutz hat in D2 ausdrücklich gefordert, dass Studierende *„nicht frühzeitig automatisch als gefährdet eingestuft werden“*. Die Studierendenvertretung befürchtet Fehldeutungen und Stigmatisierung.
- **Unklarer Zweck:** Es steht nicht da, was mit dem Ergebnis geschehen soll.

**Strategie:** **RECONSIDER**

**Begründung:**
Die Anforderung beschreibt eine **Lösung** (Abbruchprognose) und nicht das dahinterliegende **Ziel**. Laut D2 ist das Ziel der Studiengangsleitung, Lernrückstände früh zu erkennen und rechtzeitig Hilfe anzubieten. Eine Prognose darüber, wer „nicht erfolgreich abschließen wird“, ist dafür weder notwendig noch angemessen. Ob sie zulässig ist, ist ungeklärt. Würden wir die Anforderung jetzt präzisieren (etwa mit einer Mindestgenauigkeit in Prozent), müssten wir sowohl eine technische Machbarkeit als auch eine rechtliche Freigabe erfinden.

**Offene Fragen:**
1. Welches konkrete Problem soll gelöst werden, und welche Maßnahme soll auf eine Erkennung folgen? → *Studiengangsleitung*
2. Ist eine solche Profilbildung rechtlich zulässig, und unter welchen Bedingungen (Einwilligung, Transparenz, menschliche Prüfung)? → *Datenschutz & Informationssicherheit*
3. Liegen überhaupt Daten vor, die eine belastbare Aussage erlauben? → *IT & Online-Campus-Team*
4. Wie würden Studierende eine solche Einstufung wahrnehmen? → *Studierendenvertretung*

**Ergebnis:**
Die Anforderung wird **nicht übernommen**. Wir empfehlen, sie durch eine Anforderung zu ersetzen, die das eigentliche Ziel (frühe Unterstützung) beschreibt. Diese muss erst gemeinsam mit den Stakeholder*innen erhoben werden.

---

## REQ-007 / REQ-008 – The Notification Paradox & No Exceptions

**Originale:**
> REQ-007: „Studierende müssen sämtliche Benachrichtigungen jederzeit deaktivieren können.“
> REQ-008: „Das System muss alle Studierenden unabhängig von ihren Einstellungen über kritische Studienereignisse benachrichtigen.“

**Qualitätsmangel:**
- **Konsistenz:** Die beiden Anforderungen schließen sich gegenseitig aus. Sind *sämtliche* Benachrichtigungen abschaltbar, kann es keine geben, die *unabhängig von den Einstellungen* zugestellt wird.
- **Eindeutigkeit:** „kritische Studienereignisse“ ist nicht definiert.
- **Abgestimmtheit:** Hier treffen der Wunsch der Studierendenvertretung nach Kontrolle und Vermeidung von Informationsflut und das Interesse der Hochschule an verlässlicher Information aufeinander.

**Strategie:** **REWRITE** (der Widerspruch lässt sich strukturell auflösen) + **INVESTIGATE** (welche Ereignisse in welche Kategorie fallen, ist offen)

**Überarbeitete Anforderungen (*Struktur: REWRITE / Inhalt: offen*):**
- **REQ-007 (neu):** „Das System muss Studierenden die Möglichkeit bieten, Benachrichtigungen der Kategorie *optional* jederzeit einzeln zu deaktivieren.“
- **REQ-008 (neu):** „Das System muss Studierende über Ereignisse der Kategorie *verpflichtend* benachrichtigen, auch wenn sie optionale Benachrichtigungen deaktiviert haben.“
- **REQ-008b (neu):** „Das System muss Studierenden anzeigen, welche Benachrichtigungen verpflichtend sind und daher nicht deaktiviert werden können.“
- **Definition (offen):** Die Kategorie *verpflichtend* umfasst `[OFFEN: abschließende Liste der Ereignisse]`. Alle anderen Benachrichtigungen sind *optional*.

**Offene Fragen:**
1. Welche Ereignisse müssen Studierende nachweislich erreichen, z. B. aus hochschulrechtlichen Gründen? → *Studienadministration, Studiengangsleitung*
2. Gibt es solche Pflichtinformationen schon über andere Kanäle (z. B. E-Mail der Hochschule)? Dann müsste der Study Buddy sie gar nicht verpflichtend zustellen. → *Studienadministration, IT*
3. Ist eine nicht abschaltbare Benachrichtigung für Studierende akzeptabel, wenn die Liste kurz und transparent ist? → *Studierendenvertretung*

**Ergebnis:**
Der logische Widerspruch ist durch die Trennung in zwei Kategorien behoben. **Welche** Ereignisse verpflichtend sind, haben wir bewusst nicht festgelegt. Das ist eine Stakeholder-Entscheidung und kein Formulierungsproblem. Die neue Struktur betrifft auch REQ-001, REQ-003b, REQ-005 und REQ-013: Für jede dieser Benachrichtigungen ist festzulegen, zu welcher Kategorie sie gehört.

---

## REQ-009 – The Secret Dashboard

**Original:**
> „Die Studiengangsleitung muss jederzeit auf sämtliche individuellen Lernaktivitäten aller Studierenden zugreifen können.“

**Qualitätsmangel:**
- **Zulässigkeit / Konformität:** Ein unbeschränkter Zugriff auf *sämtliche individuellen* Lernaktivitäten widerspricht den Grundsätzen der Datenminimierung und Zweckbindung, die Datenschutz in D2 eingefordert hat („nur notwendige Daten“, „Zugriff begrenzt und kontrollierbar“, „nur ausgewählte Personen“).
- **Fehlender Zweck:** Wofür der Zugriff gebraucht wird, steht nicht da. Ohne Zweck lässt sich nicht beurteilen, welcher Umfang angemessen ist.
- **Abgestimmtheit:** Die Anforderung widerspricht direkt der Befürchtung der Studierendenvertretung, dass der Study Buddy zum Überwachungswerkzeug wird. Damit gefährdet sie die Akzeptanz des Systems.

**Strategie:** **RECONSIDER**

**Begründung:**
Die Anforderung darf in dieser Form nicht übernommen werden. Wir können sie aber auch nicht seriös „reparieren“, etwa indem wir „nur aggregierte, anonymisierte Daten“ einsetzen. Damit würden wir eine Entscheidung vorwegnehmen, die nur Datenschutz und Studiengangsleitung gemeinsam treffen können. Wir dokumentieren daher ausdrücklich: Ohne geklärten Zweck und ohne Prüfung durch Datenschutz ist keine Neuformulierung möglich.

**Offene Fragen:**
1. Welche Entscheidung oder Maßnahme will die Studiengangsleitung mit diesen Informationen treffen? → *Studiengangsleitung*
2. Reichen dafür aggregierte bzw. anonymisierte Daten, oder ist ein personenbezogener Zugriff nötig? → *Studiengangsleitung, Datenschutz*
3. Welche Rechtsgrundlage, welche Speicherdauer und welches Berechtigungskonzept gelten? → *Datenschutz & Informationssicherheit*
4. Wie werden Studierende darüber informiert, wer welche Daten sieht? → *Datenschutz, Studierendenvertretung*

**Ergebnis:**
Die Anforderung wird **vorerst nicht übernommen**. Wir legen sie Datenschutz und Studiengangsleitung zur gemeinsamen Klärung vor.

---

## REQ-011 – The New Login

**Original:**
> „Studierende müssen für den Study Buddy ein separates Benutzerkonto mit eigenem Passwort erstellen.“

**Qualitätsmangel:**
- **Konsistenz:** Die Anforderung widerspricht der verbindlichen technischen Rahmenbedingung aus dem **Plot Twist (Aufgabe 02b)**, laut der der Zugriff auf den Study Buddy über den bestehenden FernFH-Account erfolgt (siehe D2, Abschnitt 02b).
- **Lösungsvorgabe statt Anforderung:** Die Anforderung schreibt eine technische Lösung (eigenes Konto mit Passwort) vor, statt das Bedürfnis zu beschreiben (sichere Anmeldung).
- **Konsistenz mit REQ-010:** Ohne Verknüpfung mit der Hochschul-Identität lassen sich automatisch übernommene Daten den Studierenden nicht verlässlich zuordnen.

**Strategie:** **REWRITE**

**Begründung:**
Die nötige Information liegt vor: Die Rahmenbedingung aus Aufgabe 02b ist verbindlich. Die ursprüngliche Anforderung wird verworfen und durch eine konsistente Formulierung ersetzt.

**Überarbeitete Anforderung:**
> **REQ-011 (neu):** „Das System muss Studierenden die Möglichkeit bieten, sich mit ihrem bestehenden FernFH-Account am Study Buddy anzumelden.“
> **REQ-011b (neu):** „Das System darf von Studierenden keine Erstellung eines separaten Benutzerkontos verlangen.“

**Offene Fragen (für Details, nicht für die Anforderung selbst):**
1. Welches Authentifizierungssystem bzw. welcher Identity Provider wird verwendet? → *IT & Online-Campus-Team* (bereits in D2/02b als offene Frage notiert)
2. Gilt die Anmeldung auch für Lehrende und Studiengangsleitung, falls diese den Study Buddy nutzen? → *IT*

**Ergebnis:**
Die Anforderung ist widerspruchsfrei neu formuliert. Technische Details (Protokoll, Identity Provider) gehören nicht in die Anforderung, sondern werden mit der IT geklärt.

---

## REQ-013 – The Silent Change

**Original:**
> „Änderungen an Abgabeterminen müssen automatisch übernommen werden, ohne dass eine erneute Bestätigung erforderlich ist.“

**Qualitätsmangel:**
- **Eindeutigkeit:** Die Anforderung steht im Passiv. Es bleibt offen, *wer* was *woher* übernimmt und wer nicht bestätigen muss (Studierende? Lehrende?).
- **Vollständigkeit / Transparenz:** Eine stille Übernahme ohne Hinweis birgt das Risiko, dass Studierende geänderte Fristen übersehen.
- **Konsistenz:** Es gibt Abhängigkeiten zu REQ-010 (Datenquelle) und REQ-007/008 (ob über Änderungen benachrichtigt wird).

**Strategie:** **REWRITE** (Akteur und Sichtbarkeit präzisieren) + **INVESTIGATE** (Benachrichtigung und Quelle)

**Überarbeitete Anforderungen:**
- **REQ-013a:** „Das System muss geänderte Abgabetermine aus `[OFFEN: Quellsystem, siehe REQ-010]` übernehmen, ohne dass Studierende die Änderung bestätigen müssen.“
- **REQ-013b:** „Das System muss bei einem Abgabetermin, der sich geändert hat, den bisherigen und den neuen Termin anzeigen.“ (*Vorschlag – nicht validiert*)
- **REQ-013c:** „Das System muss Studierende über die Änderung eines Abgabetermins benachrichtigen.“ Kategorie gemäß REQ-007/008: `[OFFEN: optional oder verpflichtend]`.

**Offene Fragen:**
1. Aus welchem System kommen Abgabetermine, und wer ist dort für Änderungen verantwortlich? → *IT & Online-Campus-Team, Lehrendenvertretung*
2. Ist eine Fristverschiebung ein Ereignis, über das Studierende verpflichtend informiert werden müssen? → *Studienadministration, Studierendenvertretung*
3. Brauchen Studierende eine Änderungshistorie, oder genügt die Anzeige des alten und neuen Termins? → *Studierende / Studierendenvertretung*

**Ergebnis:**
Den Kern der Anforderung (automatische Übernahme ohne Bestätigung) haben wir beibehalten und den Akteur ergänzt. Die Transparenz-Anforderungen 013b und 013c sind unser Vorschlag zur Behebung des Mangels und müssen noch mit den Stakeholder*innen bestätigt werden.

---

## REQ-015 – The AI Knows Best

**Original:**
> „Ein KI-Modell muss anhand der Nutzungsdaten automatisch entscheiden, welche Studierenden zusätzliche Betreuung benötigen.“

**Qualitätsmangel:**
- **Zulässigkeit:** Eine vollautomatisierte Entscheidung über Personen ohne menschliche Kontrolle ist datenschutzrechtlich problematisch. Datenschutz fordert in D2, dass generative KI-Systeme vorab gesondert geprüft werden und Studierende nicht automatisch als gefährdet eingestuft werden.
- **Lösungsvorgabe:** „Ein KI-Modell“ legt die Technologie fest, bevor das Bedürfnis geklärt ist.
- **Eindeutigkeit:** „Nutzungsdaten“ und „zusätzliche Betreuung“ sind undefiniert.
- **Verantwortlichkeit:** Wer auf eine Entscheidung reagieren muss und wer haftet, ist offen. Die Lehrendenvertretung hat dazu in D2 Bedenken geäußert.
- **Konsistenz:** Die Anforderung überschneidet sich mit REQ-004, REQ-006 und REQ-003d.

**Strategie:** **RECONSIDER**

**Begründung:**
Die Anforderung verlagert eine pädagogisch und rechtlich sensible Entscheidung vollständig auf ein System. Wir könnten sie zu „Das System schlägt vor, eine Lehrperson entscheidet“ (Human-in-the-Loop) umformulieren. Damit würden wir aber eine Abstimmung mit Datenschutz, Lehrenden und Studiengangsleitung vorwegnehmen, die nicht stattgefunden hat. Diesen Lösungsansatz dokumentieren wir deshalb nur als **Option zur Klärung**, nicht als Anforderung.

**Option zur Klärung (*nicht validiert*):** Das System liefert Hinweise, und die Entscheidung über Betreuungsmaßnahmen trifft immer ein Mensch.

**Offene Fragen:**
1. Welches Betreuungsangebot gibt es, und wer entscheidet heute, wer es erhält? → *Studiengangsleitung, Lehrendenvertretung*
2. Ist eine automatisierte Auswertung von Nutzungsdaten zu diesem Zweck zulässig, und welche Anforderungen an Transparenz und menschliche Prüfung gelten? → *Datenschutz & Informationssicherheit*
3. Wer reagiert auf einen Hinweis des Systems, und wer trägt die Verantwortung? → *Lehrendenvertretung, Studiengangsleitung*
4. Wollen Studierende auf diesem Weg angesprochen werden? Braucht es ein Opt-in? → *Studierendenvertretung*

**Ergebnis:**
Die Anforderung wird **nicht übernommen**. Wir empfehlen, REQ-004, REQ-006, REQ-015 und REQ-003d gemeinsam in einem Klärungstermin mit Studiengangsleitung, Lehrendenvertretung, Studierendenvertretung und Datenschutz zu behandeln, weil alle vier dasselbe ungeklärte Ziel betreffen: Unterstützungsbedarf erkennen.
