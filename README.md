# Struktur

Dieses Repository enthält alle Dokumente unseres Statistik-Projekts, inklusive aller Analysen, Fallnotizen sowie einer Table of Contribution und Table of Prompts.

```bash
├── Health_Analyse_1/_2/_3.ipynb      # Alle Analysen unseres ersten, leider ungeeigneten Datensatzes über Global Health, welchen wir danach ersetzt haben.
├── Analyse_1-6.ipynb                 # Analysen sowie Interpretationen des Fraud-Datensatz zu Themen der Vorlesungen 1 bis 6.
├── Analyse_7und8.ipynb               # Hypothesentests sowie damit verbundene Thematiken, behandelt in den Vorlesungen 7 und 8.
├── Analyse_8.ipynb                   # Gruppenvergleiche, inkl. Post-hoc Tests und Fehlerkorrekturen, im Einklang mit VL9.
├── Analyse_10/_11.ipynb              # Regressions-Analysen sowie -Modelle, gemäss Vorlesungsinhalten der Woche 10 und 11.
├── Analyse_12.ipynb                  # Analyse der Einwohnerzahlen sowie Transaktionsbeiträge anhand des Benfordschen Gesetz.
├── Fallnotiz.ipynb                   # Alle Fallnotizen des Projekts, enthält (teilweise wiederholend) alle Interpretationen und Begründungen.
├── Add-ons.ipynb                     # Code für zusätzliche Grafiken , die wir in unserer Zwischen-/Abschlusspräsentation verwendet haben. Zusätzlich enthält es unser logistisches Regressionmodell, welches wir für die Zwischenpräsentation entworfen haben.
└── README.md                         # Alle Informationen über das Repository sowie den Table of Contributions & Table of Prompts.
```

# Team
* Thierry Suhner
* Karla Ruggaber
* Phil Solenthaler


# Vorgehen
Grundsätzlich ist zu unserer Zusammenarbeit zu sagen, dass wir die Aufteilung sowie Tasks und interne sowie externe Deadlines immer kollektiv besprochen und miteinander abgestimmt haben, ebenso haben wir uns regelmässig in Person getroffen um uns Gedanken über das weitere Vorgehen, wichtige Entscheidungen oder vertiefte Analysen zu machen. Von der Timeline her haben wir uns meistens alle zwei Wochen besprochen, wie wir die neu eingeführten Inhalte aus der Vorlesung auf unseren Datensatz anwenden wollen, und dann entweder direkt gemeinsam daran gearbeitet (Vorlesung 1-6) oder die jeweiligen Themenfelder aufgeteilt und klar definiert, was wir uns für welches Thema bis wann als Outcome vorstellen. Dadurch konnten wir unserer Meinung nach das Ziel des Projekts – die Konzepte aus der Vorlesung wirklich praktisch anzuwenden – perfekt erfüllen und enorm davon profitieren, auch den Code und die praktischen Implikationen von gelernten Konzepten zu verstehen. Wir haben uns deswegen auch dazu entschieden, von Beginn weg mit einem Notebook pro Vorlesungswoche zu arbeiten, um das Projekt bzw. die Analysen sauber thematisch zu trennen. Einzige Ausnahme stellen hier die Vorlesungswochen 7 und 8 dar, welche wir aufgrund der Zusammengehörigkeit der Themen in einem  gemeinsamen Notebook behandelt haben.


# Table of Contributions
Im Anschluss findet sich eine Tabelle welche aufzeigt, wer primär an was gearbeitet hat. Grundsätzlich ist zu erwähnen, dass unser Teamwork sehr gut funktioniert hat und der insgesamte Beitrag aller Gruppenmitglieder sich auf einem ähnlichen Niveau befindet.

| Datei | Contributions |
|---------------|---------------|
| Analyse_1.ipynb - Analyse_7.ipynb      |  Gemeinsame Erarbeitung der Analysen im Einklang mit den Vorlesungsinhalten. |
| Analyse_7und8.ipynb      | Hypothesentests, durchgeführt von Phil. |
| Analyse_9.ipynb      | Gruppenvergleiche, durchgeführt von Karla. |
| Analyse_10.ipynb + Analyse_11.ipynb        | Regression (einfache, multiple sowie Panel-Ansätze), durchgeführt von Thierry. |
| Analyse_12.ipynb | Benfordsches Gesetz, angewendet von Thierry. |
| README.md | Informationen über das Projekt, erstellt von Thierry. |
| Fallnotiz.ipynb + Table of Prompts (in README.md) | Gemeinsam erstellt und jeweils befüllt während der Analysen, über den gesamten Verlauf des Projekts. |


