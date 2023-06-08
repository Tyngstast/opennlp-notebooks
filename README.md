# OpenNLP Kotlin Notebooks

Kotlin notebooks for opennlp sentdetect training and testing with [Talbanken dataset](https://github.com/UniversalDependencies/UD_Swedish-Talbanken).

### Data formatting
[opennlp-format-data](notebooks/opennlp-format-data.ipynb) to format Talbanken to opennlp compatible training and test data.

### Train
[opennlp-train](notebooks/opennlp-train.ipynb) to train OpenNLP 2.2 sentence detector on latest talbanken data.

### Test
[opennlp-test](notebooks/opennlp-test.ipynb) to evaluate models. 
Comparing "old" swedish 1.5 model [from here](https://opennlp.sourceforge.net/models-1.5/) with new trained 2.2 version.

Slightly better results for new 2.2 trained model. Might simply be because of more extensive data in Talbanken repository since the 1.5 version was trained.

### Existing 1.5 results
```
Precision: 0.9293286219081273
Recall: 0.8630024610336341
F-Measure: 0.8949383241173968
```

### New 2.2 results
```
Precision: 0.9312169312169312
Recall: 0.8662838392124692
F-Measure: 0.8975775605609859
```
