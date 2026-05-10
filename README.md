# AI-Performance-Predictor (APP)
### Projekt im Kurs „KI entwickeln“ (Building AI)

## Summary / Zusammenfassung

Der AI-Performance-Predictor nutzt lineare Regression, um Callcenter-Daten aus PDFs zu analysieren. Das Tool berechnet nicht nur Vergangenheitswerte, sondern prognostiziert Trends für AHT und Anrufvolumina. Ziel ist eine proaktive Teamsteuerung und Anomalie-Erkennung zur Effizienzsteigerung.

## Hintergrund

In modernen Support-Teams fallen täglich riesige Mengen an Daten an. Mein Ziel ist der Übergang von einer reaktiven zu einer prädiktiven Analyse. Eine präzise Vorhersage der Bearbeitungszeit (AHT) hilft dabei, die Personalplanung zu optimieren und die Erreichbarkeit zu verbessern.

## Bereitgestellte Test-Dateien

In diesem Repository sind alle Komponenten enthalten, um das System direkt zu testen:

* **`index.html` (Das Dashboard):** Die interaktive Benutzeroberfläche. Sie kann direkt im Browser geöffnet werden und dient als Schnittstelle für den Daten-Upload und die KI-Visualisierung.
* **`Performance_Mitarbeiter_Detail.pdf` (Test-Daten):** Eine beispielhafte PDF-Datei mit realitätsnahen Performance-Werten, die im Dashboard hochgeladen werden kann, um die Analysefunktionen zu testen.

## Datenquelle und Verarbeitung

Das System ist darauf ausgelegt, unstrukturierte Daten aus operativen Berichten nutzbar zu machen:

1.  **Daten-Upload:** Über das HTML5-Dashboard können PDF-Berichte per Drag-and-Drop geladen werden.
2.  **Lokale Verarbeitung:** Die Extraktion der Kennzahlen (LE gesamt, AHT, ACT, Produktivität) erfolgt clientseitig (Privacy by Design).
3.  **KI-Analyse:** Die aufbereiteten Daten werden direkt an die integrierten Modelle übergeben.

## KI-Techniken

* **Lineare Regression:** Zur Berechnung der Performance-Kurve und Vorhersage künftiger AHT-Trends.
* **Anomalie-Erkennung:** Identifizierung von statistischen Ausreißern in den Leistungsdaten.
* **k-Nearest Neighbors (k-NN):** Vergleich von Profilen zur Identifikation von Best-Practice-Arbeitsweisen.

## Wie wird es eingesetzt?

Teamleiter laden PDF-Reports hoch und erhalten sofort visuelle Prognosen und Warnungen bei Anomalien. Dies ermöglicht eine vorausschauende Ressourcenplanung statt einer reinen Nachbetrachtung.

## Ausblick

Zukünftig soll das Modell um Natural Language Processing (NLP) erweitert werden, um zusätzlich die Stimmung (Sentiment) in Gesprächsnotizen aus den Reports zu analysieren.
