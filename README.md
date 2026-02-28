# Insurance Charges Prediction 📊

This project predicts individual insurance charges using personal characteristics. It demonstrates the **full data science workflow**, including exploratory data analysis (EDA), feature engineering, and machine learning model development.

---

## 📊 Insights & Results

### 1️⃣ Exploratory Data Analysis
- Initial EDA revealed that being a **smoker** has the highest correlation with insurance charges (Pearson correlation ~0.79), highlighting its significant impact on healthcare costs.
- Example visualization:

![Smoker vs Charges](images/smoker_charges.png)

### 2️⃣ Model Performance
- After preprocessing and feature engineering, several machine learning models were trained.
- The **Random Forest Regressor** emerged as the top performer, achieving a strong **R² Score of 86.54%**.
- Demonstrates the model’s effectiveness in predicting insurance charges based on individual characteristics.

---

## 🛠️ Technical Workflow

### 1️⃣ Data Preprocessing
- Removed duplicate entries.
- Performed **label encoding** for binary categorical features (`sex`, `smoker`).
- Applied **one-hot encoding** for multi-category features (`region`).
- Standardized numerical features using **StandardScaler**.

### 2️⃣ Feature Engineering
- Created a new feature **`bmi_category`** (underweight, normal, overweight, obese) from the `bmi` column.
- Improved predictive power of the dataset.
- Example visualization:

![BMI Categories](images/bmi_category.png)

### 3️⃣ Model Training & Evaluation
- Built and evaluated multiple regression models:
  - Linear Regression
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors (KNN)
  - XGBoost
- Used **Scikit-learn** and **XGBoost** libraries to find the most accurate predictor.

### R² Score Comparison of Models

| Model               | R² Score |
|-------------------|----------|
| Random Forest      | 0.865369 |
| XGBoost            | 0.847802 |
| Linear Regression  | 0.804071 |
| KNN                | 0.749705 |
| Decision Tree      | 0.744208 |

- Random Forest and XGBoost are the top performers, indicating robust predictive capability.

### 4️⃣ Full Data Science Lifecycle
- Applied end-to-end data science:
  - Data cleaning and preprocessing
  - Feature engineering
  - Model selection and evaluation
  - Actionable insights extraction

---
