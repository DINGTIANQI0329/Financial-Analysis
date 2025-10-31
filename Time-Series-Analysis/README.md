# Volatility Clustering and Crude Oil Time Series Analysis

## 📊 Project Overview

This project aims to conduct an in-depth time series analysis of daily price data for **WTI Crude Oil** and **Brent Crude Oil**.

The core objective of the analysis is to **identify and study the phenomenon of "volatility clustering"**—the tendency for asset prices to experience periods of high volatility followed by periods of low volatility.

The project unfolds through three phases of analysis reports:
1.  Basic Statistical Properties
2.  Time Series Modeling
3.  Volatility Clustering Analysis

---

## 🗃️ Project File Structure

. ├── 📄 01_statistics.pdf ├── 📄 02_time_series_models.pdf ├── 📄 03_volatility_clustering.pdf ├── 💾 RBRTEd.csv ├── 💾 RWTCd.csv └── README.md

### Data Sources (Data)

* `RWTCd.csv`: Contains daily ("d") price data for **West Texas Intermediate (WTI) Crude Oil**.
* `RBRTEd.csv`: Contains daily ("d") price data for **Brent Crude Oil**.

### Analysis Reports

* `01_statistics.pdf`:
    * **Phase 1: Descriptive Statistics and Empirical Properties**
    * Contents may include: visualization of price and return series, analysis of mean, median, standard deviation, skewness, and kurtosis, stationarity tests (e.g., ADF test), and autocorrelation analysis (ACF/PACF plots).

* `02_time_series_models.pdf`:
    * **Phase 2: Classical Time Series Modeling**
    * Contents may include: application of AR, MA, ARMA, or ARIMA models to fit the price or return data. This section aims to establish a baseline before volatility modeling (Phase 3).

* `03_volatility_clustering.pdf`:
    * **Phase 3: Volatility Clustering Analysis**
    * This is the core of the project. Contents may include:
        * Identifying evidence of volatility clustering (e.g., autocorrelation of squared returns).
        * Applying GARCH (Generalized Autoregressive Conditional Heteroskedasticity) family models to capture time-varying volatility.
        * Using clustering algorithms (like K-Means or Markov Switching Models) to identify different volatility regimes (high-volatility vs. low-volatility periods).

---

## 📈 Analysis Workflow

This project follows a standard financial econometrics workflow:

1.  **Data Preparation**: Load `RWTCd.csv` and `RBRTEd.csv` data, perform data cleaning, and calculate log returns (which are typically stationary and suitable for modeling).
2.  **Statistical Analysis (see `01_statistics.pdf`)**: Examine the stylized facts of the return series, such as heavy tails (high kurtosis) and volatility clustering.
3.  **Mean Modeling (see `02_time_series_models.pdf`)**: Establish a mean equation (e.g., ARMA model) for the return series and obtain the residuals.
4.  **Volatility Modeling (see `03_volatility_clustering.pdf`)**: Apply models like GARCH to the residuals (or original returns) to model volatility.
5.  **Clustering Analysis (see `03_volatility_clustering.pdf`)**: Use machine learning clustering methods based on volatility features to classify market regimes.

---

## 🛠️ (Placeholder) How to Run

*This project requires corresponding Python or R scripts to reproduce the reports.*

### Dependencies

* Python 3.x
* pandas
* numpy
* matplotlib / seaborn
* statsmodels (for ARIMA, GARCH)
* scikit-learn (for clustering)

### Running the Analysis

1.  (Placeholder) Install dependencies:
    ```bash
    pip install pandas numpy matplotlib statsmodels scikit-learn
    ```
2.  (Placeholder) Run the analysis script:
    ```bash
    python run_analysis.py
    ```
