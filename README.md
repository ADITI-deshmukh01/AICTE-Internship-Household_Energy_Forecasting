# AICTE Internship – Household Energy Forecasting

## Introduction
This project is developed as part of the **AICTE Edunet Foundation Internship (Aug–Sep 2025)** under the theme **Sustainable Energy & Efficiency**.  
The goal is to analyze and forecast household energy consumption using real-world electricity usage data and apply machine learning techniques for prediction.

Energy efficiency is one of the most important challenges for a sustainable future. By understanding consumption patterns, households and policymakers can make informed decisions to reduce wastage and improve sustainability.

---

## Objectives
- Explore household energy usage data and identify key patterns.
- Perform data preprocessing and cleaning to prepare the dataset for ML models.
- Build a machine learning model to forecast energy consumption.
- Evaluate model performance using standard regression metrics.
- Document insights and future directions for advanced forecasting.

---

## Dataset
The dataset used is the **Household Power Consumption Dataset** from UCI/Kaggle.  
It contains electric power consumption measurements from a single household over almost 4 years (December 2006 – November 2010).

📂 Source: [Kaggle - Household Power Consumption Dataset](https://www.kaggle.com/datasets)

### Dataset Description
| Column | Description |
|--------|-------------|
| Date   | Date of measurement (dd/mm/yyyy) |
| Time   | Time of measurement (hh:mm:ss) |
| Global_active_power | Household global active power (kilowatts) |
| Global_reactive_power | Household global reactive power (kilowatts) |
| Voltage | Average voltage (volts) |
| Global_intensity | Average current intensity (ampere) |
| Sub_metering_1 | Energy sub-metering 1 (kitchen appliances) |
| Sub_metering_2 | Energy sub-metering 2 (laundry room appliances) |
| Sub_metering_3 | Energy sub-metering 3 (heating & cooling) |

---

## Workflow

### Week 1 – Data Preparation
- Imported dataset using Pandas.
- Combined **Date + Time** into a single datetime column.
- Handled missing values and cleaned the dataset.
- Selected features (inputs) and target (output).
- Split the dataset into training and testing sets.

### Week 2 – Machine Learning Model
- Selected **Linear Regression** as baseline ML model.
- Trained model using input features (Voltage, Global Intensity, Sub-metering values, etc.).
- Predicted target variable (**Global Active Power**).
- Evaluated performance using **MAE, RMSE, and R² score**.
- Documented results and observations.

---

## Implementation

### Libraries Used
- **Python 3**
- **Pandas, NumPy** → Data handling
- **Matplotlib, Seaborn** → Visualization
- **Scikit-learn** → Machine learning (Linear Regression, metrics)

### Example Code Snippet
```python
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import numpy as np

# Train/Test Split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Train Model
model = LinearRegression()
model.fit(X_train, y_train)

# Predict
y_pred = model.predict(X_test)

# Evaluate
mae = mean_absolute_error(y_test, y_pred)
rmse = np.sqrt(mean_squared_error(y_test, y_pred))
r2 = r2_score(y_test, y_pred)
```

---

## Results & Observations
- ✅ The model successfully predicted household energy usage trends.  
- ✅ Daily consumption shows clear **morning and evening peaks**.  
- ✅ Weekends may show slightly different patterns compared to weekdays.  
- ⚠️ Accuracy is limited since weather and seasonal data are not yet integrated.  

**Evaluation Metrics (example):**
- MAE: *X.XX*  
- RMSE: *X.XX*  
- R² Score: *0.XX*  

---

## Future Work
- Apply advanced ML forecasting models (**ARIMA, LSTM, Random Forest, XGBoost**).
- Compare **weekdays vs weekends** consumption patterns.
- Integrate **weather data** (temperature, sunlight hours) for better correlation.
- Extend project to **real-time energy monitoring dashboards**.

---

## Conclusion
This project demonstrates how household energy data can be analyzed and used for forecasting.  
Accurate predictions can help improve energy efficiency, reduce wastage, and support sustainable living practices.

---
