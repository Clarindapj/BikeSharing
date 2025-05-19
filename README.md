# Bike Sharing Demand Prediction Project

This repository contains a machine learning project focused on predicting hourly bike rental demand for a bike-sharing platform using regression algorithms. The aim is to help operators and city planners optimize bike distribution, improve user satisfaction, and support data-driven operational decisions.

---

## Objectives

- Build a machine learning model to accurately predict the number of bikes rented per hour.
- Develop an interpretable model to identify key factors influencing bike rental demand.
- Support efficient and effective operational planning for bike-sharing services.

---

## Technologies Used

**Programming Language**
- Python - The primary language for data processing and machine learning.

**Libraries & Frameworks**
- Pandas - Data manipulation and analysis.
- NumPy - Numerical computations.
- Matplotlib & Seaborn - Data visualization.
- Scikit-learn - Data preprocessing, splitting, model training, and evaluation.
- Jupyter Notebook - Interactive data exploration and project documentation.

---

## Project Structure

```
├── README.md                         <- Project overview and documentation
├── Data
│   ├── bike_sharing_data.csv         <- Dataset
│   └── Bike Sharing Dataset.pdf      <- Dataset description
├── Model
│   ├── model_GradientBoosting.sav    <- Saved Gradient Boosting model (Pickle)
│   └── model_GradientBoosting.joblib <- Saved Gradient Boosting model (Joblib)
├── Notebook
│   └── Bike-Sharing.ipynb            <- Main Jupyter Notebook for the project
└── requirements.txt                  <- List of dependencies
```

---

## Business Problem & Approach

Capital Bikeshare operates over 700 stations and 5,400 bikes in Washington D.C. Accurate demand prediction is crucial for:
- Preventing overfilling or underfilling at stations.
- Enhancing user experience by ensuring bike availability.
- Supporting city planners in infrastructure decisions.

### Steps Taken:
1. **Data Collection & Understanding:**  
   - Hourly data on rentals, weather, and temporal features.
2. **Data Cleaning & Preparation:**  
   - Handling missing values, removing data leakage risks, and feature engineering.
3. **Feature Selection:**  
   - Key predictors: hour, season, holiday, weather situation, temperature, “feels like” temperature, and humidity.
4. **Data Splitting:**  
   - 80% for training, 20% for testing.
5. **Preprocessing:**  
   - Scaling numerical features; encoding categorical features.
6. **Model Building & Selection:**  
   - Linear Regression, Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting.
7. **Hyperparameter Tuning:**  
   - GridSearchCV and RandomizedSearchCV for optimization.
8. **Evaluation:**  
   - Metrics: RMSE, MAE, MAPE, R².

---

## Model Evaluation Metrics

- **RMSE (Root Mean Squared Error):**  
  Overall error in prediction made.

- **MAE (Mean Absolute Error):**  
  Errors that are made on average.

- **MAPE (Mean Absolute Percentage Error):**  
  Accuracy as a percentage return.

- **R2 (Coefficient of Determination):**  
  Proportion of variance in the actual values that is explained by the model; ranges from 0 (no explanatory power) to 1 (perfect fit). Higher R2 means the model better explains the variability in the outcome.

---

## Model Results

| Model              | RMSE    | MAE    | R²      | MAPE    |
|--------------------|---------|--------|---------|---------|
| Linear Regression  | 109.60  | 79.11  | 0.615   | 2.42    |
| Ridge              | 109.60  | 79.07  | 0.615   | 2.41    |
| Lasso              | 114.32  | 83.40  | 0.581   | 2.39    |
| Decision Tree      | 137.21  | 88.83  | 0.396   | 1.08    |
| Random Forest      | 109.53  | 71.95  | 0.615   | 0.95    |
| Gradient Boosting  | 106.40  | 74.86  | 0.637   | 1.54    |

The **Gradient Boosting** model achieved the best performance, with the lowest RMSE and highest R², indicating it explains about 64% of the variance in hourly bike rentals.

---

## Conclusion

- The Gradient Boosting model is the most effective for predicting hourly bike rental demand in this project.
- Key factors influencing demand include temperature, hour of the day, and season.
- Accurate predictions enable better operational planning, improved user satisfaction, and more efficient bike-sharing management.
