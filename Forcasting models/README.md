# 📈 Forecasting Models — Interactive Course

A single-file, self-contained interactive course covering the full spectrum of forecasting methods — from classical econometrics to machine learning and production pipelines. Open `forecast.html` in any modern browser and the entire course runs locally with no server, no installation, and no internet required after the initial CDN load.

---

## 🚀 Quick Start

```bash
git clone https://github.com/your-username/forecasting-models.git
cd forecasting-models
# Then just open the file:
open forecast.html          # macOS
start forecast.html         # Windows
xdg-open forecast.html      # Linux
```

Or open it directly in Chrome / Firefox by double-clicking `forecast.html`.

---

## 📚 Course Structure

| Module | Topics | Lessons |
|--------|--------|---------|
| **1 · Foundations** | Time series concepts, stationarity, ACF/PACF, decomposition | 4 + quiz |
| **2 · Classical Econometrics** | AR, MA, ARMA, ARIMA, SARIMA, ARIMAX, AIC/BIC, ADF/KPSS | 4 + quiz |
| **3 · Multivariate & Macro** | VAR, VECM, cointegration, Johansen test, IRF, DSGE overview | 3 + quiz |
| **4 · Machine Learning** | Random Forest, XGBoost/GBM, LSTM/RNN, feature engineering | 3 + quiz |
| **5 · Advanced Topics** | Prophet, state space models, Kalman filter, ensemble forecasting, DM test | 4 + quiz |
| **6 · Practical Workflow** | Data preparation, time series CV, backtesting, production pipelines | 3 + quiz |

**28 lessons · 18 quiz questions · 17 interactive simulations**

---

## ✨ Features

### 🎛️ Interactive Simulations
Every major model has a real-time parameter explorer built with Plotly.js. Drag sliders and watch the process update instantly — no page reloads.

- AR/MA coefficient tuner with live ACF/PACF plots
- ARIMA differencing & forecasting visualizer
- SARIMA seasonal period explorer
- VAR bivariate system simulator
- Impulse Response Function animator
- Kalman Filter Q/R noise ratio demo
- Prophet changepoint & seasonality simulator
- Walk-Forward CV fold visualizer
- Gradient Boosting iteration convergence plotter
- LSTM lookback window & horizon explorer
- … and more

