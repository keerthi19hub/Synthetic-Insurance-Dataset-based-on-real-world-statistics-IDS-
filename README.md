# 📊 Synthetic Insurance Analytics — Actuarial Modeling & Risk Stratification Framework

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1E1B4B,3730A3,6366F1&height=220&section=header&text=Synthetic%20Insurance%20Analytics&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Actuarial%20Modeling%20%26%20Risk%20Stratification%20Framework&descSize=18&descAlignY=60&descAlign=50" width="100%" alt="Insurance Analytics Banner" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Actuarial%20Data%20Science-1E1B4B?style=for-the-badge" alt="Actuarial Science" />
  <img src="https://img.shields.io/badge/Language-Python%203.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Library-Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="Scikit-Learn" />
  <img src="https://img.shields.io/badge/Tool-Jupyter%20Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
  <img src="https://img.shields.io/badge/Modeling-Regression%20%26%20Cost%20Estimation-6366F1?style=for-the-badge" alt="Cost Modeling" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

---

## 📌 Table of Contents

- [📖 Executive Summary](#-executive-summary)
- [🎯 Real-World Problem & Actuarial Context](#-real-world-problem--actuarial-context)
- [✨ Key Features & Findings](#-key-features--findings)
- [🏗️ Predictive Modeling Pipeline](#️-predictive-modeling-pipeline)
- [🛠️ Tech Stack Matrix](#️-tech-stack-matrix)
- [⚙️ Reproducible Quickstart & Setup](#️-reproducible-quickstart--setup)
- [📁 Project Structure](#-project-structure)
- [👩‍💻 Author & Contributions](#-author--contributions)

---

## 📖 Executive Summary

The **Synthetic Insurance Analytics & Risk Stratification Framework** is an actuarial data science project modeling health insurance claim charges across demographic, clinical, and regional lifestyle variables. Utilizing synthetic data calibrated against empirical real-world medical statistics, the project applies parametric regression and machine learning estimators to quantify non-linear premium cost drivers, assess tobacco consumption penalties, and model pediatric coverage variance.

---

## 🎯 Real-World Problem & Actuarial Context

- **The Problem:** Setting accurate insurance policy premiums requires precise risk stratification. Underestimating claims leads to underwriting insolvency, while overcharging prices out low-risk policyholders. Disentangling collinear interactions between BMI, smoking status, age, and regional hospital overhead is critical for actuarial solvency.
- **The Solution:** A transparent computational pipeline that conducts bivariate statistical hypothesis testing, feature transformation, and comparative regression modeling to provide reliable cost expectation curves.

---

## ✨ Key Features & Findings

- **🚬 The Smoking Multiplier:** Smoking status emerges as the single most punitive cost coefficient, multiplying expected claims by 3.5×–4× across equivalent age cohorts.
- **⚖️ Non-Linear BMI Interactions:** Observed severe synergistic cost spikes when high BMI (>30) co-occurs with tobacco use.
- **👶 Dependent Child Elasticity:** Modeled incremental claim risk scaling with dependent count.
- **📉 Comprehensive Actuarial Visualizations:** Residual distribution plots, feature weight bar charts, and cost-density curves.

---

## 🏗️ Predictive Modeling Pipeline

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                       Actuarial Data Science Pipeline                       │
└─────────────────────────────────────────────────────────────────────────────┘
                                       │
                                       ▼
               ┌──────────────────────────────────────────────┐
               │ Synthetic Healthcare Dataset (Empirically)   │
               │ (Age, Sex, BMI, Children, Smoker, Region)    │
               └───────────────────────┬──────────────────────┘
                                       │
                                       ▼
               ┌──────────────────────────────────────────────┐
               │    Exploratory Analysis & Transformations    │
               │  - Outlier bounds and log-charge analysis    │
               │  - Categorical dummy / one-hot encoding      │
               │  - Polynomial interaction feature generation │
               └───────────────────────┬──────────────────────┘
                                       │
                                       ▼
               ┌──────────────────────────────────────────────┐
               │        Predictive Regression Suite           │
               │  - Ordinary Least Squares (OLS) Regression   │
               │  - Ridge / Lasso Regularized Models          │
               │  - Random Forest Regressor                   │
               │  Metrics: R² Score, RMSE, MAE                │
               └──────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack Matrix

| Category | Tools & Libraries | Role |
| :--- | :--- | :--- |
| **Language** | Python 3.10+ | Scientific computing and actuarial modeling |
| **Regression & ML** | Scikit-Learn | Linear models, regularized regression, ensemble modeling |
| **Data Processing** | Pandas, NumPy | Data cleaning, quantile filtering, interaction terms |
| **Visualization** | Seaborn, Matplotlib | Regression curves, residual analysis, distribution KDEs |
| **Notebook** | Jupyter Notebook | Executable research environment |

---

## ⚙️ Reproducible Quickstart & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/keerthi19hub/Synthetic-Insurance-Dataset-based-on-real-world-statistics-IDS-.git
cd Synthetic-Insurance-Dataset-based-on-real-world-statistics-IDS-
```

### 2. Environment Setup & Dependencies
```bash
python -m venv venv
venv\Scripts\activate  # On Linux/macOS: source venv/bin/activate

pip install pandas numpy scikit-learn seaborn matplotlib jupyter
```

### 3. Run Analysis Notebook
```bash
jupyter notebook "Synthetic Insurance Dataset based on real world statistics(IDS) (3).ipynb"
```

---

## 📁 Project Structure

```text
Synthetic-Insurance-Dataset-based-on-real-world-statistics-IDS-/
├── Synthetic Insurance Dataset based on real world statistics(IDS) (3).ipynb # Primary analysis notebook
└── README.md                                                                 # Technical documentation
```

---

## 👩‍💻 Author & Contributions

**Keerthi N**  
- **GitHub:** [@keerthi19hub](https://github.com/keerthi19hub)  
- **Portfolio:** [keerthi19hub.github.io](https://keerthi19hub.github.io)  
- **Course:** Introduction to Data Science (IDS) · Alliance University, Bengaluru  
- **Role:** Dataset synthesis analysis, statistical regression modeling, and actuarial cost report generation.

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1E1B4B,3730A3,6366F1&height=100&section=footer" width="100%" alt="Footer Banner" />
</p>