# Table of Prompts
| Modell | Prompt |
|---------------|---------------|
| ChatGPT 5.0   | Bitte hilf mir beim Berechnen des Variance Inflation Factors in Python, wie geht das am einfachsten? |
| ChatGPT 5.0   | Welche der folgenden Panel-Ansätze macht bei meinem Datensatz am meisten Sinn in einem Modell umzuseten? Demeaning, First Differences, Two-Way Fixed Effects, Random Effects. Ich möchte mit dem Modell gerne klassifizieren, ob eine Transaktion Fraud ist oder nicht |
| ChatGPT 5.0 | Welche Möglichkeiten gibt es, in Python die Class Imbalance zu korrigieren? Mein Datensatz enthält nur sehr wenige Fraud-Fälle, ich würde aber mein Modell zur Klassifizierung von Transaktionen nach Fraud/Nicht-Fraud gerne robuster trainieren durch eine ausgeglichene Anzahl an Fraud- und Nicht-Fraud-Fällen im Training Set. |
| ChatGPT 5.0 | GIbt es in python einen plot, der wie ein bar chart ist, jedoch angeordnet wie eine Uhr, bei der aus der Mitte der Bar-Chart an den Rand des Kreises wächst, je nachdem wie viele Frauds in dieser Stunde passiert sind?|
| ChatGPT 5.0 | Welche plots würden die Performance meines logistic regression Modell für eine Präsentation am besten darstellen? Ich habe bereits eine Confustion Matrix sowie eine ROC-Curve. |
| ChatGPT 5.0 | Ich würde gerne die Anzahl Beobachtungen pro Staat in einer Karte darstellen. Kannst du mir den python code geben, mit der ich eine US-Karte mit den einzelnen Bundesstaaten erstellen kann? |
| ChatGPT 5.0 | Ich habe sehr viele paarweise Tests (Dunn) und korrigiere p-Werte mit Benjamini–Hochberg (FDR). Auch habe ich ein Plot, der sortierte p-Werte gegen die BH-Schwelle zeigt: was sieht man im Plot, wie liest man die Grenze "signifikant/nicht signifikant" warum ist FDR hier sinnvoll |
| ChatGPT 5.0 | Ich habe eine symmetrische p-Wert-Matrix (DataFrame) aus paarweisen Tests. Schreibe Code, der: p-Werte nur aus dem oberen Dreieck extrahiert, BH/FDR darauf anwendet, die korrigierten Werte wieder zurück in eine Matrix schreibt (symmetrisch, Diagonale=1) |
| ChatGPT 5.0 | Ich habe eine Spalte dob (Geburtsdatum) in meinem DataFrame ds. Schreibe Code, der dob robust in datetime konvertiert (errors='coerce') und daraus das Alter in Jahren relativ zu 2019-01-01 berechnet und als ds['age'] speichert.|
| ChatGPT 5.0 | Ich analysiere den Betrag amt über mehrere kategoriale Gruppen. Schreibe Code, der die Verteilung je Gruppe untersucht (z. B. Schiefe) und begründet, warum ein nichtparametrischer Test angebracht ist. Nutze pandas und scipy.|
| ChatGPT 5.0 | Ich möchte prüfen, wie sich eine log-Transformation auf die Verteilung von amt auswirkt. Schreibe Code, der: Histogramme von amt und log(amt) nebeneinander darstellt, Median und Mittelwert einzeichnet, kurze Kommentare im Code ergänzt.|
| ChatGPT 5.0 | Ich habe eine kontinuierliche Variable age. Schreibe Python-Code, der: age in sinnvolle Altersgruppen (Bins) einteilt die Gruppen sprechend benennt (z. B. '18–25', '26–35'), das Ergebnis als neue Spalte age_group speichert.|
