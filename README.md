# Stroke Prediction and Apple Quality Analysis
## Overview
This repository contains an exploratory data analysis (EDA) and predictive modeling project focused on two datasets:

**Stroke Prediction Dataset**: Analyzes factors influencing stroke likelihood, with a focus on glucose levels.

**Apple Quality Dataset**: Predicts apple quality (good or bad) using machine learning models.

The project includes statistical tests, data visualizations, and machine learning models (linear regression and logistic regression) to derive insights and predictions.

---
## Datasets
1. Stroke Prediction Dataset
- Source: Kaggle
- Description: Contains demographic, lifestyle, and medical information to predict stroke likelihood.
- Key Features:
  - avg_glucose_level: Average glucose level in blood.
  - stroke: Binary target variable (1 = stroke, 0 = no stroke).
- Objective: Determine if patients who had a stroke have higher average glucose levels than those who did not.

2. Apple Quality Dataset
- Source: locally sourced Apple_Quality.csv dataset
- Description: Contains features like size, weight, sweetness, crunchiness, juiciness, ripeness, and acidity to predict apple quality.
- Key Features:
  - Quality: Target variable (good or bad).
- Objective: Predict apple quality using machine learning models.

## Project Structure
```
/ML-intro
├── data/
│   ├── healthcare-dataset-stroke-data.csv
│   └── Apple_Quality.csv
├── ML_notebook.ipynb
└── README.md
```

---
## Key Analyses
### Stroke Prediction Analysis
Statistical Tests:
- Shapiro-Wilk Test: Checked for normality in glucose levels.
- Levene’s Test: Assessed equal variance between stroke and non-stroke groups.
- Mann-Whitney U-Test: Compared glucose levels between stroke and non-stroke patients.

Findings:
- Stroke patients have significantly higher average glucose levels (p-value < 0.05).
- Weak correlation between glucose levels and stroke likelihood.

### Apple Quality Analysis
Machine Learning Models:
- Linear Regression: Identified ripeness as the best predictor of apple quality (weak correlation).
- Logistic Regression: Achieved 75% accuracy in predicting apple quality.
- Confusion Matrix:
  - Balanced performance in classifying good and bad apples.
  - Misclassification rates: 98 false positives and 99 false negatives.
 
---
## Results
### Stroke Prediction
Conclusion: Higher glucose levels are associated with an increased likelihood of stroke.<br>
Implications: Monitoring glucose levels could be crucial for stroke prevention.

### Apple Quality
Conclusion: Logistic regression outperformed linear regression for binary classification.<br>
Implications: Ripeness is a key factor, but combining multiple features could improve predictions.

---
## Future Work
### Stroke Prediction:
- Explore additional features (e.g., age, hypertension) to improve predictions.
- Use logistic regression or other classification models for stroke prediction.

### Apple Quality:
- Experiment with advanced models like Random Forests or Support Vector Machines.
- Address class imbalance (if present) using resampling techniques.

---
## Acknowledgments
- Stroke Prediction Dataset: Credit to [Fedesoriano](https://www.kaggle.com/fedesoriano) on Kaggle.
- Apple Quality Dataset: Credit to my University Professor.

---
## License
This project is licensed under the MIT License. See the [LICENSE](https://github.com/Reignu/ML-intro/blob/main/LICENSE) file for details.

