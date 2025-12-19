# Student Sleep Patterns Analysis

## Overview
This project analyzes the relationship between **age** and various lifestyle factors (screen time, sleep duration, caffeine intake, study hours, and physical activity) among students. The analysis uses **linear regression**, **k-nearest neighbors (KNN)**, and **logistic regression** to model and predict these relationships.

---

## Dataset
- **Source:** `student_sleep_patterns.csv`
- **Features:**
  - `Age`
  - `Screen_Time`
  - `Sleep_Duration`
  - `Caffeine_Intake`
  - `Study_Hours`
  - `Physical_Activity`

---

## Analysis & Models

### 1. Linear Regression
Predicts the following dependent variables using `Age` as the independent variable:
- **Screen Time**
- **Sleep Duration**
- **Caffeine Intake**
- **Study Hours**
- **Physical Activity**

**Metrics:**
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)
- Mean Absolute Percentage Error (MAPE)

### 2. K-Nearest Neighbors (KNN)
- Predicts `Sleep_Duration` based on `Age` (normalized).
- Uses `k=5` neighbors.

### 3. Logistic Regression
- Classifies `Screen_Time` as **High** or **Low** (based on median) using `Age`.
- Outputs accuracy and classification report.

---

## Visualizations
- Scatter plots with regression lines for each linear model.
- Actual vs. predicted plots for KNN and logistic regression.

---

## How to Run
1. Ensure you have the required libraries:
   ```bash
   pip install pandas numpy scikit-learn matplotlib
   ```
2. Place `student_sleep_patterns.csv` in your working directory.
3. Run the script.

---

## Key Findings
- **Age vs. Screen Time:** [Brief insight, e.g., "Screen time tends to decrease with age."]
- **Age vs. Sleep Duration:** [Brief insight]
- **Age vs. Caffeine Intake:** [Brief insight]
- **Age vs. Study Hours:** [Brief insight]
- **Age vs. Physical Activity:** [Brief insight]

---

## Future Work
- Explore multivariate regression with more features.
- Experiment with other classification algorithms.
- Collect more data for robust modeling.

---

## License
[Specify if applicable, e.g., MIT, GPL, etc.]

