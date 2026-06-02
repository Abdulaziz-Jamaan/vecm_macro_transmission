# vecm_macro_transmission

An empirical macroeconomic analysis framework utilizing a Structural Vector Error Correction Model (VECM) to investigate long-run equilibrium relationships and short-run dynamic transmission mechanisms within a multi-variable economic system.

## 📌 Project Overview
This repository contains the data, code, and post-estimation diagnostics for a **6-variable ($k=6$) VECM** anchored by a **single cointegrating vector ($r=1$)**. The primary objective is to map how structural shocks propagate through the macroeconomic system, measuring both the speed of adjustment and the multi-channel transmission effects over time.

## 🛠️ Methodology & Analytical Pipeline
The core analysis is executed within a unified Python pipeline (`vecm_macro_transmission.ipynb`) and covers:

1. **Unit Root Testing & Stationarity:** Checking integration properties using Augmented Dickey-Fuller (ADF) and Phillips-Perron (PP) tests.
2. **Cointegration Testing:** Utilizing the Johansen cointegration framework to establish the presence of a single long-run equilibrium relationship ($r=1$).
3. **Model Estimation:** Fitting the $k=6$ VECM to capture the system's asymmetric speed of adjustment.
4. **Post-Estimation Diagnostics:** Extensive statistical validation including:
   * Residual autocorrelation tests (Portmanteau/LM tests)
   * Normality tests (Jarque-Bera)
   * Structural stability analysis via Companion Matrix roots
5. **Shock Profiling:** Simulating macroeconomic policy shocks using **Orthogonalized Impulse Response Functions (OIRFs)** and Forecast Error Variance Decomposition (FEVD).

## 🗂️ Repository Structure
├── vecm_macro_transmission.ipynb   # Core Jupyter Notebook containing the full modeling pipeline
├── data/                            # Raw and transformed macroeconomic time-series data
├── outputs/                         # Exported plots (OIRFs, Companion Matrix plots) and diagnostic tables
└── README.md                        # Project documentation
