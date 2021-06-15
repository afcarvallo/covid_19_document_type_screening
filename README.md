# COVID-19 document type screening with neural language models for evidence-based healthcare

This repository contains the code used for experiments in the paper: "COVID-19 document type screening with neural language models for evidence-based healthcare"

In this paper we use an XLNET model finetuned on Epistemonikos dataset consisting on non-covid evidence labeled as systematic-review, primary study non randomized controlled trial, primary study randomized controlled trial, broad synthesis and excluded. 

Once the model was trained we evaluate their generalization capability on CORD-19 dataset adapted to the evidence-based medicine domain. 

CORD-19 dataset used for evaluation and XLNET pre-trained model with epistemonikos dataset can be found in the following link: 
**LINK**

The jupyter notebook code to run the experiments are included in this github repository in the scripts folder.

We obtained the following results: 

