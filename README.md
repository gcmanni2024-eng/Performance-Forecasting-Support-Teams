# AI-Performance-Predictor (APP)
### Projekt im Kurs „KI entwickeln“ (Building AI)

## Zusammenfassung

Der AI-Performance-Predictor nutzt lineare Regression, um Callcenter-Daten aus PDFs zu analysieren. Das Tool berechnet nicht nur Vergangenheitswerte, sondern prognostiziert Trends für AHT und Anrufvolumina. Ziel ist eine proaktive Teamsteuerung und Anomalie-Erkennung zur Effizienzsteigerung. (Projekt im Kurs „KI entwickeln“)

## Hintergrund

In modernen Support-Teams fallen täglich riesige Mengen an Daten an, die oft nur im Nachhinein betrachtet werden. Mein Ziel ist es, den Übergang von einer reaktiven zu einer prädiktiven Analyse zu schaffen. Eine präzise Vorhersage der Bearbeitungszeit (AHT) hilft dabei, die Personalplanung zu optimieren und die Kundenzufriedenheit durch bessere Erreichbarkeit zu steigern.

## Daten und KI-Techniken

Das Projekt stützt sich auf strukturierte Performance-Daten, die automatisiert aus PDF-Berichten extrahiert werden. Eine entsprechende Beispieldatei (Performance_Mitarbeiter_Detail.pdf) befindet sich in diesem Repository. 

Die technische Basis bildet ein HTML5/JavaScript-Dashboard (siehe index.html), welches die PDF-Daten clientseitig ausliest und für die KI-Modelle aufbereitet. Zu den Kernvariablen gehören:

* LE gesamt: Anzahl der bearbeiteten Anrufe.
* AHT (Average Handling Time): Die durchschnittliche Bearbeitungszeit pro Fall (Ist vs. Soll).
* ACT & ACW: Reine Gesprächszeit und Nachbearbeitungszeit.
* Produktivität: Der prozentuale Anteil der aktiven Arbeitszeit.

Techniken:
1. Lineare Regression: Zur Berechnung der Steigung der Performance-Kurve und für Trend-Vorhersagen.
2. Anomalie-Erkennung: Identifizierung von statistischen Ausreißern (z. B. extrem niedrige Produktivität).
3. k-Nearest Neighbors (k-NN): Vergleich von Mitarbeiter-Profilen zur Identifikation von Best-Practice-Arbeitsweisen.

## Wie wird es eingesetzt?

Die Lösung wird als Web-Dashboard für Teamleiter eingesetzt. Diese laden PDF-Reports per Drag-and-Drop hoch und erhalten sofort visuelle Prognosen und Warnungen bei Anomalien. Dies entlastet die Planung und sorgt für eine faire Arbeitsverteilung.

## Herausforderungen

Die KI kann keine unvorhersehbaren externen Ereignisse einplanen. Zudem muss der Datenschutz bei der Verarbeitung personenbezogener Leistungsdaten höchste Priorität haben.

## Wie geht es weiter?

Zukünftig soll das Modell um Natural Language Processing (NLP) erweitert werden, um zusätzlich die Stimmung (Sentiment) in Gesprächsnotizen zu analysieren.
