# Vietnam House Price Prediction

> **Status:** 🚧 Work in progress (started October 2026)

Predicting Vietnamese property **listing prices** from listing attributes
(area, location, number of rooms, ...), using public data from Kaggle.

**Important:** the data contains *asking prices* posted by sellers, not actual
transaction prices. Results only describe listing prices for the population
the dataset represents.

## Project goals

- Build a leakage-safe machine learning pipeline for price prediction
- Compare models against a simple baseline using cross-validation
- Explain predictions and report prediction intervals
- Deliver a small interactive demo

## Data

- Source: Kaggle — *TBD (dataset selection in progress)*
- The raw data is **not** included in this repository.
  Download it from the source above and place the files in `data/raw/`.

## Setup

Requires [conda](https://docs.conda.io/) (Miniconda or Anaconda).

```bash
git clone git@github.com:dnhoang-2006/vn-house-price.git
cd vn-house-price
conda env create -f environment.yml
conda activate vnhp
jupyter notebook
```

## Project structure

```
vn-house-price/
├── data/raw/          # raw data (not tracked by git)
├── notebooks/         # Jupyter notebooks, numbered in order
├── src/               # reusable Python code
├── reports/           # project design and final report
├── environment.yml    # conda environment
└── README.md
```

## Roadmap

- [x] Project setup and environment
- [ ] Dataset selection and data design
- [ ] Data cleaning
- [ ] Exploratory data analysis
- [ ] Baseline and machine learning models
- [ ] Model explanation and error analysis
- [ ] Demo app and final report