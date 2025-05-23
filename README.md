# Code für Data Mining-Algorithmen und Feature Engineering zur Vorhersage von Retouren im  Onlinehandel – Khaled El-Dakhakhny

Dies ist der Quellcode. Der Code darf genutzt und angepasst werden, 
sofern die Nutzung **nicht kommerziell** ist und mein Name(Khaled El-Dakhakhny) als Urheber genannt wird.

## Lizenz

Dieser Code steht unter der **Creative Commons BY-NC 4.0 Lizenz**.  
Mehr Informationen: [https://creativecommons.org/licenses/by-nc/4.0/](https://creativecommons.org/licenses/by-nc/4.0/)


## Notebook

Das Colab-Notebook befindet sich hier:  
https://colab.research.google.com/drive/1e-3MJ4v09tG_aLd7T0dPnTTeR6TCAmAc

## Modelle

Die folgenden trainierten Modelle liegen im Repository:

- `dt_model.pkl`: Trainiertes Decision Tree Modell (68,69 %)
- `xgb_model.pkl`: Trainiertes XGBoost Modell (69,36 % )

## Datensatzbeschreibung

### 1. `df13_all_dataset_new_feature_engineering.parquet`
- Vollständiger Datensatz mit allen Originalzeilen (inkl. 39.419 Zeilen mit fehlendem `deliveryDate`)
- Diese fehlenden Werte wurden **behandelt** 
- Alle neuen Features sind enthalten

### 2. `df_without_missing_deliverydate_with_all_features.parquet`
- Variante des Datensatzes, bei dem alle **39.419 Zeilen mit fehlendem `deliveryDate` entfernt** wurden
- Enthält alle neuen Features


### 3. `orders_class2_with_all_feature.parquet`
- Der **Test-/Klassifizierungsdatensatz** mit denselben Features wie im Training
- Wird verwendet zur Vorhersage und externen Modellbewertung

## Präsentation

Im Repository ist außerdem die Abschlusspräsentation hinterlegt:  
- `Präsentation.pptx`
