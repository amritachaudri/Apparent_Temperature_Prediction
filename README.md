# Apparent Temperature Prediction

This repository demonstrates a **machine learning pipeline** for predicting *Apparent Temperature* using historical weather data. The project is designed as a learning exercise to explore relationships between meteorological variables and build predictive models.

## Key Questions Addressed
- Is there a relationship between **humidity** and **temperature**?
- What about between **humidity** and **apparent temperature**?
- Can we **predict apparent temperature** using regression models?

## Dataset Overview
The dataset contains **5,999 records** with **12 attributes** and no missing values.

### Features:
- **Target Variable:** `Apparent Temperature (C)`
- **Predictors:** `Temperature (C)`, `Humidity`, `Wind Speed (km/h)`, `Wind Bearing (degrees)`, `Visibility (km)`, `Pressure (millibars)`, `Precip Type`

### Cleaning & Preparation:
- Dropped irrelevant fields: `Loud Cover` (constant zero) and `Daily Summary` (textual).
- Outliers in `Humidity` handled using **Interquartile Range (IQR)**.
- Encoded categorical variables like `Precip Type`.

## Exploratory Findings
- Strong positive correlation between **Temperature** and **Apparent Temperature**.
- Moderate negative correlation between **Humidity** and **Apparent Temperature**.
- No significant multicollinearity among predictors.

---

## Tech Stack
- **Data Wrangling:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Modeling:** `scikit-learn` (`LinearRegression`)

Install dependencies:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
