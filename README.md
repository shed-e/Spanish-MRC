# PharmaCoNER using BERT in the Machine Reading Comprehension Framework

# Directory
```
Spanish-MRC
|
├─ dataset-cased
|   ├─ train.txt
|   ├─ dev.txt
|   ├─ test.txt
|   ├─ query_tarin.txt
|   ├─ query_dev.txt
|   └─ query_test.txt
|
├─ dataset-uncased
|   ├─ train.txt
|   ├─ dev.txt
|   ├─ test.txt
|   ├─ query_tarin.txt
|   ├─ query_dev.txt
|   └─ query_test.txt
| 
├─ Spanish-Query
|   ├─ Q1
|   ├─ Q2
|   └─ Q3
|  
├─ models
|   ├─ PubMedBERT-Base-uncased(abstracts + full text)
|   ├─ PubMedBERT-Base-uncased(abstracts only)
|   ├─ BlueBERT-Base-uncased(PubMed)
|   ├─ ClinicalBERT
|   ├─ PubMedBERT-Base-uncased(abstracts only)
|   └─ BioBERT-Base v1.2 (+ PubMed 1M)
| 
├─ processors
|   ├─ bert_ent.py
|   └─ utils_ner.py
| 
├─ metrics
|   └─ ner_metrics.py
| 
├─ output
| 
├─ run.ipynb
| 
└─ README.md
```
 * dataset-cased and datset-uncased: provide the processed upper and lower case PharmaCoNER dataset.
 * Spanish-Query: provide three kinds of Spanish queries.
 * models: provide the model required for the experiment.
 * processor: provides read and basic pre-processing procedures for data sets.
 * metrics: defined The evaluation function of the model.
 * outputs: used to store the output files.
 * run.ipynb: Modify the dataset and model paths and run to get the corresponding experimental results.
 
# Experimental Environment
* Ubuntu 18.04
* python 3.9.13
* transformers 4.25.1
* torch 1.13.0
* numpy 1.21.5
* pandas 1.4.4
* scipy 1.9.1
