# Titanic Survival Prediction

## Project Overview
This project predicts passenger survival on the Titanic using machine learning models. The goal was to build a simple end-to-end classification pipeline, compare a baseline model with a more advanced model, and interpret the most important predictors of survival.

## Dataset
The dataset used in this project is the Titanic dataset, which contains passenger-level information such as age, sex, ticket class, fare, and survival outcome.

Target variable:
- `Survived` (0 = did not survive, 1 = survived)

## Data Preprocessing
The following preprocessing steps were performed:
- Removed irrelevant columns: `Name`, `Ticket`, `Cabin`, and `PassengerId`
- Filled missing values in `Age` using the median
- Filled missing values in `Embarked` using the mode
- Converted categorical variables into numeric variables using one-hot encoding

## Methods
Two classification models were built and compared:
1. Logistic Regression
2. Random Forest Classifier

The dataset was split into training and test sets using an 80/20 split.

## Evaluation Metrics
Model performance was evaluated using:
- Accuracy
- Confusion Matrix
- ROC-AUC

## Results

### Logistic Regression
- Accuracy: 0.810
- ROC-AUC: 0.883

### Random Forest
- Accuracy: 0.821
- ROC-AUC: 0.887

## Key Findings
- Random Forest performed slightly better than Logistic Regression.
- The most important features in the Random Forest model were:
  - `Sex_male`
  - `Fare`
  - `Age`
- These findings are consistent with historical patterns, where gender, socioeconomic status, and age influenced survival outcomes.

## Tools Used
- Python
- pandas
- NumPy
- scikit-learn
- matplotlib

## Project Takeaway
This project demonstrates a complete machine learning workflow, including data cleaning, feature engineering, model training, model evaluation, and interpretation.

## Future Improvements
Possible next steps include:
- Hyperparameter tuning
- Cross-validation
- Trying gradient boosting methods such as XGBoost
- Using SHAP values for more detailed model interpretation
