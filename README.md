# GR-QSAR-FAERS

Machine-learning classification of glucocorticoid receptor affinity and application to FAERS drugs.

## Overview

This repository contains the Python code used for model development, applicability-domain assessment, SHAP-based model interpretation, and prediction of GR affinity classes for FAERS drug structures. FAERS disproportionality analyses, including the main analysis, applicability-domain sensitivity analysis, route-restricted subgroup analysis, volcano plots, and summary tables, were performed using JMP Student Edition and are described in the accompanying manuscript. The numerical results underlying these analyses are reported in the accompanying manuscript and Supporting Information.

High GR affinity was operationally defined as pKi ≥ 8.0. The model was developed using molecular descriptors and evaluated using nested cross-validation. The applicability domain was assessed before interpreting predictions for FAERS drug structures.

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
```

## Analysis workflow

The notebook performs the following analyses:

1. Loading and preprocessing GR binding-affinity data
2. Definition of high and non-high GR affinity classes
3. Molecular descriptor preprocessing
4. Feature selection
5. Nested cross-validation
6. Algorithm and hyperparameter optimization
7. Final model construction
8. Applicability-domain assessment
9. SHAP-based model interpretation
10. Prediction of GR affinity classes for FAERS drug structures
11. Descriptive comparison with available measured pKi values

## Input data

The required input files and their expected formats are described in:

- [`data/README.md`](data/README.md)

The original BindingDB and FAERS source data are not included in this repository. Users should obtain the data from the original data providers and comply with their applicable terms of use.

## Usage

1. Clone or download this repository.
2. Place the required input files in the `data` directory.
3. Install the required Python packages.

Install the required packages using:

```bash
pip install -r requirements.txt
```

4. Open the notebook in the `notebooks` directory.
5. Run the notebook cells in order.

The generated files are saved in the `results` directory.

## Interpretation

The model classifies compounds according to GR binding affinity and does not distinguish functional modes of action, such as agonism, partial agonism, or antagonism.

Disproportionality signals obtained from FAERS represent reporting associations and do not establish causal relationships between GR affinity and adverse events.

## Citation

Citation information will be added after publication of the accompanying manuscript.

## License

The analysis code in this repository is available under the MIT License. The original data sources remain subject to their respective terms of use and licensing conditions.
