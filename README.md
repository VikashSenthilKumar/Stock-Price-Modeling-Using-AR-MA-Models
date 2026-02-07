# Stock Price Modeling Using AR & MA Models

## Project Overview
This project focuses on modeling short-term stock price behavior using classic time series analysis techniques: Autoregressive (AR) and Moving Average (MA) models. The objective is to understand temporal dependencies in financial data and build reliable forecasting models.

The project involves preprocessing non-stationary price data, identifying optimal model parameters using ACF and PACF plots, fitting models using `statsmodels`, evaluating performance, and exporting the trained model for production use.

## System Requirements
* **Python 3.x**
* **Pandas** (Data manipulation)
* **Statsmodels** (Time series analysis)
* **Matplotlib** (Visualization)
* **Scikit-learn** (Metrics)

## Project Structure
* `Stock_Modeling.ipynb`: Jupyter notebook containing the full data pipeline, analysis, modeling, and evaluation.
* `stock_ar_model.pkl`: Serialized model file ready for production deployment.

## Installation & Usage
1.  Clone this repository.
2.  Install required libraries:
    ```bash
    pip install pandas statsmodels matplotlib scikit-learn
    ```
3.  Run the `Stock_Modeling.ipynb` notebook to reproduce the results.

## Model Details
* **Data Transformation**: Raw stock prices were converted to returns using differencing to achieve stationarity, verified by the Augmented Dickey-Fuller (ADF) test.
* **Lag Selection**: ACF/PACF plots were utilized to determine orders $p$ and $q$.
* **Evaluation**: Models were compared based on AIC, BIC, and residual analysis.

## Exported Model
The best-performing model is exported as `Stock_Price_Modelling .pkl`. This file can be loaded in a production environment using `pickle` to generate forecasts.

## 🚀 How to Use
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/VikashSenthilKumar/Stock-Price-Modeling-Using-AR-MA-Models.git]
