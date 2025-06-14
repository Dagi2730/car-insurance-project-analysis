# 🚗 AlphaCare Car Insurance Risk Analytics Project

## 🧠 Business Objective

AlphaCare Insurance Solutions (ACIS) aims to modernize its marketing and risk-based pricing strategies by leveraging advanced data analytics and machine learning. This project focuses on analyzing historical car insurance data in South Africa to:

- Optimize marketing strategies.
- Identify low-risk customer segments eligible for premium reductions.
- Build a data-driven, dynamic pricing model.

---

## 🗂️ Project Structure

This repository contains all code, analysis notebooks, and outputs for a complete end-to-end analytics pipeline, structured around four main tasks:

car-insurance-project-analysis/
│
├── data/ # Raw and processed datasets (DVC-tracked)
├── notebooks/ # Jupyter Notebooks for EDA, modeling, hypothesis tests
├── scripts/ # Reusable code scripts and functions
├── models/ # Trained models and evaluation results
├── reports/ # Interim and final reports
├── .dvc/ # DVC configuration
├── .github/workflows/ # CI/CD setup
├── requirements.txt # Project dependencies
└── README.md # Project overview


---

## 🔍 Task Overview

### ✅ Task 1: Exploratory Data Analysis (EDA) & Statistical Understanding

**Goals:**
- Understand claim and premium distributions
- Discover high-risk vs low-risk segments
- Identify outliers, trends, and data quality issues

**Key EDA Components:**
- **Loss Ratio Analysis:** TotalClaims / TotalPremium
- **Temporal Patterns:** Month-wise trends in claim frequency/severity
- **Geographic Risk:** Province and postal code comparisons
- **Vehicle Analysis:** Claims by Make, Model, and VehicleType
- **Gender and Risk:** Claims and premium differences by gender
- **Outlier Detection:** Boxplots on financial and vehicle attributes

**Visual Output:**
- Histograms, heatmaps, correlation plots, box plots
- 3+ creative visualizations capturing key insights

---

### ✅ Task 2: Data Version Control (DVC)

**Goals:**
- Ensure reproducibility and auditability of data pipelines
- Track data versions and enable rollbacks

**Steps Implemented:**
- Initialized DVC in the project
- Configured local remote storage
- Tracked historical insurance datasets via `dvc add`
- Synced data versions with Git via `.dvc` metadata

---

### ✅ Task 3: Hypothesis Testing

**Objective:** Statistically validate or reject assumptions about risk and profitability to inform segmentation strategy.

**Tested Null Hypotheses (H₀):**
1. No risk difference across provinces  
2. No risk difference between zip codes  
3. No margin (TotalPremium - TotalClaims) difference between zip codes  
4. No risk difference between women and men  

**Approach:**
- Used chi-squared, t-tests, and z-tests
- Segmented control/test groups
- Computed claim frequency, severity, and margin

**Business Interpretation:** 
Rejected hypotheses provided actionable guidance for pricing adjustments by region, gender, and location.

---

### ✅ Task 4: Predictive Modeling

**Subtasks:**
1. **Risk Model (Claim Severity):**
   - Predict `TotalClaims` using regression models
   - Models: Linear Regression, Random Forest, XGBoost
   - Evaluation: RMSE, R²

2. **Pricing Model (Premium Optimization):**
   - Predict `CalculatedPremiumPerTerm`
   - Explore probability-based pricing:  
     `Premium = P(Claim) × Severity + Expenses + Margin`
   - Classification model for claim probability

3. **Interpretability:**
   - SHAP or LIME used to explain top 5–10 important features
   - Business-driven interpretations (e.g., vehicle age effect)

---

## 🧾 Data Description

**Time Period:** February 2014 – August 2015  
**Data Domains:**

- **Client Info:** Gender, MaritalStatus, Citizenship, VAT, Bank, etc.  
- **Location:** Province, Country, ZipCode, CrestaZones  
- **Vehicle Info:** Make, Model, Year, CubicCapacity, BodyType, etc.  
- **Policy Info:** CoverType, Product, TermFrequency, Excess, SumInsured  
- **Claims & Premiums:** TotalPremium, TotalClaims

---

## 💡 Final Deliverables

- **Insights Report:** Data-driven strategies for regional pricing, gender-based adjustments, and vehicle risk profiling
- **Risk and Pricing Models:** Predictive analytics tools to support dynamic insurance pricing
- **EDA Dashboard (Optional):** Visual summary of portfolio metrics
- **CI/CD & DVC Integration:** Ensures reproducibility, traceability, and audit-readiness

---

## Author

Dagmawit Andargachew
