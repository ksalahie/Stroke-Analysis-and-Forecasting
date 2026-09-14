[README.md](https://github.com/user-attachments/files/32196475/README.md)
# Statistical Analysis and Stroke Prediction

This project analyzes health and lifestyle data to evaluate the statistical probability of a stroke. We aim to identify key risk factors and model the likelihood of a stroke using patient characteristics.

## The Data

The dataset contains patient health records and lifestyle variables.
* **Source:** https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset
* **Target:** Stroke occurrence (Binary)
* **Variables:** Age, gender, hypertension, heart disease, average glucose level, BMI, smoking status, marital status, work type, and residence type.
* **Context:** Stroke is responsible for approximately 11% of global deaths. The dataset is imbalanced because stroke events are a statistical minority.

## Statistical Methods and Code Structure

The analysis focuses on understanding variable distributions and applying probability models:
* **Data Preprocessing:** Handling missing values, standardizing numerical variables, and encoding categorical data.
* **Sampling:** Balancing the target variable distribution using Random Undersampling and SMOTE to prevent bias.
* **Feature Selection:** Ranking the statistical importance of each variable to isolate the strongest predictors.
* **Probability Modeling:** Fitting Logistic Regression, XGBoost, LightGBM, and CatBoost algorithms to calculate stroke probabilities.
* **Ensemble Model:** Combining the outputs of multiple models via a voting classifier to improve statistical reliability.

## Results

The models are evaluated on their classification performance.

| Metric | Score |
|---|---|
| Accuracy | 0.8333 |
| Precision | 0.9608 |
| Recall | 0.7649 |
| F1-score | 0.8731 |
| ROC AUC score | 0.8719 |
| PR AUC score | 0.1856 |
| Kaggle Submission | 0.825 |

**Author:** Karim Salahie.
