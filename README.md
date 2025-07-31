# 📈 Yes Bank Stock Price Prediction (Regression Approach)
### 📌 Project Overview
This project focuses on predicting the monthly closing stock price of Yes Bank using regression techniques. The bank’s stock price has experienced significant volatility, particularly after the 2018 fraud case involving Rana Kapoor, making prediction an interesting and challenging problem.

The model utilizes historical open, high, low, and close prices to forecast the monthly closing price, implementing linear, Ridge, and Lasso Regression with hyperparameter tuning for optimal performance.

### 📊 Dataset
- **Source:** Historical stock price data of Yes Bank.
- **Features:** Date (converted to Month & Year for EDA)
  - Open Price
  - High Price
  - Low Price
  - Close Price (Target variable)

### 🛠 Tools & Libraries
- Pandas – Data cleaning & preprocessing
- NumPy – Numerical computations
- Matplotlib & Seaborn – Data visualization
- Scikit-learn – Model building, GridSearchCV, evaluation metrics

### ⚙️ Approach
**1. Data Preprocessing**
  - Converted Date column to datetime
  - Extracted Month and Year for analysis
  - Encoded Month using one-hot encoding (get_dummies)
  - Split the dataset into 80% training and 20% testing

**2. Model Building**
  - Linear Regression (Baseline model)
  - Ridge Regression with GridSearchCV (Hyperparameter tuning)
  - Lasso Regression with GridSearchCV (Hyperparameter tuning)

**3. Evaluation Metrics**
  - MSE, RMSE, MAE, MAPE
  - R² Score, Adjusted R²

### 📈 Key Results
- Linear Regression: RMSE = 13.24, R² = 0.9844, MAPE = 11.1%
- Ridge Regression (tuned): RMSE = 13.31, R² = 0.9842, MAPE = 11.1%
- Lasso Regression (tuned): RMSE = 13.19, R² = 0.9845, MAPE = 8.09%
- ✅ Best Model: Lasso Regression with GridSearchCV (lowest MAPE and slightly better interpretability).

### 💡 Business Impact
- Reduced average prediction error to 8%, improving accuracy of monthly forecasts.
- Helps analysts and investors make more risk-aware buy/sell decisions.
- Supports financial strategy planning by providing reliable trend predictions.
