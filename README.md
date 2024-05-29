# Exploring-Foundation-Models-for-Cell-Type-Annotation-in-COVID-19

Transformer-based foundation models have the potential to significantly advance single-cell RNA sequencing (scRNA-seq) analysis, contributing to our understanding of viral pandemics such as COVID-19. In this study, we explore a very specific application of foundation models for scRNA-seq analysis, with a particular focus on blood cell types in the context of COVID-19. Concretely, we investigate the efficiency and generalization performance of the scGPT foundational model on cell-type annotation using techniques such as linear probing and similarity search prototype embedding (SSPL) on two blood datasets. Our analysis reveals two key findings: 1) similarity search on data points within the embedding space not only outperforms linear probing in performance but also exhibits greater efficiency and 2) zero-shot scGPT embeddings used for SSPL continue to perform well even in the small data regime and also demonstrate transferability to COVID-19 patients, even when their samples are not represented in the training data. We hope this study could benefit future research by adapting foundation models for efficient, robust, and generalizable analysis of scRNA-seq in infectious disease outbreaks and pandemics.

## foundation model: scGPT

https://github.com/bowang-lab/scGPT

## Data:
Dataset 1: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE155673 

Dataset 2: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE166992

Datasets were downloaded from sCOVID atlas: http://bio-computing.hrbmu.edu.cn/scovid/#/home

## scripts
Script folder contains three file:

scgpt_SSPL.ipynb : This file applies similarity search prototype learning on the 2 datasets

scgpt_linear_prob.ipynb : This file applies linear probing on the 2 datasets

scgpt_inference_linear_prob.ipynb : This file can be used for the inference of fined-tuned models
