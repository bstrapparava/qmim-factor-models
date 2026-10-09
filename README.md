# Factor Models and Performance Measurement: Hedge Fund Strategy Indexes

Analysis for *Quantitative Methods in Investment Management* (Columbia University, Fall 2026).

The project evaluates nine Dow Jones Credit Suisse hedge fund strategy indexes over January 1994 to June 2012 (222 monthly observations), using the Fama-French and Carhart factors.

## What's inside

| File | Content |
|---|---|
| `bs3759_HW2.ipynb` | All code and outputs. Every table and figure in the report is computed here from the data. |
| `report/bs3759_HW2_report.pdf` | Written report with tables, charts and interpretation (8 pages). |
| `data/Performance_Measurement_Spreadsheet-1.xlsx` | Monthly returns: risk-free rate, Mkt-RF, SMB, HML, UMD, nine strategy indexes and the broad DJCS index. |
| `requirements.txt` | Python libraries needed. |

## Analysis

1. **Data audit:** sample period, frequency, missing values, decimal units.
2. **Outlier sensitivity:** Equity Market Neutral with and without November 2008 (−40.46%).
3. **Performance summary:** arithmetic and geometric returns, volatility, Sharpe ratio, maximum drawdown, skewness and excess kurtosis for each strategy.
4. **Benchmark-relative performance:** active return, tracking error and information ratio against the DJCS Hedge Fund Index.
5. **Path dependence:** Global Macro cumulative wealth, high-water mark and drawdown (peak, trough, recovery).
6. **Smoothing:** lag-one autocorrelation and why it makes √12 annualization understate risk.
7. **Factor attribution:** one-factor (CAPM) and four-factor (Carhart) regressions for Equity Long/Short, with alpha, confidence intervals, appraisal ratio and factor loadings.

## How to run

```bash
pip install -r requirements.txt
jupyter notebook bs3759_HW2.ipynb
```

Then run **Restart & Run All**. The notebook reads the data from `data/`.

In Google Colab, upload the notebook, create a `data` folder in the Files panel and upload the spreadsheet into it.