### 🐍 In-Browser Python (Pyodide)
Every lesson includes a runnable Python code block. Click **▶ Run** and the code executes directly in your browser via [Pyodide](https://pyodide.org/) — no local Python installation needed.

- Powered by Pyodide v0.25 (NumPy, micropip pre-loaded)
- Editable textarea — modify code and re-run instantly
- Output captured and displayed inline
- Graceful fallback messaging if Pyodide is unavailable

> **First run:** Pyodide downloads ~10 MB from CDN and takes ~20 seconds to initialise. Subsequent runs in the same session are instant.

### 📊 R Code Blocks
Clean, production-quality R examples for every model using canonical packages:

| Package | Used for |
|---------|----------|
| `forecast` | ARIMA, ETS, auto.arima, tsCV |
| `vars` | VAR, VECM, IRF, FEVD |
| `urca` | Johansen cointegration, ADF |
| `tseries` | ADF, KPSS, unit root tests |
| `KFAS` / `dlm` | State space, Kalman filter |
| `prophet` | Meta's Prophet model |
| `ranger` / `xgboost` | ML models for time series |
| `keras` | LSTM networks |

One-click **Copy** button on every code block.

### 📐 Mathematical Formulations
Every model includes its full mathematical specification rendered with [MathJax](https://www.mathjax.org/) — AR lag polynomials, Kalman gain equations, VECM error-correction terms, XGBoost regularised objective, and more.

### 📝 Quizzes & Progress Tracking
- 3 multiple-choice questions at the end of each module
- Instant feedback highlighting correct / incorrect answers
- Sidebar progress bar tracking visited lessons across all 28 lessons

---

## 🏗️ Technical Stack

| Library | Version | Purpose |
|---------|---------|---------|
| [Plotly.js](https://plotly.com/javascript/) | 2.27.0 | Interactive charts & simulations |
| [Pyodide](https://pyodide.org/) | 0.25.0 | In-browser Python runtime |
| [MathJax](https://www.mathjax.org/) | 3 | LaTeX equation rendering |
| [Prism.js](https://prismjs.com/) | 1.29.0 | Syntax highlighting (Python + R) |

All loaded from CDN. Zero npm, zero build step, zero dependencies to install.

---

## 📖 Topics Covered in Depth

### Foundations
- Weak vs. strict stationarity; mean, variance, autocovariance
- Additive vs. multiplicative decomposition
- White noise, random walk, AR(1) properties
- ADF, KPSS, Phillips-Perron unit root tests
- Sample ACF/PACF and the Box-Jenkins model identification table
- STL decomposition; X-13ARIMA-SEATS seasonal adjustment

### Classical Econometrics
- AR(p), MA(q), ARMA(p,q) — lag polynomial notation, invertibility
- ARIMA(p,d,q) — Wold decomposition, Box-Jenkins workflow
- SARIMA(p,d,q)(P,D,Q)ₛ — airline model, seasonal identification
- ARIMAX — exogenous regressors, transfer function approach
- AIC, BIC, HQIC — derivation and comparison
- Auto-ARIMA grid search implementation

### Multivariate & Macro
- VAR(p) — reduced form, stability conditions, curse of dimensionality
- Structural VAR — Cholesky identification, sign restrictions
- Johansen trace and max-eigenvalue cointegration tests
- VECM — α (speed of adjustment), β (cointegrating vectors), Granger representation theorem
- Impulse Response Functions with bootstrap confidence bands
- Forecast Error Variance Decomposition (FEVD)
- New Keynesian DSGE — IS curve, Phillips curve, Taylor rule

### Machine Learning
- Lag features, rolling statistics, Fourier terms, calendar encoding
- Random Forest for regression — OOB error, feature importance
- XGBoost — second-order gradients, regularised objective, early stopping
- LightGBM/CatBoost mentions
- LSTM gate equations (forget, input, cell, output)
- Sequence-to-sequence architecture, lookback window design
- Dropout regularisation, MinMax scaling, inverse transform

### Advanced Topics
- Prophet — piecewise linear/logistic trend, Fourier seasonality, holiday effects
- State space models — general linear Gaussian framework
- Kalman filter — prediction/update equations, steady-state gain
- Extended Kalman Filter (EKF), Unscented KF, particle filters (overview)
- Ensemble methods — equal weight, Bates-Granger optimal weights, stacking
- MAE, RMSE, MAPE, sMAPE, MASE — properties and use cases
- Diebold-Mariano test — HAC variance, sequential testing

### Practical Workflow
- LOCF, seasonal, and Kalman imputation — causal vs. non-causal
- IQR and STL-based outlier detection; winsorisation
- Box-Cox transformation — Guerrero method for λ selection
- Walk-forward (expanding) vs. rolling-window cross-validation
- `TimeSeriesSplit` in scikit-learn; `tsCV` in R forecast
- Conformal prediction intervals — calibration residuals, marginal coverage guarantee
- Production pipeline class — ingestion → validation → features → fit → serve → monitor

---

## 🖥️ Browser Compatibility

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Full support |
| Firefox 90+ | ✅ Full support |
| Edge 90+ | ✅ Full support |
| Safari 15+ | ✅ Full support |
| Mobile browsers | ✅ Responsive layout |

---

## 📁 File Structure

```
forecasting-models/
└── forecast.html      # The entire course — HTML + CSS + JS inline (237 KB)
└── README.md
```

Everything is intentionally kept in a single file for maximum portability — share it via email, USB, or GitHub and it works anywhere.

---

## 🤝 Contributing

Contributions welcome! Ideas for extensions:

- Additional modules: GARCH/volatility models, Bayesian forecasting, N-BEATS/N-HiTS neural architectures
- WebR integration for true in-browser R execution
- More Pyodide examples using `statsmodels` and `scikit-learn` (requires additional package loading)
- Dark mode toggle
- Export quiz results to PDF

Please open an issue before submitting a large PR.

---

## 📄 License

MIT License — free to use, modify, and distribute for personal or commercial purposes. See [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgements

- [Box & Jenkins (1976)](https://www.wiley.com/en-us/Time+Series+Analysis%3A+Forecasting+and+Control-p-9780470272283) — the original ARIMA methodology
- [Taylor & Letham (2018)](https://doi.org/10.1080/00031305.2017.1380080) — Prophet: Forecasting at Scale
- [Hyndman & Athanasopoulos — *Forecasting: Principles and Practice*](https://otexts.com/fpp3/) — the definitive open-access textbook
- [Diebold & Mariano (1995)](https://doi.org/10.1080/07350015.1995.10524599) — comparing predictive accuracy
- The [Pyodide](https://pyodide.org/), [Plotly](https://plotly.com/), and [MathJax](https://www.mathjax.org/) teams for making browser-based data science possible
