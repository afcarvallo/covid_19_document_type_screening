# COVID-19 document type screening with neural language models for evidence-based healthcare

This repository contains the code used for experiments for COVID-19 document type screening.

We use an XLNET model finetuned on Epistemonikos dataset consisting on non-covid evidence labeled as systematic-review, primary study non randomized controlled trial, primary study randomized controlled trial, broad synthesis and excluded. And compare to baselines BioBERT and Random Forest.

Once the model was trained we evaluate their generalization capability on CORD-19 dataset adapted to the evidence-based medicine domain. 

CORD-19 dataset used for evaluation and XLNET pre-trained model with epistemonikos dataset can be found in the following link:
https://zenodo.org/record/4968811

The jupyter notebook code to run models predictions are included in the following links:

-  [XLNET](https://github.com/afcarvallo/covid_19_document_type_screening/blob/main/scripts/XLNet_CORD19_predictions.ipynb).
-  [BioBERT](https://github.com/afcarvallo/covid_19_document_type_screening/blob/main/scripts/BioBERT_CORD19_predictor.ipynb).
-  [Random Forest](https://github.com/afcarvallo/covid_19_document_type_screening/blob/main/scripts/RandomForest_CORD19_predictor.ipynb).

Results are shown in f1-score: 

|  type of article  | Random Forest | XLNET | BioBERT |
|:-----------------:|:-------------:|:-----:|:-------:|
|  Broad Synthesis  |      .45      |  **.81**  |   .62   |
|      Excluded     |      .34      |  **.97**  |   .73   |
|    Primary RCT    |      .56      |  **.86**  |   .71   |
|  Primary-non-RCT  |      .06      |  **.99**  |   .88   |
| Systematic Review |      .85      |  **.96**  |   .93   |
|  **Weighted Average** |  .54      |  **.97**  |   .84   |





