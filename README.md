# SABR stochastic volatility model in practice

Code for my MSc thesis at the Barcelona School of Economics (Finance Program), *SABR: A stochastic
volatility model in practice*.

The notebook `MP_cleancode.ipynb`:
1. **Calibrates the SABR model** maturity by maturity with non-linear least squares, using Hagan's
   implied-volatility formula (β = 1).
2. **Rebuilds volatility smiles and the implied-volatility surface**, with a single parameter set and with
   maturity-specific parameters, and studies how the smile moves when the forward price changes.
3. **Prices options by conditional Monte Carlo** (Willard's formula) and recovers the implied-volatility
   surface from the simulated prices.
4. **Compares Hagan's formula and conditional Monte Carlo** against the market surface (mean squared error
   and computing time).

**Data:** the notebook reads market option data from `data.xlsx`, which is not included in this repository.

**Stack:** Python (NumPy, pandas, SciPy, Matplotlib).
