# Titanic Survival Prediction

🚀 **Random Forest outperformed Logistic Regression, achieving ROC-AUC of 0.890**

This project builds and compares machine learning models to predict passenger survival on the Titanic dataset. It demonstrates a complete end-to-end workflow, from data preprocessing to model evaluation and interpretation.

---

## 📊 Project Overview

The goal of this project is to:
- Build a baseline classification model
- Improve performance using a more advanced model
- Interpret key factors influencing survival

---

## 📁 Dataset

The dataset contains passenger-level information such as:
- Age
- Sex
- Passenger class (Pclass)
- Fare
- Embarkation port

**Target variable:**
- `Survived` (0 = did not survive, 1 = survived)

---

## 🧹 Data Preprocessing

The following steps were applied:
- Removed irrelevant columns: `Name`, `Ticket`, `Cabin`, `PassengerId`
- Imputed missing values:
  - `Age` → median
  - `Embarked` → mode
- Converted categorical variables using one-hot encoding

---

## 🤖 Models

Two models were built and compared:

### 1. Logistic Regression (Baseline)
- Simple and interpretable model
- Used as a benchmark

### 2. Random Forest (Advanced Model)
- Captures nonlinear relationships
- Handles feature interactions automatically

---

## 📈 Evaluation Metrics

Model performance was evaluated using:
- Accuracy
- Confusion Matrix
- ROC-AUC

---

## 📊 Results

| Model | Accuracy | ROC-AUC |
|------|---------|--------|
| Logistic Regression | 0.810 | 0.883 |
| Random Forest | 0.821 | 0.887 |

👉 **Random Forest showed improved performance, indicating nonlinear relationships in the data.**

---

## 🔍 Feature Importance

The most important features identified by the Random Forest model:

- `Sex_male`
- `Fare`
- `Age`

These findings align with historical patterns, where:
- Gender played a major role in survival
- Socioeconomic status influenced access to resources
- Age affected survival likelihood

---

## 📂 Project Structure
```
Titanic-Survival-Prediction/
├── README.md
├── titanic_survival_prediction.ipynb
└── requirements.txt
```

---

## 🛠 Tools Used

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- Jupyter Notebook

---

## 🎯 Key Takeaways

- Random Forest improved classification performance over Logistic Regression
- Feature importance helped interpret model behavior
- The project demonstrates a full machine learning workflow:
  - Data cleaning
  - Feature engineering
  - Model training
  - Evaluation
  - Interpretation

---

## 🔮 Future Improvements

- Hyperparameter tuning
- Cross-validation
- Gradient boosting (XGBoost, LightGBM)
- SHAP-based model interpretation

---
