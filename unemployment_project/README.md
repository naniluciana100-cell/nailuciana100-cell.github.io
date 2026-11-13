# U.S. Unemployment Forecasting by Age Group

## ECON 5371 – Time Series Analysis

### Project Overview
This project analyzes and forecasts U.S. unemployment rates for four age groups: 16–19, 20–24, 25–34, and 55 years and older.

Monthly unemployment data from the Federal Reserve Economic Data (FRED) database are analyzed using ARIMA time series models.

The project examines historical unemployment trends, tests for stationarity, compares ARIMA models, evaluates forecasting accuracy, and produces 12-month unemployment forecasts.

## Data Sources
Source: Federal Reserve Economic Data (FRED), using U.S. Bureau of Labor Statistics data.

- Ages 16–19: LNS14000012
- Ages 20–24: LNS14000036
- Ages 25–34: LNS14000089
- Ages 55+: LNS14024230

The analysis focuses on monthly unemployment data from 2000 through August 2026.

## Methods
The analysis uses:
- Summary statistics and time series plots
- ADF and KPSS stationarity tests
- ACF and PACF plots
- ARIMA model estimation and AIC comparison
- Forecast evaluation using MAE and RMSE
- Ljung–Box tests
- Twelve-month unemployment forecasts

## Selected ARIMA Models

| Age Group | ARIMA Model | AIC |
|---|---|---|
| 16–19 | (2,1,2) | 1130.106 |
| 20–24 | (1,1,1) | 997.013 |
| 25–34 | (0,1,1) | 650.958 |
| 55+ | (1,1,1) | 625.658 |

## Project Files
- `data/raw/`: Original unemployment datasets
- `data/clean/`: Cleaned unemployment dataset
- `code/`: Python analysis notebook
- `output/`: Forecast tables, model results, and graphs
- `Paper/`: Final research paper
- `Dashboard/`: Dashboard files

## How to Run the Analysis
1. Install Python and JupyterLab with the required libraries: pandas, numpy, matplotlib, scipy, and statsmodels.
2. Open `Unemployment_analysis_FINAL.ipynb` from the main project folder.
3. Ensure the four original CSV files are available in `data/`.
4. Select **Kernel → Restart Kernel and Run All Cells**.
5. Review the generated tables and graphs in `output/`.

## Reproducibility
The analysis uses relative paths within the project folder. The notebook generates model results, forecast tables, and figures from the unemployment data.

## AI Use Disclosure
AI assistance was used for coding guidance, fixing errors, and organizing project files. The analysis and results should be reviewed by teacher or student.