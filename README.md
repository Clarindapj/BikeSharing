# Predicting Demand for Bike Sharing Projects

This repository hosts a machine learning project that focuses on the estimation of hourly bike rental expectations using regression techniques on a bike-sharing dataset. It attempts to assist the operators and planners of a city in ensuring better user satisfaction while making data-driven decisions on operational and strategic planning.  

---  

## Goals  

- Develop and assess the performance of a machine learning model capable of predicting the rentals value on an hourly basis.

- Design an interpretable model which can highlight the major drivers of the business for rental demand.

- Assist in attaining the precision needed on operational plans for bike sharing services.

---

## Tools Used  

**Software Engineering Tool**

- Python - The first language to address data processing, and machine learning activities.  

**Libraries & Frameworks**

- Pandas - Handling data and analysis procedures.

- NumPy - Scientific calculation associated tasks.

- Matplotlib & Seaborn - Presentation of analyzed data.

- Scikit-learn - Functions for data cleaning, sampling, and training the model on the data followed by evaluation.

- Jupyter Notebook - Exploratory data analysis markdown, and other project documentation.

---

## Project Structure

```
  
├── README.md                                                       < - Project Summary and Detailed Documentation 
  
├── Data
│   ├── bike_sharing_data.csv                                     < - Dataset
│   └── Bike Sharing Dataset.pdf                                   < - Description of the Dataset 
  
├── Model
│   ├── model_GradientBoosting.sav                                 < - Stored Gradient Boosting Model (Pickle) 
│   └── model_GradientBoosting.joblib                              < - Stored Gradient Boosting Model (Joblib) 
  
├── Notebook
│   └── Bike-Sharing.ipynb                                         < - Project's Primary Jupyter Notebook 
  
└── requirements.txt                                               < - Dependency List 
  
```
---

## Business Problem & Approach

With more than 700 stations and 5,400 bikes, managing Capital Bikeshare in Washington D.C. comes with its challenges. Precise demand forecasting aids in:

- Mitigating over congestion or under capacity at docking stations. 

- Improving user satisfaction through optimal bike usability. 

- Assisting planners and policymakers of the city in planning infrastructural frameworks.

###  Steps Taken:

1. **Collection & Understanding Data:**

   - Rentals on the hour, weather information, and time indicators.

2. **Cleaning & Preparing Data:**

   - Addressing missing data, eliminating leakage of data integrity, and creation of necessary features.

3. **Determination of Features:**
 
   - Important predictors: hour of the day, season, public holiday, meteorological situation, temperature, “feels like” temperature, and humidity.

4. **Partitioning for analysis:**
 
   - 80% for model training and the rest 20% for evaluation.

5. **Preprocessing** 

   - Standard scaling applied on numerical features while categorical variables underwent encoding.
  
6. **Construct and Assess Model:**
  
   - Linear Regression, Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting.

7. **Hyperparameter Tuning:**
  
   - Optimization with GridSearchCV and RandomizedSearchCV.
 
8. **Evaluation:**  
 
   - RMSE, MAE, MAPE, and R².

---  
## Model Evaluation Metrics  
- **RMSE (Root Mean Squared Error):**  

  Overall prediction error.

- **MAE (Mean Absolute Error):**  

  Average predictive errors incurred.  

- **MAPE (Mean Absolute Percentage Error):**  

  Return accuracy expressed as a percentage.

- **R2 (Coefficient of Determination):**  

  Measure of how much of the variance in the actual values can be attributed to the model. It ranges from 0—no explanatory power—to 1, indicating perfect fit. Higher R2 indicates greater explanatory power of the model on the outcome's variability.

---

## Model Results

| Model              | RMSE    | MAE    | R²      | MAPE    |

|--------------------|---------|--------|-------|---------|

| Linear Regression   | 109.60  | 79.11  | 0.615   | 2.42     |

| Ridge               | 109.60  | 79.07  | 0.615   | 2.41     |

| Lasso               | 114.32  | 83.40  | 0.581   | 2.39     |

| Decision Tree       | 137.21  | 88.83  | 0.396   | 1.08     |

| Random Forest       | 109.53  | 71.95  | 0.615   | 0.95     |

| Gradient Boosting   | 106.40  | 74.86  | 0.637   | 1.54     |

The **Gradient Boosting** model achieved the best performance with the lowest RMSE and highest R², suggesting that it explains approximately 64% of variance in the hourly rentals.

---

## Conclusion

- For this project, the Gradient Boosting model is considered the most optimal for predicting the rental demand of bikes on an hourly basis.

- Temperature, the time of day, and the season were observed to significantly influence demand.

- Precise estimates lead to improved operational strategies, increased user satisfaction, and optimized bike-share system management.

---

## Contant Me
- Name: Clarinda Puspitajati  
- E-mail: clarindapj@gmail.com  
- LinkedIn: [Clarinda's LinkedIn](https://www.linkedin.com/in/clarindapj/)
