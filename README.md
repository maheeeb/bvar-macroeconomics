# 🇮🇩 BVAR Analysis of Indonesia’s Macroeconomic Variables (2015–2024)

This repository contains a research project analyzing the dynamic interactions among several key macroeconomic variables in Indonesia using a **Bayesian Vector Autoregressive (BVAR)** model. The variables studied include:

- Rupiah exchange rate  
- Exports  
- Imports  
- Gold prices
- Inflation

## 📘 Overview

This research aims to address the limitations of conventional VAR models, particularly the issue of overparameterization, by applying a BVAR approach with:

- **Hierarchical Minnesota priors**
- **Markov-Chain Monte Carlo (MCMC)** estimation

The study covers data from **2015 to 2024**.

## 🧪 Methodology

- **Data Processing**:  
  All time series were made stationary through first-order differencing and normalized using z-score transformation.

- **Lag Selection**:  
  Optimal lag length determined using the **Akaike Information Criterion (AIC)**, with **lag 6** selected.

- **Model Evaluation**:  
  Evaluated using **Mean Absolute Percentage Error (MAPE)**:
  - Gold Price (Train): **10.09%**
  - Inflation (Train): **3.74%**
  - Test performance shows challenges due to high uncertainty during the test period.

- **Impulse Response Function (IRF)**:  
  Analysis used to understand short-term dynamic effects, such as:
  - Exchange rate depreciation’s impact on inflation
  - Export growth leading to a temporary drop in imports

## 📌 Key Insights

- BVAR effectively models macroeconomic interactions under data and parameter constraints.
- Captures meaningful short-term relationships between variables.
- Performs well on in-sample data but shows sensitivity to high uncertainty in out-of-sample forecasts.

## 📁 Contents

- `data4.xlsx` – Preprocessed macroeconomic time series  
- `Syntax.rmd` – Model building and evaluation code (BVAR, MCMC, IRF, etc.)  
 

## 🔧 Tools & Libraries

- R `BVAR` package

## 📜 License

This project is for academic purposes. Feel free to explore, cite, and adapt with credit.


