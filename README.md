# Actuarial Risk Analysis & Healthcare Insurance Charge Modeling

> **An Introduction to Data Science (IDS) research project analyzing medical insurance charges, demographic risk factors, and actuarial distributions using statistical hypothesis testing and predictive analytics.**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://python.org)
[![Data Science](https://img.shields.io/badge/Domain-Actuarial%20Analytics-green)](https://github.com/keerthi19hub)
[![Statistics](https://img.shields.io/badge/Statistics-SciPy%20%7C%20Statsmodels-blue)](https://www.statsmodels.org/)
[![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-F37626?logo=jupyter&logoColor=white)](https://jupyter.org)

---

## 1. Project Overview

In healthcare insurance, underwriting risk and setting premium charges require precise statistical modeling of patient attributes.

This project, developed for the **Introduction to Data Science (IDS)** curriculum, performs a rigorous empirical study on a synthetic insurance dataset calibrated against real-world healthcare statistics. The study models how lifestyle indicators (smoking status, BMI), demographics (age, gender, dependents), and regional factors influence total annual medical expenditures.

---

## 2. Key Attributes & Feature Schema

The dataset captures customer records across the following actuarial dimensions:
- `age`: Primary policyholder age (years).
- `sex`: Policyholder gender (`male`, `female`).
- `bmi`: Body Mass Index providing an objective index of body weight relative to height ($kg/m^2$).
- `children`: Number of dependent children/dependents covered by health insurance.
- `smoker`: Binary indicator of smoking status (`yes`, `no`).
- `region`: Residential area in the US (`northeast`, `southeast`, `southwest`, `northwest`).
- **`charges`** *(Target)*: Individual medical expenses billed by health insurance ($).

---

## 3. Statistical Analysis & Hypotheses

### 1. Smoker Impact on Billed Charges
- **Hypothesis ($H_0$):** Medical charges for smokers and non-smokers follow identical distributions.
- **Methodology:** Independent two-sample t-test (`scipy.stats.ttest_ind`) and Mann-Whitney U test.
- **Finding:** Strongly rejected ($p < 10^{-10}$). Smoking is the single largest multiplier of healthcare charges, shifting the median cost by more than \$20,000 annually.

### 2. BMI and Obesity Interaction
- Customers with a $BMI \ge 30$ who smoke experience a compounding non-linear surge in billed charges compared to either factor in isolation.

### 3. Regional Variance
- One-way ANOVA testing was performed to evaluate charge differences across geographic regions (Southeast exhibits slightly higher mean charges due to elevated regional obesity indicators).

---

## 4. Technology Stack

- **Language:** Python 3.10+
- **Data Manipulation:** `pandas`, `numpy`
- **Statistical Analysis:** `scipy.stats` (norm, ttest_ind, chi2_contingency), `statsmodels.api`
- **Visualization:** `seaborn`, `matplotlib`
- **Preprocessing:** `scikit-learn` (`LabelEncoder`, `StandardScaler`)

---

## 5. Repository Structure

```
Synthetic-Insurance-Dataset-based-on-real-world-statistics-IDS-/
├── Synthetic Insurance Dataset based on real world statistics(IDS) (3).ipynb
└── README.md
```

---

## 6. Setup & Execution

```bash
# 1. Clone repository
git clone https://github.com/keerthi19hub/Synthetic-Insurance-Dataset-based-on-real-world-statistics-IDS-.git
cd Synthetic-Insurance-Dataset-based-on-real-world-statistics-IDS-

# 2. Virtual environment
python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/macOS

# 3. Dependencies
pip install pandas numpy seaborn matplotlib scipy statsmodels scikit-learn jupyter

# 4. Launch notebook
jupyter notebook
```

---

## 7. Author & Academic Context

- **Author:** **Keerthi N** (*Alliance University, BCA*)
- **Course:** Introduction to Data Science (IDS)
- **Verified Contribution:** Authored statistical pipeline, hypothesis tests, distribution plots, and correlation models.

---

## 8. License

Released under the [MIT License](https://opensource.org/licenses/MIT).
