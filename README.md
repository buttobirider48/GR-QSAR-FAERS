# GR-QSAR-FAERS

Machine-learning classification of glucocorticoid receptor affinity and application to FAERS drugs.

## Overview

This repository contains the analysis notebook used to develop a machine-learning model for classifying compounds with high affinity for the human glucocorticoid receptor (GR) and to apply the resulting model to drug structures identified in the FDA Adverse Event Reporting System (FAERS).

High GR affinity was operationally defined as pKi ≥ 8.0. The model was developed using molecular descriptors and evaluated using nested cross-validation. The applicability domain was assessed before interpreting predictions for FAERS drug structures.

This repository provides the model-development and drug-prediction workflow. The disproportionality analysis of adverse event reports was conducted separately and is described in the accompanying manuscript.

## Repository structure

```text
GR-QSAR-FAERS/
├── data/
│   └── README.md
├── notebooks/
│   ├── GR_QSAR_model_FAERS_prediction_GitHub_ready.ipynb
│   └── README.md
├── results/
│   └── README.md
├── .gitignore
├── LICENSE
└── README.md

