# Hybrid Physics–Machine Learning Modeling of Gas Adsorption on Zeolites

## Overview

This repository presents a **research-oriented comparison between classical adsorption isotherm models and machine learning approaches** for predicting gas adsorption behaviour. The study focuses on **CO₂ and CH₄ adsorption on ammonium ZSM-5**, integrating physics-based modeling with data-driven regression techniques.

The objective is to evaluate when traditional thermodynamic models remain sufficient and when modern ML models provide superior predictive capability.

---

## Key Features

* Comparative modeling of **Langmuir**, **Freundlich**, and ML-based adsorption predictions.
* Implementation of **ElasticNet regression** and **XGBoost/Random Forest** models.
* Quantitative evaluation using RMSE and R² metrics.
* Physics-informed interpretation of adsorption behaviour.
* Research-grade analysis suitable for chemical engineering and materials science applications.

---

## Dataset

* Experimental adsorption data for:

  * CO₂ adsorption
  * CH₄ adsorption
* Variables include:

  * Pressure
  * Adsorption loading (mmol/g)
  * Gas identity

The dataset reflects heterogeneous surface adsorption behaviour typical of zeolitic materials.

---

## Modeling Approaches

### 1. Physics-Based Models

* **Langmuir Isotherm**

  * Assumes monolayer adsorption and uniform surface sites.
* **Freundlich Isotherm**

  * Captures heterogeneous adsorption energetics.

### 2. Machine Learning Models

* ElasticNet Polynomial Regression
* Gradient-boosted tree / ensemble models

ML models learn nonlinear adsorption relationships without explicit thermodynamic assumptions.

---

## Main Results & Scientific Insights

### CO₂ Adsorption

* Freundlich model shows strong performance.
* Indicates physically regular adsorption governed by energetics.
* ML provides modest improvement but does not outperform Freundlich significantly.

### CH₄ Adsorption

* Langmuir model performs poorly.
* ML models achieve near-perfect predictive accuracy.
* Suggests complex adsorption mechanisms not captured by classical equations.

### Research Conclusion

Physics-based models retain interpretability and accuracy for strongly interacting gases, whereas ML models excel for weakly adsorbing systems with nonlinear behaviour.

---

## Repository Structure

```
├── Comparison.ipynb           # Main analysis notebook
├── CO2_CH4_Compiled_Data.csv  # Adsorption dataset
├── README.md                  # Project documentation
```

---

## Installation

Clone the repository:

```
git clone <your-repo-link>
cd <repo-name>
```

Install required packages:

```
pip install numpy pandas scikit-learn xgboost matplotlib seaborn
```

---

## Usage

Run the notebook:

```
jupyter notebook Comparison.ipynb
```

The notebook includes:

* Data preprocessing
* Isotherm fitting
* ML model training
* Performance comparison
* Physics-based interpretation

---

## Research Applications

* Adsorbent screening and optimization
* Hybrid physics–ML modeling
* Carbon capture material studies
* Chemical engineering process modeling

---

## Citation

If you use this work in research, please cite:

```
Hybrid Physics–Machine Learning Modeling of Gas Adsorption on Zeolites, GitHub Repository.
```

---

## Future Work

* Physics-informed neural networks for adsorption modeling
* Multi-temperature isotherm integration
* Transfer learning across different zeolite frameworks

---
