# Machine Learning Assignment I

This repository contains the implementation and analysis of two selected tasks for Machine Learning Assignment I.

## Selected Tasks

### Task 1 – Regression Analysis: CO₂ Emission Prediction

The objective of this task is to develop a regression model to predict vehicle CO₂ emissions based on vehicle characteristics and fuel consumption parameters.

**Domain:** Environmental Science and Machine Learning

**Model Used:** Multiple Linear Regression

**Target Variable:** CO2 Emissions (g/km)

#### Features Used

- Engine Size (L)
- Cylinders
- Fuel Consumption City (L/100 km)
- Fuel Consumption Hwy (L/100 km)
- Fuel Consumption Comb (L/100 km)
- Fuel Consumption Comb (mpg)

#### EDA Performed

- Dataset structure and information analysis
- Missing value analysis
- Duplicate value analysis
- Descriptive statistical analysis
- CO₂ emissions distribution analysis
- Correlation analysis
- Correlation heatmap
- Engine Size vs CO₂ Emissions
- Cylinders vs CO₂ Emissions
- Fuel Consumption vs CO₂ Emissions
- Actual vs Predicted CO₂ Emissions
- Residual analysis

#### Model Evaluation

| Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | 12.1021 |
| Mean Squared Error (MSE) | 368.3229 |
| Root Mean Squared Error (RMSE) | 19.1917 |
| R² Score | 0.8979 |

The model achieved an R² score of approximately **89.79%**, indicating that the selected features explain a substantial proportion of the variation in vehicle CO₂ emissions.

---

## Task 5 – Logistic Regression: Bank Customer Churn Prediction

The objective of this task is to develop a classification model to predict whether a bank customer will churn based on demographic, financial, and account-related characteristics.

**Domain:** Banking and Financial Services

**Model Used:** Logistic Regression

**Target Variable:** Churn

- `0` – Customer retained
- `1` – Customer churned

#### Features Used

- Credit Score
- Country
- Gender
- Age
- Tenure
- Balance
- Products Number
- Credit Card
- Active Member
- Estimated Salary

The `customer_id` variable is excluded from model training because it is an identifier rather than a predictive feature.

#### EDA Performed

- Dataset structure and information analysis
- Missing value analysis
- Duplicate value analysis
- Descriptive statistical analysis
- Customer churn distribution
- Churn percentage analysis
- Churn by gender
- Churn by country
- Age distribution by churn
- Balance distribution by churn
- Active member vs churn
- Number of products vs churn
- Numerical correlation analysis
- Correlation heatmap

#### Data Preprocessing

- Removed identifier variable from modelling
- Encoded categorical variables
- Applied feature scaling
- Divided the dataset into training and testing sets
- Used stratified train-test splitting

#### Model Evaluation

The Logistic Regression model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix
- ROC Curve

### Task 5 Results

The final evaluation values are available in the `Bank_Churn_Logistic_Regression.ipynb` notebook.

| Metric | Result |
|---|---:|
| Accuracy | Refer to notebook |
| Precision | Refer to notebook |
| Recall | Refer to notebook |
| F1 Score | Refer to notebook |
| ROC-AUC | Refer to notebook |

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# Repository Structure

```text
ML-Assignment-1/
│
├── Task_1_CO2_Regression/
│   │
│   ├── dataset/
│   │   └── CO2 Emissions_Canada.csv
│   │
│   └── notebook/
│       ├── CO2_Regression.ipynb
│       └── .gitkeep
│
├── Task_5_Bank_Churn/
│   │
│   ├── dataset/
│   │   └── Bank Customer Churn Prediction.csv
│   │
│   └── notebook/
│       ├── Bank_Churn_Logistic_Regression.ipynb
│       └── .gitkeep
│
├── README.md
└── requirements.txt
