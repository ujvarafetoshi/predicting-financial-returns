# Financial Returns Analysis Project

## Overview
This project involves the analysis of daily financial returns of Hermes and BlackRock from the year 2000 to 2024. The objective is to predict future returns and manage a dynamic portfolio for investing in these assets using Autoregressive (AR) and ARMA models.

## Dataset
The dataset contains the daily returns of BlackRock and Hermes companies spanning over 24 years. The data includes three columns: Date, BLK returns, and Hermes returns.

## Libraries Used
- `numpy`: For mathematical operations
- `pandas`: For data manipulation and analysis
- `matplotlib.pyplot`: For plotting graphs
- `statsmodels`: For statistical models, including AR and ARMA models
- `scipy.stats`: For statistical functions

## Methodology
1. **Data Preparation**: The dataset is loaded, and preliminary data exploration is performed to understand its structure and characteristics.
2. **Stationarity Check**: Visual inspection and statistical tests are conducted to check the stationarity of the time series.
3. **Modeling**:
   - Autocorrelation and partial autocorrelation plots are generated to identify the order of AR models.
   - AR and ARMA models are fitted to the returns to predict future values.
   - The Box-Pierce test is used to check for autocorrelation in residuals.
4. **Dynamic Portfolio Management**: 
   - The minimum variance portfolio is computed using the covariance matrix of the asset returns.
   - Time-varying variances are predicted using ARMA models for both Hermes and BlackRock returns to adjust the portfolio dynamically.

## Key Insights
Since financial returns have time-varying volatility, and when there is high volatility, future returns are expected to be highly volatile, or conversely, low volatility follows low volatility, we focused on squared demeaned returns. This approach acknowledges that the series are autocorrelated, enhancing our model's relevance and accuracy in predicting future returns.

## Results
- The project successfully predicts future returns using AR and ARMA models.
- A dynamic portfolio management strategy is developed that utilizes the predicted time-varying variances of Hermes and BlackRock returns.

## Conclusion
The analysis provides insights into the financial returns of Hermes and BlackRock, demonstrating the potential of AR and ARMA models in predicting returns and managing investment portfolios dynamically.
