# Housing Price Prediction – Multiple Linear Regression 🏡

A case study leveraging multiple linear regression to model and predict housing prices based on key property features.

---

## 🎯 Problem Statement

Real estate stakeholders—buyers, sellers, and investors—need reliable estimates of home values based on property features like area, number of bedrooms, and location. This project aims to build an interpretable regression model that quantifies the relationship between these features and house prices.

---

## 🗂 Dataset Overview

- **Filename**: `housing.csv`
- **Sample Size**: ~ X – specify number of rows
- **Features Included**:
  - `area` (sq ft)
  - `bedrooms`
  - `bathrooms`
  - `stories`
  - `parking`
  - `mainroad` (yes/no)
  - `guestroom` (yes/no)
  - `furnishingstatus` (furnished/semi-furnished/unfurnished)
  - … and other relevant attributes
- **Target Variable**: `price` (house selling price)

---

## 🧰 Tools & Libraries

- Python 3.x (Jupyter Notebook)
- pandas, NumPy — data manipulation
- matplotlib, seaborn — visual analysis
- scikit-learn / statsmodels — linear regression modeling

---

## 🚀 EDA & Modeling Workflow

1. **Data Preparation**  
   - Import CSV and inspect for missing values & inconsistencies  
   - Encode categorical variables (e.g., `mainroad`, `furnishingstatus`)  
   - Detect and handle outliers

2. **Exploratory Data Analysis**  
   - Univariate stats: histograms, box plots for distributions  
   - Bivariate plots: scatter, bar plots, correlation heatmaps  
   - Insight examples:
     - Larger area → higher price  
     - Furnished homes outperform unfurnished ones  
     - Parking capacity shows a moderate price uptick

3. **Feature Selection**  
   - Evaluate correlation matrix  
   - Use tools like Variance Inflation Factor (VIF) to check multicollinearity  
   - Select an optimal subset of predictors

4. **Model Building**  
   - Split dataset into training/test sets (e.g., 80/20)  
   - Train multiple linear regression using training data  
   - Evaluate using R², RMSE, MAE

5. **Performance & Validation**  
   - Display training vs test performance  
   - Perform residual analysis to assess linearity, homoscedasticity, and normality assumptions  
   - Optionally refine model via feature transformation or interaction terms

---

## 📈 Key Findings (Example)

- **Positive Correlates**: `area`, `bedrooms`, `bathrooms`, `parking`
- **Categorical Impacts**: Furnishing status adds an average premium of ₹X lakhs  
- **Model Performance**:
  - Training R² ≈ 0.75  
  - Test R² ≈ 0.72  
  - RMSE ~ ₹Y lakhs, indicating acceptable error margins

---

## 🗂 Project Structure

```
├── housing.csv                              # Raw dataset
├── Housing_Case_Study_Linear_Regression.ipynb  # Analysis notebook
├── README.md                                # Project overview (this file)
└── Optional: model_artifacts/, visuals/     # Saved plots or models
```

---

*Created by Shivansh – feel free to explore the notebook and experiment further!*