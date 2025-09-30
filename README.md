#  Food Delivery Time Estimation

##  Project Overview
This project aims to estimate the **delivery time of food orders** using machine learning techniques.  
The dataset contains details about delivery persons, customer locations, restaurant info, traffic conditions, festivals, and other factors that influence delivery time.  

The main objective is to **predict the time taken (in minutes)** for each order.

---

##  Dataset Information
- **File Used:** `train.csv`  
- **Key Features:**
  - Delivery person’s age & ratings
  - Vehicle condition
  - Multiple deliveries assigned
  - Distance between restaurant & customer
  - Traffic conditions
  - Festival effect
  - Weekday vs Weekend

- **Target Variable:** `Time_taken(min)`

---

##  Steps Followed

### 1. Data Understanding
- Loaded dataset using **Pandas**.
- Explored structure, data types, and shape.
- Checked missing values & duplicates.

### 2. Data Cleaning
- Handled missing values.
- Removed/treated outliers.
- Converted categorical features into numeric.

### 3. Feature Engineering
- Created new features:
  - `Distance_km` → distance between restaurant & customer
  - `Prep_time(min)` → order preparation time
  - `Is_Weekend` → weekend flag
  - `Time_per_km` → efficiency of delivery time
- Encoded categorical variables.

### 4. Exploratory Data Analysis (EDA)
- Distribution plots for age, ratings, and delivery time.
- Relationship between traffic, festivals, and delivery time.
- Correlation heatmap of features.
- Weekday vs Weekend comparison.

### 5. Model Building
Trained multiple machine learning models:
- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Gradient Boosting Regressor  

### 6. Model Evaluation
- Metrics used:
  - R² Score
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
- Compared models and selected best performer (Random Forest / Gradient Boosting performed best).

### 7. Final Prediction
- Predicted `Time_taken(min)` for new/unseen data.
- Visualized **Actual vs Predicted values**.

---

##  Results & Insights
- Distance & weekend effect are strong predictors of delivery time.
- Random Forest & Gradient Boosting models outperformed Linear Regression.
- Feature engineering significantly improved accuracy.

---

##  Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  

---

##  Conclusion
This project successfully demonstrates how machine learning can be applied to **predict real-world delivery times**, helping food delivery companies improve operations and customer satisfaction.

---
