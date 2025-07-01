# Bank Term Deposit Campaign - Exploratory Data Analysis (EDA)

This project explores marketing data from a Portuguese banking institution to understand customer behavior and identify key factors that influence subscription to a term deposit. 

---

## 🔍 Problem Statement

The bank runs marketing campaigns to encourage clients to subscribe to term deposits. The goal is to analyze past campaign data to discover which customer attributes and campaign strategies are most effective in achieving a positive response.

---

## 🎯 Objective

- Perform exploratory data analysis (EDA) on customer and campaign-related data.
- Identify patterns, trends, and insights that influence the likelihood of a customer subscribing to a term deposit (`response` variable).
- Provide visual summaries and business recommendations.

---

## 📁 Dataset Overview

- **Source**: Provided as CSV file (`bank_marketing_updated_v1.csv`)
- **Records**: 45,213 customers
- **Target Variable**: `response` (yes/no)
- **Key Features**:
  - Demographics: `age`, `marital`, `jobedu`, `salary`, `balance`
  - Financial: `housing`, `loan`, `default`
  - Campaign: `contact`, `duration`, `campaign`, `pdays`, `previous`, `poutcome`

---

## 🛠️ Tools & Libraries Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📊 EDA Steps

1. **Data Cleaning**:
   - Removed headers from metadata rows
   - Handled missing/null values
   - Corrected inconsistent data types

2. **Univariate Analysis**:
   - Distributions of age, salary, balance
   - Count plots for categorical variables like marital status and housing

3. **Bivariate Analysis**:
   - `response` vs job, education, housing, etc.
   - Duration of call vs success rate

4. **Correlation Analysis**:
   - Analyzed feature correlations with the target variable

5. **Visualizations**:
   - Bar plots, histograms, pie charts, and heatmaps

---

## 💡 Key Insights

- Subscription rates are higher among customers with specific jobs like admin or students.
- Campaigns involving long-duration calls show higher conversion.
- Customers without loans or defaults show better response rates.
- Unknown or secondary contact methods perform worse than personal calls.

---

## 📌 Project Structure

```
├── EDA_Code.ipynb              # Jupyter notebook with code and analysis
├── bank_marketing_updated_v1.csv  # Raw dataset
├── README.md                   # Project overview (this file)
├── Bank_Term_Deposit_EDA_Report.pdf  # PDF report with visuals and insights
```

---

## 📄 Report

You can view the complete PDF report here:  
👉 [Bank_Term_Deposit_EDA_Report.pdf](./Bank_Term_Deposit_EDA_Report.pdf)

---

## 🚀 Future Work

- Feature engineering for ML classification
- Model training (Logistic Regression, Random Forest, etc.)
- Predictive dashboard deployment