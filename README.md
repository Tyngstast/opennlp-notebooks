# OpenNLP Kotlin Notebooks

Kotlin notebooks for opennlp sentdetect training and testing with [Talbanken](https://github.com/UniversalDependencies/UD_Swedish-Talbanken) 
and [Sprakbanken (SUC)](https://github.com/kb-labb/sucx3_ner) datasets.

## Data formatting
[opennlp-format-data](notebooks/opennlp-format-data.ipynb) to format data sets to opennlp compatible training and test data.

## Train
[opennlp-train](notebooks/opennlp-train.ipynb) to train OpenNLP 2.2 sentence detector on latest data.

## Test
[opennlp-test](notebooks/opennlp-test.ipynb) to evaluate models. 
Comparing "old" swedish 1.5 model [from here](https://opennlp.sourceforge.net/models-1.5/) with new trained 2.2 models.

### Existing 1.5, Trained on Talbanken, tested on Talbanken
```
Precision: 0.9293286219081273
Recall: 0.8630024610336341
F-Measure: 0.8949383241173968
```

### New 2.2. Trained on Talbanken, tested on Talbanken
```
Precision: 0.9312169312169312
Recall: 0.8662838392124692
F-Measure: 0.8975775605609859
```

### New 2.2 Trained on Talbanken + Sprakbanken, tested on Talbanken + Sprakbanken
```
Precision: 0.9312169312169312
Recall: 0.8662838392124692
F-Measure: 0.8975775605609859
```

### Existing 1.5, Trained on Talbanken, tested on Talbanken + Sprakbanken
```
Precision: 0.8998357963875205
Recall: 0.842968850147417
F-Measure: 0.8704745515917663
```

### New 2.2 Trained on Talbanken + Sprakbanken, tested on Talbanken
```
Precision: 0.9322183098591549
Recall: 0.8687448728465955
F-Measure: 0.8993630573248407
```

### Result
We can see that the new model outperforms when trained and tested on the same dataset, and even more so when trained on 
a much larger dataset and evaluated on Talbanken.
