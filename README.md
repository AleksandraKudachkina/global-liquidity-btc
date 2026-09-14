# Does Global Liquidity Lead Bitcoin?

A macro-econometric study of the relationship between global liquidity conditions
and Bitcoin's future returns and downside risk.

## Research Question
Do changes in global liquidity contain predictive information about future
Bitcoin returns and downside risk? Which lag is most informative? Does the
relationship survive out-of-sample and after controlling for DXY, real yields,
and risk appetite?

## Structure
- `data/` — raw and processed data (raw data not tracked in git, see data_loader.py)
- `notebooks/` — step-by-step analysis
- `src/` — reusable functions (data loading, liquidity index, stats tests, regimes, backtest)
- `report/` — final write-up

## Methodology
1. Data collection (BTC, Fed/ECB balance sheets, M2, DXY, real yields, VIX, Nasdaq)
2. Global Liquidity Index construction (Net Liquidity + PCA factor)
3. Stationarity testing (ADF) and transformations
4. Cross-correlation lag analysis
5. Lagged regressions with macro controls (HAC standard errors)
6. Granger causality (with caveats)
7. Rolling regression (stability over time)
8. Out-of-sample walk-forward validation
9. Liquidity Regime Score + simple backtest

## Status
🚧 Work in progress

## License
MIT
