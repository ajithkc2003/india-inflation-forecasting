# Inflation Forecasting in India Using Time Series and Machine Learning

## Objective

This project aims to forecast India's Consumer Price Index (CPI) inflation by integrating classical time series techniques with modern machine learning approaches. The study investigates historical inflation patterns, identifies structural changes in inflation dynamics, and evaluates multiple forecasting models to generate a reliable inflation outlook for 2026.

A significant contribution of this project is the identification of a structural break in September 2016 following the adoption of India's Flexible Inflation Targeting (FIT) framework. By focusing on the post-2016 inflation regime and incorporating important macroeconomic indicators such as Wholesale Price Index (WPI), crude oil prices, and exchange rates, the project develops a forecasting framework that balances predictive accuracy with economic interpretability.

---

## Skills Learned

- Time Series Analysis and Forecasting
- ARIMA and ARIMAX Modeling
- Structural Break Detection and Regime Analysis
- Stationarity Testing using Augmented Dickey-Fuller (ADF) Test
- Feature Engineering for Time Series Data
- Seasonal Decomposition using STL
- Machine Learning for Economic Forecasting
- Support Vector Regression (SVR)
- Random Forest Regression
- Gradient Boosting (XGBoost)
- Model Evaluation using RMSE, MAE, R², and AIC
- Data Preprocessing and Transformation
- Economic Data Analysis and Interpretation
- Forecast Visualization and Comparative Analysis

---

## Tools Used

- **Python** for statistical analysis and machine learning implementation
- **Pandas** for data manipulation and time-series processing
- **NumPy** for numerical computation
- **Statsmodels** for ARIMA and ARIMAX modeling
- **Scikit-learn** for SVR, Random Forest, and Gradient Boosting models
- **Matplotlib** for visualization
- **Seaborn** for statistical graphics
- **SciPy** for statistical testing and diagnostics
- **Microsoft Excel (Power Query)** for data extraction, cleaning, and integration

---

## Project Workflow

### 1. Data Collection and Integration

Monthly macroeconomic data from January 2012 to December 2025 were collected from official and reliable sources.

#### Data Sources

- Consumer Price Index (CPI)
- Wholesale Price Index (WPI)
- Brent Crude Oil Prices
- INR/USD Exchange Rate

The datasets were cleaned, standardized, and merged into a unified time-series framework for analysis.

---

### 2. Exploratory Data Analysis (EDA)

Comprehensive exploratory analysis was performed to understand inflation behavior and identify relationships among variables.

#### Key Insights

- CPI inflation remained relatively stable with moderate variability.
- WPI exhibited higher volatility and occasional deflation periods.
- Crude oil prices showed the highest variability.
- Exchange rates displayed a gradual depreciation trend.
- Strong positive correlation between CPI and WPI.
- Significant influence of crude oil prices on wholesale inflation.

---

### 3. Data Preprocessing and Feature Engineering

To improve model performance and statistical validity, the following preprocessing techniques were applied:

- Logarithmic Transformation
- STL Seasonal Decomposition
- De-trending and Differencing
- Stationarity Testing using ADF Test
- Structural Break Analysis
- Forecast Recomposition to Original Scale

#### Structural Break Detection

A major structural break was identified in **September 2016**, corresponding to India's transition to the **Flexible Inflation Targeting (FIT)** regime. Modeling was therefore focused on the post-2016 period to improve forecasting accuracy.

---

### 4. Classical Time Series Modeling

#### ARIMA (2,0,2)

The ARIMA model was developed to capture inflation persistence and short-term fluctuations.

**Performance Metrics**

| Metric | Value |
|----------|----------|
| RMSE | 0.39 |
| MAE | 0.31 |
| R² | 0.91 |
| AIC | -412.6 |

---

#### ARIMAX (2,0,2)

The ARIMAX model extended ARIMA by incorporating key exogenous variables:

- Wholesale Price Index (WPI)
- Brent Crude Oil Prices
- Exchange Rate (INR/USD)

**Performance Metrics**

| Metric | Value |
|----------|----------|
| RMSE | 0.34 |
| MAE | 0.28 |
| R² | 0.94 |
| AIC | -438.2 |

The inclusion of external economic drivers significantly improved forecasting performance.

---

### 5. Machine Learning Modeling

Three machine learning algorithms were evaluated.

#### Support Vector Regression (SVR)

| Metric | Value |
|----------|----------|
| RMSE | 1.04 |
| R² | 0.88 |

- Best-performing machine learning model.
- Effectively captured non-linear inflation dynamics.

---

#### Random Forest Regression

| Metric | Value |
|----------|----------|
| RMSE | 1.43 |
| R² | 0.81 |

- Good predictive capability.
- Slight evidence of overfitting.

---

#### Gradient Boosting (XGBoost)

| Metric | Value |
|----------|----------|
| RMSE | 1.44 |
| R² | 0.79 |

- Captured complex relationships.
- Limited by relatively small dataset size.

---

### 6. Model Comparison and Validation

A comparative evaluation was conducted between econometric and machine learning models.

| Model | RMSE | R² |
|---------|---------|---------|
| ARIMA | 0.39 | 0.91 |
| ARIMAX | 0.34 | 0.94 |
| SVR | 1.04 | 0.88 |
| Random Forest | 1.43 | 0.81 |
| XGBoost | 1.44 | 0.79 |

#### Key Findings

- ARIMAX outperformed ARIMA due to exogenous variables.
- SVR was the strongest machine learning model.
- In-sample validation showed ARIMAX closely matched actual inflation values.
- ARIMAX was selected as the final forecasting model.

---

### 7. Inflation Forecasting for 2026

Using the ARIMAX (2,0,2) model, inflation forecasts were generated for the year 2026.

#### Forecast Highlights

- Expected Inflation Range: **2.1% – 3.1%**
- Inflation expected to remain within RBI's target tolerance band.
- Stable inflation environment under current economic conditions.
- Evidence of anchored inflation expectations under the FIT framework.

---

## Key Findings

- Structural break identified in September 2016.
- WPI and crude oil prices significantly influence CPI inflation.
- ARIMAX outperformed ARIMA across all evaluation metrics.
- SVR was the strongest machine learning model.
- ARIMAX provided the most reliable and economically meaningful forecasts.
- Inflation in 2026 is expected to remain stable and policy-consistent.

---

## Future Scope

Potential extensions of this work include:

- Incorporating interest rates and money supply variables.
- Using higher-frequency economic indicators.
- Applying deep learning architectures such as LSTM.
- Developing hybrid ARIMAX–Machine Learning models.
- Implementing real-time inflation forecasting systems.

---

## Conclusion

This project demonstrates how combining classical econometric techniques with modern machine learning approaches can improve inflation forecasting accuracy. While machine learning models captured complex non-linear patterns, the ARIMAX model achieved the best balance between predictive performance and economic interpretability. The resulting framework provides valuable insights for policymakers, researchers, and economic analysts seeking reliable inflation forecasts for India.
 ## Project Report
 ![Nmap Scan](https://github.com/ajithkc2003/india-inflation-forecasting/blob/main/Project_AJITH%20KC.pdf)
