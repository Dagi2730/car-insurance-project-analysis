# 🚗 AlphaCare Insurance Solutions - Task 1: Exploratory Data Analysis (EDA)

## 🔍 Overview

This branch contains the **exploratory data analysis (EDA)** for the car insurance dataset provided by AlphaCare Insurance Solutions. The goal of Task 1 is to understand the data, clean it, and uncover initial insights that will inform future modeling and marketing strategies.

---

## ✅ What We Did

- 🧹 **Data Cleaning**
  - Dropped rows with missing values in key columns to maintain data integrity.
  - Removed columns with excessive missing data or low relevance (`Gender`, `MaritalStatus`).

- 📊 **Univariate Analysis**
  - Visualized distributions for numeric variables like:
    - `TotalPremium`
    - `TotalClaims`
    - `SumInsured`
    - `CalculatedPremiumPerTerm`
  - Plotted counts for categorical variables such as:
    - `Bank`
    - `VehicleType`
    - `Province`
    - `NewVehicle`

- 📈 **Bivariate Analysis**
  - Boxplots showing relationships between:
    - `TotalPremium` and `VehicleType`
    - `TotalPremium` and `Province`
    - `TotalPremium` and `NewVehicle`
  - Scatter plots for numeric pairs like:
    - `SumInsured` vs `TotalPremium`

- 🔗 **Correlation Analysis**
  - Correlation heatmap for numeric variables to identify linear associations.

- 🧊 **Multivariate Insights** (limited)
  - Boxplots combining `TotalPremium` by `VehicleType` and `NewVehicle`.
  - Heatmap for counts of `Province` vs `VehicleType`.
  - Stacked bar charts showing `CoverType` distribution across `Product`.

---

## 🛠 How to Run

1. Clone this branch and create your Python environment:
   ```bash
   git checkout task-1
   python -m venv venv
   source venv/bin/activate  # or .\venv\Scripts\activate on Windows
   ```

📂 Project Structure
bash
Copy
Edit
task-1/
├── notebooks/           # Jupyter notebooks for EDA and visualization
├── data/                # Raw and cleaned datasets
├── visuals/             # Generated plots and charts
├── README.md            # This README file
└── requirements.txt     # Python dependencies



