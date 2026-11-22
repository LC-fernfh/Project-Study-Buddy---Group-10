# Teil C – Zerlegen statt etikettieren

## „Das System sollte benutzerfreundlich sein.“
**1 · Was ist unklar?**  
1) Für wen soll das System benutzerfreundlich sein: Studierende, Lehrende oder Studienadministration?
2) Welche Aufgaben müssen besonders leicht gehen (z. B. nächste Abgabefrist finden, Benachrichtigungen einstellen, Lernfortschritt ansehen)?
3) Woran würden Sie erkennen, dass das System benutzerfreundlich ist: Welche Prüfmethode und welches Erfolgskriterium akzeptieren Sie bei der Abnahme?

**2 · Funktion**  
Die Aussage enthält keine eigene Funktion. Sie beschreibt, wie gut Funktionen nutzbar sein sollen. Dahinter stehen Kernaufgaben, z. B.: „Das System muss Studierenden auf der Startseite die als Nächstes fälligen Abgaben ihrer belegten Lehrveranstaltungen anzeigen.“ (Katalog S-01)

**3 · Qualität**  
Messgröße: Erfolgsquote und Zeit bei einer Kernaufgabe. Zielwert: Mindestens 90 % der Testpersonen finden ihre nächste Abgabefrist ohne Hilfe innerhalb von 60 Sekunden. Bedingung: moderierter Usability-Test mit mindestens 8 berufsbegleitend Studierenden, erster Kontakt ohne Schulung. (Katalog S-12; Zielwert ist unser Vorschlag und mit der Studiengangsleitung abzustimmen.)

**4 · Randbedingung**  
Ja: Barrierefreiheit nach WCAG 2.1 Stufe AA. Quelle: Web-Zugänglichkeits-Gesetz (WZG) bzw. EU-Richtlinie 2016/2102, Geltung für die FernFH ist mit Studiengangsleitung / Qualitätsmanagement zu klären. Außerdem mögliche Gestaltungsvorgaben des Online Campus, Quelle: IT & Online-Campus-Team.

**5 · Ebene**  
System

## „Die App sollte schnell antworten.“

**1 · Was ist unklar?**  
1) Welche Aktionen müssen schnell sein: Aufruf der Übersicht, Laden der Fristen, Antwort auf eine Frage, Zustellung einer Benachrichtigung?
2) Wie schnell ist „schnell“, und wo wird gemessen (Server, Endgerät, mobiles Netz)?
3) Unter welcher Last muss das gelten, z. B. am Semesterstart oder kurz vor großen Abgabeterminen, mit wie vielen gleichzeitigen Nutzenden?

**2 · Funktion**  
Keine neue Funktion. Die Aussage bezieht sich auf bestehende Funktionen, vor allem: „Das System muss Studierenden eine Übersicht mit Abgabeterminen und Lernfortschritt anzeigen.“ (Katalog S-01 und S-08)

**3 · Qualität**  
Messgröße: Ladezeit der Übersichtsseite bis zur vollständigen Anzeige. Zielwert: bei 95 % der Aufrufe höchstens 2 Sekunden. Bedingung: gemessen am Endgerät bei bis zu 500 gleichzeitig angemeldeten Nutzenden. (Katalog S-11; Zielwert ist unser Vorschlag und mit der IT auf Machbarkeit zu prüfen.)

**4 · Randbedingung**  
Ja: Die Daten (Fristen, Kurse) kommen über die Schnittstellen des bestehenden Online Campus. Die erreichbare Antwortzeit hängt davon ab. Quelle: IT & Online-Campus-Team. Seit dem Plot Twist muss das zusätzlich auch in der Web-App gelten (Quelle: IT).

**5 · Ebene**  
System


# Teil Plot-Twist

## Randbedingung

## Begründung: 
Die Vorgabe kommt von außen, von der IT, und nicht aus einem Bedarf der Nutzenden. Sie beschreibt keine Funktion („was“) und keine messbare Güte („wie gut“), sondern legt die Plattform fest, auf der das System laufen muss. Sie ist verbindlich und schränkt den Lösungsraum ein. Wir tragen sie als Randbedingung auf Systemebene mit Quelle „IT & Online-Campus-Team“ ein (Katalog S-22). Folgen: Bestehende Anforderungen müssen für Browser neu geprüft werden, vor allem Anmeldung über den FernFH-Account, Benachrichtigungen (Push im Browser), Antwortzeiten und Barrierefreiheit. Unklar ist auch, was „ab sofort“ für Zeitplan und Budget bedeutet.

## Rückfrage 1
Bleibt die native App bestehen, und muss die Web-App denselben Funktionsumfang bieten (inklusive Benachrichtigungen), oder reicht ein Teil der Funktionen?
## Rückfrage 2
Welche Browser und Versionen müssen unterstützt werden, und gelten in der Web-App dieselben Vorgaben für Anmeldung über den FernFH-Account und Barrierefreiheit?
