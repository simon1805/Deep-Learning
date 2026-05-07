# Prüfungsaufgabe 1: Deep-Learning
## Starten der Umgebung
Das Notebook kann per mybinder (https://mybinder.org/) geöffnet werden.
Folgende Daten müssen in die Felder eingetragen werden:
- Github Repo: https://github.com/simon1805/Deep-Learning.git
- Git ref: main
- File to open: index.ipynb
## Dokumentation
- Ziel ist es, Banknoten anhand von Wellenlet-transformierten Bildmerkmalen als authentisch oder gefälscht zu klassifizieren.
- Der Datensatz beinhaltet vier kontinuierliche Feature (Varianz, Skewness, Kurtosis, Entropie) und ein binäres Klassenlabel.
- Zuerst wird eine explorative Datenanalyse (EDA) durchgeführt, um die Verteilung und Beziehungen der Features zu visualisieren.
- Die Daten werden mit StandardScaler standardisiert und in Trainings- und Testsets aufgeteilt (70/30).
- Anschließend wird ein Deep Neural Network (DNN) mit versteckten Schichten [10, 20, 10] trainiert.
- Zum Vergleich wird zusätzlich ein Random Forest Classifier mit 200 Estimatoren trainiert.
## Erwartetes Ergebnis
- Die EDA zeigt ein Countplot der Klassenverteilung und ein Pairplot mit Hue nach Klasse, das die Trennbarkeit der Features verdeutlicht.
- Die standardisierten Features liegen im Bereich von ungefähr -3 bis +3 und sind optimiert für neuronale Netze.
- Das DNN-Modell erreicht sehr hohe Genauigkeit (>99%) auf dem Testset, mit ausgezeichneten Precision-, Recall- und F1-Scores.
- Der Random Forest Classifier zeigt ebenfalls gute Ergebnisse, schneidet aber etwas schlechter ab als das DNN.
- Ausgaben umfassen Confusion Matrices und Classification Reports für beide Modelle.
- Die Ergebnisse demonstrieren die Leistungsfähigkeit von Deep Neural Networks bei strukturierten tabellarischen Daten.