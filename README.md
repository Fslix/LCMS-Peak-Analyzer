# LCMS-Peak-Analyzer

Erste Ideen des LCMS-Peak-Analyzers (veröffentlichbarer Teil):
Zur Reduktion der Komplexität werden die Parameter bestimmter Verteilungen, welche einen Peak modellieren, genutzt:
Arbeitshypthosen waren unabhängige Achsen (nicht haltbar) und Gaußverteilung (nicht optimal)

Der finale Algorithmus
Der final einzusetzende Algorithmus ist sehr simpel gehalten:

1. Suche der nächsten Region of Interest
2. Daten in dieser Region in Form der Trainingsdaten beschreiben
3. Trainiertes Netzwerk anwenden (auf jede Achse einzeln)
4. Multivariate Verteilung als "Produkt" der Dichten berechnen
5. Von allen Daten die entsprechende Dichte abziehen
6. Gehe zurück zu 1.

Genutzt werden Alphatims und noch zu liefernde Datensets
