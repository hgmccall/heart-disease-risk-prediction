# heart-disease-risk-prediction
Machine learning project that predicts the likelihood of heart disease using patient health metrics and classification models including Logistic Regression, Random Forest, and XGBoost.
# Heart Disease Prediction Using Machine Learning

A machine learning project that predicts the presence of heart disease using patient health indicators and compares classification model performance.

---

## Overview

This project explores the use of machine learning techniques to predict whether a patient has heart disease based on medical and demographic information.

Using a heart disease dataset containing patient health metrics such as age, cholesterol levels, blood pressure, chest pain type, and exercise-induced angina, multiple classification models were trained and evaluated to determine their effectiveness in identifying heart disease.

The project demonstrates data preprocessing, classification modeling, model evaluation, and data visualization using Python and Scikit-learn.

---

## Objectives

The primary goals of this project were to:

- Predict the presence of heart disease using machine learning
- Prepare medical data for classification analysis
- Train and evaluate multiple classification models
- Compare model performance using standard evaluation metrics
- Identify factors associated with heart disease
- Visualize patterns within the dataset

---

## Dataset

Heart Disease Prediction Dataset

The dataset contains patient medical information, including:

- Age
- Sex
- Chest Pain Type
- Blood Pressure (BP)
- Cholesterol
- Fasting Blood Sugar
- EKG Results
- Maximum Heart Rate
- Exercise-Induced Angina
- ST Depression
- Number of Major Vessels
- Thallium Test Results

Target Variable:

- Heart Disease
 - Presence (1)
 - Absence (0)

---

## Data Cleaning & Preparation

Several preprocessing steps were performed before training the machine learning models.

### Target Variable Encoding

The target variable was converted from categorical labels to numerical values:

- Presence → 1
- Absence → 0

This allowed machine learning algorithms to process the data.

### Missing Value Validation

The dataset was examined for missing values.

Result:
- No missing values were identified.

### Feature Standardization

Column names were standardized by replacing spaces with underscores to improve compatibility with machine learning workflows.

Example:

- "Heart Disease" → "Heart_Disease"

---

## Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Machine Learning Models

- Decision Tree Classifier
- Logistic Regression
- Random Forest (Feature Importance Analysis)

### Development Environment

- Jupyter Notebook

---

## Methodology

### Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

This allowed model performance to be evaluated on unseen data.

### Decision Tree Classification

A Decision Tree Classifier was trained using all available predictor variables.

The model learned patterns in patient characteristics to classify whether heart disease was present or absent.

### Logistic Regression

A Logistic Regression model was trained and evaluated as an alternative classification approach.

Performance metrics were compared against the Decision Tree model.

### Feature Importance Analysis

Random Forest feature importance scores were used to identify the variables that contributed most strongly to heart disease prediction.

---

## Model Performance

### Decision Tree

Test Accuracy:

68.5%

Confusion Matrix:

```
[[22 11]
 [ 6 15]]
```

The Decision Tree successfully identified many heart disease cases but produced a larger number of incorrect predictions compared to Logistic Regression.

---

### Logistic Regression

Test Accuracy:

92.6%

Classification Report:

- Precision: 0.95
- Recall: 0.86
- F1 Score: 0.90

The Logistic Regression model significantly outperformed the Decision Tree model and provided the highest predictive performance.

---

## Visualizations

Several visualizations were created to better understand the data and model performance.

### Heart Disease Distribution

A count plot was used to examine the number of patients with and without heart disease.

### Cholesterol vs Heart Disease

A box plot was used to compare cholesterol levels between patients diagnosed with heart disease and those without the condition.

### Confusion Matrix

A heatmap visualized model predictions versus actual outcomes, making classification performance easier to interpret.

### Chest Pain Type vs Heart Disease

A count plot was used to investigate the relationship between chest pain categories and heart disease prevalence.

### Decision Tree Visualization

A graphical representation of the trained Decision Tree model provided insight into the decision-making process used for classification.

### Feature Importance

A Random Forest feature importance chart highlighted the variables most influential in predicting heart disease.

---

## Key Findings

### Logistic Regression Performed Best

The Logistic Regression model achieved approximately 92.6% accuracy, significantly outperforming the Decision Tree model.

### Certain Medical Indicators Were Strong Predictors

Variables such as chest pain type, maximum heart rate, ST depression, and vessel count appeared to play important roles in classification.

### Machine Learning Can Effectively Predict Heart Disease

The results demonstrate that patient health measurements can be used to accurately identify individuals at risk for heart disease.

### Visualization Improved Interpretability

The confusion matrix, box plots, and feature importance analysis helped explain both the data patterns and model behavior.

---

## Future Improvements

Potential enhancements include:

- Hyperparameter tuning to improve model performance
- Cross-validation for more robust evaluation
- Additional classification algorithms such as Support Vector Machines
- Feature selection techniques
- Interactive dashboards for model exploration
- Predictive web application deployment

---

## Author

Hailey McCall

LinkedIn: www.linkedin.com/in/hailey-mccall

GitHub: https://github.com/haileymccall

From <edge://commercial-copilot-chat/> 

