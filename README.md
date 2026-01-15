# Olist-E-Commerce-Analytics-Projekt : Microsoft Fabric End‑to‑End Projekt

Dieses Projekt zeigt eine vollständige End‑to‑End‑Analytics‑Lösung in Microsoft Fabric auf Basis des realen Olist E‑Commerce Datasets (Kaggle).
Es bildet einen modernen Data‑Engineering‑Workflow ab – von der Rohdatenaufnahme bis zum fertigen Power‑BI‑Dashboard.
Das Projekt zeigt, wie ich komplexe Datenstrukturen analysiere, transformiere, modelliere und in geschäftsrelevante Insights überführe.

## Projekt Ziel 

Ziel ist der Aufbau einer skalierbaren Analytics‑Plattform, die zentrale Geschäftsfragen beantwortet:
  - Wie entwickeln sich Umsatz und Bestellvolumen
  - Welche Produktkategorien und Verkäufer performen am besten
  - Wie zuverlässig sind die Lieferprozesse
  - Wie hängen Lieferzeiten mit Kundenzufriedenheit zusammen

Der Fokus liegt auf Datenqualität, Modellierung, Automatisierung und Visualisierung.

## Business‑Fragen 
Damit dein Projekt nicht nur technisch, sondern auch “business‑relevant” wirkt, definieren wir 4–6 klare Fragen:

  ### Verkauf & Umsatz
    - Wie entwickeln sich Umsatz und Bestellvolumen über die Zeit?
    - Welche Produktkategorien und Verkäufer performen am besten?
  
  ### Logistik & Lieferung
    - Wie lange dauert die Lieferung im Durchschnitt?
    - Wie hoch ist der Anteil verspäteter Lieferungen (gegenüber dem geschätzten Lieferdatum)?
    - Gibt es regionale Unterschiede in der Lieferperformance?
  
  ### Kundenzufriedenheit
  
    - Wie verteilen sich die Review‑Scores?
    - Wie stark hängen Lieferverzögerungen mit schlechten Bewertungen zusammen?
  
## Architektur (Microsoft Fabric)
Das Projekt nutzt folgende Fabric‑Komponenten:

  - Lakehouse – Speicherung von Roh‑ und Transformationsdaten
  - Notebooks – Datenexploration, Bereinigung, Transformation
  - Data Pipelines – Orchestrierung der Datenprozesse
  - Semantic Model – Modellierung im Sternschema
  - Power BI – Visualisierung der Analyseergebnisse

 ##   Projektstruktur
 
fabric-olist-project/
│
├── 01_raw/                 # Rohdaten (CSV aus Kaggle)
├── 02_transformed/         # Bereinigte & transformierte Delta-Tabellen
├── 03_semantic_model/      # Fakten- und Dimensionstabellen
├── 04_powerbi/             # Power BI Dateien & Screenshots
│
├── notebooks/              # Fabric Notebooks (Exploration, Transformation)
├── docs/                   # Architekturdiagramme, Screenshots, Notizen
│
└── README.md               # Projektbeschreibung

## Verwendete Datensätze (Kaggle)
Das Olist‑Dataset enthält u. a.:
Bestellungen,Bestellpositionen,Kunden,Produkte,Verkäufer,Zahlungen,Lieferdaten,Reviews,Geodaten

## Datenmodell (Sternschema)
  ### Faktentabellen
  - FactOrders
  - FactOrderItems
  - FactPayments
  - FactReviews
  
  ### Dimensionstabellen
  - DimCustomer
  - DimProduct
  - DimSeller
  - DimDate
  - DimGeolocation

Das Modell ist optimiert für Power BI und schnelle analytische Abfragen.

## Ergebnisse & Insights
Das Power‑BI‑Dashboard liefert u. a.:

  - Umsatztrends und saisonale Muster
  - Top‑Produkte und Top‑Verkäufer
  - Analyse der Lieferperformance (inkl. Verspätungen)
  - Zusammenhang zwischen Lieferzeit und Review‑Score
  - Regionale Unterschiede im Kauf‑ und Lieferverhalten

Diese Insights zeigen, wie Daten zur Optimierung von Logistik, Sortiment und Kundenzufriedenheit genutzt werden können.

## Machine Learning
Ein zusätzliches Notebook zeigt:

  - Vorhersage von Lieferverzögerungen
  - Feature‑Analyse (z. B. Distanz, Produktkategorie, Gewicht)

Dieses Projekt zeigt die Fähigkeiten in:

  - Datenmodellierung & Data Engineering
  - Fabric‑Architektur & Cloud‑Analytics
  - Automatisierung & Pipelines
  - Business‑orientierter Analyse
  - Power BI Reporting
  - Kommunikation komplexer Daten in verständlicher Form


