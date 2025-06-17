# 🌳 Taxi Tip Amount Prediction using Decision Tree Regressor

This project builds a regression model using **Decision Tree Regressor** to predict the **tip amount** from NYC Taxi trip data based on multiple features.

---

## 📌 Objective
Predict the `tip_amount` for a taxi trip using variables like fare, tolls, distance, and more.

---

## 📊 Dataset Overview

Each row in the dataset represents a taxi trip with features including:
- **Fare amount**
- **Trip distance**
- **Tolls amount**
- **Payment type**
- **Vendor ID**
- And more...

The **target variable** is: `tip_amount`

---

## 🧠 Features Used

| Feature                | Type       | Description                          |
|------------------------|------------|--------------------------------------|
| fare_amount            | Numerical  | Fare charged for the trip            |
| tolls_amount           | Numerical  | Toll charges during the trip         |
| trip_distance          | Numerical  | Distance of the trip in miles        |
| ...                    | ...        | ...                                  |

Non-correlated features like `VendorID`, `store_and_fwd_flag`, etc. were removed for performance optimization.

---

## 🔧 Steps Performed

### 1. Data Preprocessing
- Checked for missing values
- Dropped features with low correlation

### 2. Exploratory Data Analysis
- Correlation plot with `tip_amount`

### 3. Modeling
- Used `DecisionTreeRegressor` from Scikit-learn
- `criterion='squared_error'`, `max_depth=8`

### 4. Optimization
- Removed unimportant features and tested impact on performance
- Tuned `max_depth` to improve R² and reduce MSE

---

## 📈 Evaluation Metrics

| Metric         | Value            |
|----------------|------------------|
| R² Score       | 0.89 (example)   |
| MSE            | 0.54 (example)   |

---

## 🧰 Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---
