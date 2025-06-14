# 🚗 ACIS Car Insurance Analysis – Task 1: EDA & Statistical Thinking

Welcome to the exploratory data analysis (EDA) phase of the **AlphaCare Insurance Solutions (ACIS)** car insurance project. This repository contains all analysis and visualizations related to understanding the insurance data, assessing risks, and uncovering key drivers of claims and premiums in South Africa.

---

## 📁 Repository Structure

car-insurance-project-analysis/
│
├── data/ # Raw and processed data files
├── notebooks/# .ipynb files for cleaning,eda & additional analysis
├── README.md # This file
└── requirements.txt # Project dependencies


---

## 🧠 Business Context

AlphaCare Insurance Solutions (ACIS) is seeking to optimize its marketing strategy and identify low-risk customers for targeted discounts. The dataset includes historical insurance data containing premiums, claims, customer demographics, and vehicle information.

---

## 🎯 Objectives of Task 1

1. Perform deep exploratory data analysis on the provided dataset.
2. Assess distribution, variance, and presence of outliers in critical variables like:
   - `TotalPremium`
   - `TotalClaims`
   - `LossRatio`
3. Perform statistical tests (e.g., normality testing) to guide later modeling choices.
4. Explore geographic and group-based trends (e.g., Province, Gender, VehicleType).
5. Calculate correlations in monthly trends between premiums and claims.
6. Create actionable visualizations to communicate insights.

---

## ✅ Key Achievements

### 🔍 Data Quality & Cleaning
- Handled missing values and verified data types.
- Detected and flagged extreme outliers in `TotalClaims`, `LossRatio`, and `CustomValueEstimate`.

### 📊 Univariate & Bivariate Analysis
- Distribution analysis of key financial metrics using histograms and violin plots.
- Bar plots comparing average Loss Ratio across Province, Gender, and Vehicle Type.

### 📈 Correlation & Time-Series Thinking
- Computed monthly percentage changes in premiums and claims by `ZipCode`.
- Filtered ZipCodes with insufficient or non-variable data.
- Found meaningful correlation ranges between premium and claim trends.

### 📍 Geographic Trends
- Compared premiums, claims, and vehicle types by Province and ZipCode.
- Found regions with high risk vs. profitability potential.

### 🧪 Statistical Thinking
- Normality tests using Shapiro-Wilk showed non-normal distributions (important for modeling).
- Logical segmentation for future hypothesis testing (e.g., Loss Ratio across Genders or Provinces).

---

## 🌟 Top 3 Visualizations

1. **Violin Plot – Premium Distribution by Vehicle Type**  
   Clear differences in median premiums; luxury and SUV types show higher risk exposure.

2. **Bar Chart – Loss Ratio by Province**  
   Reveals specific provinces with unsustainably high claims relative to premiums.

3. **Time-Series Plot – Monthly Premium vs. Claims**  
   Highlights divergence or alignment in financial activity over time.

> All plots styled using seaborn/matplotlib with clean palettes, annotations, and improved readability.

---

## 🛠️ Tech Stack

- Python 3.12
- pandas, numpy
- seaborn, matplotlib
- scipy.stats (for statistical testing)
- Jupyter Notebook
- Git, GitHub

---

## 🚧 Next Steps

- [ ] Task 2: Hypothesis testing and inferential statistics
- [ ] Task 3: Predictive modeling and targeting low-risk customers
- [ ] Final dashboard and reporting (Week 3)

---

## 📌 How to Run

1. Clone the repository  
   `git clone https://github.com/your-username/car-insurance-project-analysis.git`

2. Navigate and activate virtual environment  

3. Run the notebook in Jupyter or VS Code  
Open `notebooks/task_1_eda.ipynb` to explore the EDA.

---

## 👩‍💼 Maintainer

Dagmawit Andargachew

---

