# AI-Performance-Predictor (APP)
### Projekt im Kurs „KI entwickeln“ (Building AI)

## Zusammenfassung
Der AI-Performance-Predictor nutzt lineare Regression, um Callcenter-Daten aus PDFs zu analysieren. Das Tool berechnet nicht nur Vergangenheitswerte, sondern prognostiziert Trends für AHT und Anrufvolumina. Ziel ist eine proaktive Teamsteuerung und Anomalie-Erkennung zur Effizienzsteigerung. (Projekt im Kurs „KI entwickeln“)

## Hintergrund
In modernen Support-Teams fallen täglich riesige Mengen an Daten an, die oft nur im Nachhinein betrachtet werden. Mein Ziel ist es, den Übergang von einer reaktiven zu einer prädiktiven Analyse zu schaffen. Eine präzise Vorhersage der Bearbeitungszeit (AHT) hilft dabei, die Personalplanung zu optimieren und die Kundenzufriedenheit durch bessere Erreichbarkeit zu steigern.

## Daten und KI-Techniken
Datenquellen & Verarbeitung
Das Projekt stützt sich auf strukturierte Performance-Daten, die automatisiert aus PDF-Berichten extrahiert werden. Eine entsprechende Beispieldatei (Performance_Mitarbeiter_Detail.pdf) befindet sich in diesem Repository.

Die technische Basis bildet ein HTML5/JavaScript-Dashboard (siehe index.html), welches die PDF-Daten clientseitig ausliest und für die KI-Modelle aufbereitet. Zu den Kernvariablen gehören:


LE gesamt: Anzahl der bearbeiteten Anrufe.   


AHT (Average Handling Time): Die durchschnittliche Bearbeitungszeit pro Fall (Ist vs. Soll).   


ACT & ACW: Reine Gesprächszeit und Nachbearbeitungszeit.   


Produktivität: Der prozentuale Anteil der aktiven Arbeitszeit (netto/brutto).   

KI-Techniken
Um aus diesen Rohdaten echte Erkenntnisse zu gewinnen, kommen folgende Techniken zum Einsatz:

Lineare Regression (Trend-Analyse): Das Dashboard nutzt die extrahierten Zeitreihen, um mittels linearer Regression die Steigung der Performance-Kurve zu berechnen. Dies ermöglicht eine "Trend-Morgen"-Vorhersage für AHT und Anrufvolumina.

Anomalie-Erkennung: Durch statistische Analyse erkennt die KI Ausreißer. Im vorliegenden Datensatz (siehe PDF) würde das System beispielsweise automatisch Alarm schlagen, wenn die Produktivität massiv sinkt (z. B. auf 4,5%) oder die Nachbearbeitungszeit (ACW) ungewöhnlich hoch ist.   

Klassifizierung (k-Nearest Neighbors):
Die KI vergleicht Mitarbeiter-Profile anhand der IDs (z. B. (67993)), um Ähnlichkeiten in der Arbeitsweise zu finden und gezieltes Coaching anzubieten.

## Wie wird es eingesetzt?
Die Lösung wird als Web-Dashboard für Teamleiter eingesetzt. Diese laden PDF-Reports per Drag-and-Drop hoch und erhalten sofort visuelle Prognosen und Warnungen bei Anomalien. Dies entlastet die Planung und sorgt für eine faire Arbeitsverteilung.

## Herausforderungen
Die KI kann keine unvorhersehbaren externen Ereignisse (z. B. technische Totalausfälle) einplanen. Zudem muss der Datenschutz bei der Verarbeitung personenbezogener Leistungsdaten höchste Priorität haben.

## Wie geht es weiter?
Zukünftig soll das Modell um Natural Language Processing (NLP) erweitert werden, um zusätzlich die Stimmung (Sentiment) in Gesprächsnotizen zu analysieren.

## Danksagung
Dieses Projekt entstand im Rahmen des Kurses "Elements of AI / Building AI".
