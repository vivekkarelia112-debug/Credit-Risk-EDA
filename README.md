# Credit Risk Exploratory Data Analysis

## 📌 Project Overview

This project explores a credit risk dataset to understand the relationships between borrower characteristics, loan information, and loan default status.

Using Python and exploratory data analysis (EDA), the project examines patterns in loan defaults across factors such as income, employment length, loan amount, interest rate, loan intent, credit history, and home ownership.

The goal is to identify meaningful patterns in the dataset and communicate findings through statistical summaries and visualizations.

## 🎯 Objectives

- Understand the structure and characteristics of the dataset.
- Identify and handle duplicate records and implausible values.
- Examine the distribution of borrower and loan-related variables.
- Explore relationships between loan characteristics and default status.
- Visualize key patterns and summarize the findings.
- Practice data cleaning, exploratory analysis, and data visualization using Python.

## 📂 Project Structure

```text
01-Credit-Risk-EDA/
│
├── data/
│   └── credit_risk_dataset.csv
│
├── notebook/
│   └── credit_risk_eda.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## 🛠️ Tools and Technologies

- **Python** — Data analysis and programming
- **Pandas** — Data manipulation and cleaning
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Jupyter Notebook** — Interactive analysis

## 📊 Dataset

The dataset contains borrower information and loan-related variables, including:

- Age
- Annual income
- Home ownership
- Employment length
- Loan intent
- Loan grade
- Loan amount
- Interest rate
- Previous default history
- Credit history length
- Loan-to-income ratio
- Loan status

The original dataset contains **32,581 rows and 12 columns**.
**Source:** [Credit Risk Dataset — Kaggle](https://www.kaggle.com/laotse/credit-risk-dataset)  
**Creator:** Lao Tse  
**Licence:** CC0 1.0 Universal (Public Domain), as listed on Kaggle when checked.

## 🧹 Data Cleaning and Preparation

The notebook performs the following preparation steps:

- Preserves the original dataset in a separate DataFrame.
- Creates an analysis copy for cleaning.
- Removes exact duplicate rows.
- Excludes records with implausible ages above 100.
- Treats negative employment lengths and employment lengths greater than the applicant's age as missing values.
- Fills missing employment lengths and interest rates using their respective medians.
- Checks the cleaned data before proceeding with the analysis.

These decisions are assumptions made for this exploratory analysis and may influence the results.

## 🔍 Exploratory Data Analysis

The analysis investigates:

- Distributions of borrower and loan characteristics.
- Loan default distribution.
- Default patterns across loan grades and home ownership categories.
- Default rates across different loan intents.
- Differences in loan amounts, interest rates, income, employment length, and loan-to-income ratios between default and non-default groups.

## 💡 Key Findings

The cleaned analysis dataset contains **32,411 records**.

Key observations include:

- Approximately **21.87%** of records have a loan status of `1`, while **78.13%** have a loan status of `0`.
- The proportion of records with loan status `1` varies substantially across loan grades, increasing from **10.0% for Grade A** to **98.4% for Grade G**. Grade G has a relatively small sample size.
- Loan intent also shows differences: debt consolidation has a higher loan-status-`1` proportion than venture loans in this dataset.
- The loan-status-`1` group has higher median loan amounts, interest rates, and loan-to-income ratios than the loan-status-`0` group.
- The loan-status-`1` group has lower median annual income and employment length than the loan-status-`0` group.

These findings describe associations observed in the dataset. They do not establish causation.

## ⚠️ Limitations

- The analysis is exploratory and does not establish causal relationships.
- Data-cleaning decisions and median imputation may affect the results.
- Some categories contain relatively few observations, which can make their observed proportions less reliable.
- The findings may not generalize to other populations, lenders, or time periods.
- The dataset's target encoding and original source should be verified using the dataset documentation.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project directory

```bash
cd 01-Credit-Risk-EDA
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

Open `notebook/credit_risk_eda.ipynb` and run the cells from top to bottom.

Ensure the dataset is available at the relative path expected by the notebook.

## 📌 Future Improvements

- Add additional visualizations and deeper statistical analysis.
- Investigate relationships between multiple borrower characteristics.
- Explore feature engineering for a potential credit risk prediction model.
- Develop a machine learning model in a separate project.
- Improve documentation of the dataset source and cleaning assumptions.

## 👤 Author

Created as a data analytics portfolio project to practice Python, data cleaning, exploratory data analysis, and visualization.
