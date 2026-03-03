#  Air Quality Index (AQI) Prediction using Random Forest

##  Project Overview
Air pollution is a critical environmental and public health issue.  
This project builds a **Machine Learning regression model** to predict the **Air Quality Index (AQI)** using pollutant concentration data.

The model uses **Random Forest Regressor** and achieves extremely high predictive accuracy.

---

##  Objective
To develop a supervised regression model that predicts AQI values based on air pollutant concentrations and temporal features.

---

##  Dataset Information
- ~32,000+ records
- 15 original features
- Target Variable: **AQI**
- Key predictors:
  - PM2.5
  - PM10
  - NO2
  - SO2
  - CO
  - O3
  - Temporal features (year, month, day, season, weekday)

---

##  Project Workflow

1. Data Cleaning & Preprocessing  
2. Exploratory Data Analysis (EDA)  
3. Feature Selection  
4. One-Hot Encoding of categorical variables  
5. Train-Test Split (80-20)  
6. Random Forest Model Training  
7. Model Evaluation  
8. Feature Importance Analysis  
9. Hyperparameter Tuning using GridSearchCV  

---

##  Model Used
**RandomForestRegressor (Scikit-learn)**

Why Random Forest?
- Handles non-linear relationships
- Robust to outliers
- No need for feature scaling
- Provides feature importance

---

##  Model Performance

### Base Model:
- R² Score: ~0.99909
- RMSE: ~0.9489

### Tuned Model:
- R² Score: ~0.99911
- RMSE: ~0.9362

The high performance is due to the strong mathematical relationship between pollutant concentrations and AQI calculation.

---

##  Key Insights

- **PM2.5 contributes over 93%** to AQI prediction.
- PM10 is the second most influential pollutant.
- Temporal features have minimal direct impact.
- AQI is largely driven by particulate matter concentration.

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

##  Future Improvements

- Deploy model using Streamlit
- Compare with XGBoost and Gradient Boosting
- Time-series forecasting approach
- Real-time AQI dashboard integration

---

##  Learning Outcomes

- End-to-end ML pipeline implementation
- Handling categorical encoding properly
- Detecting and avoiding data leakage
- Hyperparameter tuning
- Interpreting feature importance
