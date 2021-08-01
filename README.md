# w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer

This repository contains Jupyter Notebooks for the paper: [Medical Relationship Extraction with Bio-Clinical BERT and Longformer](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/W266%20-%20Medical%20Relationship%20Extraction%20with%20Bio-Clinical%20BERT%20and%20Longformer.pdf).

## Dataset
The 2012 i2b2 temporal relation dataset can be found here: https://portal.dbmi.hms.harvard.edu/projects/n2c2-nlp/ and requires registaration.

## Notebooks
A total of six notesbooks were used in this project. 

* [data_parse.ipynb](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/data_parse.ipynb)                   - for parsing the XML files from the 2021 i2b2 temporal relation dataset and includes the addition of entity tokens
* [data_prep_eda.ipynb](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/data_prep_eda.ipynb)               - exploratory analysis of the dataset and producing a subset dataset
* [train_baseline.ipynb](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/train_baseline.ipynb)               - model training of baseline 
* [train_bioclinicalbert_cls.ipynb](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/train_bioclinicalbert_cls.ipynb)   - model training of Bio-Clinical BERT with [CLS] + entity mask
* [train_longformer_cls.ipynb](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/train_longformer_cls.ipynb)         - model training of Longformer with [CLS] + entity mask, and handcrafted example prediction
* [result_analysis.ipynb](https://github.com/sli0111/w266-2021-Medical-Relationship-Extraction-with-Bio-Clinical-BERT-and-Longformer/blob/main/result_anlaysis.ipynb)             - interpretation of model predictions, includes classification report, confusion matrix, and studying examples


## Environment and Requirements
The notebooks were run on Amazon EC2 instance using Deep Learning AMI (Ubuntu 18.04) Version 47.0 (ami-069137bd6aaaa65ab).  The p3.2x large GPU was used for training.

Both Bio-Clinical BERT and Longformer were loaded from transformer library from HuggingFace.  Model architecture was built and trained using Keras from Tensorflow 2.5.







