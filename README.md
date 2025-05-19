Here is your cleaned and corrected Markdown document, with special attention paid to the formatting and alignment of the **Model Results** table, general grammar, consistent terminology, and overall Markdown structure.

---

# Predicting Demand for Bike Sharing Projects

This repository hosts a machine learning project focused on estimating hourly bike rental demand using regression techniques on a bike-sharing dataset. The goal is to assist city operators and planners in improving user satisfaction through data-driven decisions for operational and strategic planning.

---

## Goals

* Develop and assess a machine learning model capable of predicting rental demand on an hourly basis.
* Design an interpretable model that highlights key drivers influencing rental demand.
* Assist in achieving the precision required for operational planning of bike-sharing services.

---

## Tools Used

### Software Engineering Tool

* **Python** – Primary language for data processing and machine learning tasks.

### Libraries & Frameworks

* **Pandas** – Data handling and analysis.
* **NumPy** – Scientific computations.
* **Matplotlib & Seaborn** – Data visualization.
* **Scikit-learn** – Data preprocessing, model training, and evaluation.
* **Jupyter Notebook** – Exploratory data analysis and project documentation.

---

## Project Structure

```
├── README.md                             <- Project summary and documentation
├── Data
│   ├── bike_sharing_data.csv             <- Dataset
│   └── Bike Sharing Dataset.pdf          <- Dataset description
├── Model
│   ├── model_GradientBoosting.sav        <- Pickle model
│   └── model_GradientBoosting.joblib     <- Joblib model
├── Notebook
│   └── Bike-Sharing.ipynb                <- Main Jupyter notebook
└── requirements.txt                      <- Dependencies list
```

---

## Business Problem & Approach

Managing Capital Bikeshare in Washington D.C. with over 700 stations and 5,400 bikes presents challenges. Accurate demand forecasting helps:

* Prevent over-congestion or under-capacity at docking stations.
* Improve user satisfaction through optimal bike availability.
* Support policymakers in infrastructure planning.

### Steps Taken

1. **Data Collection & Understanding**

   * Hourly rentals, weather data, and time-based indicators.

2. **Data Cleaning & Preparation**

   * Handling missing data, preventing leakage, and creating features.

3. **Feature Engineering**

   * Key predictors: hour, season, holidays, weather, temperature, “feels like” temperature, and humidity.

4. **Data Splitting**

   * 80% for training, 20% for evaluation.

5. **Preprocessing**

   * Standard scaling for numerical features and encoding for categorical variables.

6. **Modeling**

   * Algorithms used: Linear Regression, Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting.

7. **Hyperparameter Tuning**

   * GridSearchCV and RandomizedSearchCV.

8. **Evaluation**

   * Metrics: RMSE, MAE, MAPE, R².

---

## Model Evaluation Metrics

* **RMSE (Root Mean Squared Error):** Measures overall prediction error.
* **MAE (Mean Absolute Error):** Average of absolute prediction errors.
* **MAPE (Mean Absolute Percentage Error):** Accuracy expressed as a percentage.
* **R² (Coefficient of Determination):** Indicates model’s explanatory power (0 to 1).

---

## Model Results

| Model             | RMSE   | MAE   | R²    | MAPE |
| ----------------- | ------ | ----- | ----- | ---- |
| Linear Regression | 109.60 | 79.11 | 0.615 | 2.42 |
| Ridge             | 109.60 | 79.07 | 0.615 | 2.41 |
| Lasso             | 114.32 | 83.40 | 0.581 | 2.39 |
| Decision Tree     | 137.21 | 88.83 | 0.396 | 1.08 |
| Random Forest     | 109.53 | 71.95 | 0.615 | 0.95 |
| Gradient Boosting | 106.40 | 74.86 | 0.637 | 1.54 |

The **Gradient Boosting** model delivered the best performance, with the lowest RMSE and the highest R², indicating it explains approximately 64% of the variance in hourly rentals.

---

## Conclusion

* **Gradient Boosting** was the most effective model for predicting hourly bike rental demand.
* Key influencing factors included temperature, time of day, and season.
* Accurate demand forecasting enables better operations, enhances user experience, and optimizes resource management.

---

## Contact Me

* **Name:** Clarinda Puspitajati
* **Email:** [clarindapj@gmail.com](mailto:clarindapj@gmail.com)
* **LinkedIn:** [Clarinda's LinkedIn](https://www.linkedin.com/in/clarindapj/)
