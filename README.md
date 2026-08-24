# FINVEST

### Full-Stack Quantitative Trading, Portfolio Analytics & Risk Platform

FINVEST is a full-stack quantitative finance platform designed to simulate equity trading, analyze portfolio risk, rank stocks using multi-factor signals, and provide data-driven market insights.

The platform combines **quantitative screening, portfolio analytics, risk management, behavioral analysis, sentiment signals, and predictive modeling** into a unified trading environment.

---

## Key Features

### 📊 Multi-Factor Stock Ranking
- Ranks **Nifty 50 equities** using a multi-factor scoring framework.
- Combines **valuation, momentum, and market-cap signals**.
- Provides quantitative screening to identify relatively attractive equities.

### 📈 Quantitative Stock Screening
- Performs **exploratory data analysis (EDA)** on market and equity-level data.
- Supports Momentum-to-Valuation analysis for comparative stock assessment.
- Enables systematic filtering and ranking of securities.

### 💹 Trading Simulator
- Full-stack simulated trading environment for equity transactions.
- Supports **buy/sell workflows, order management, watchlists, and portfolio tracking**.
- Provides market dashboards for monitoring securities and positions.

### 🛡️ Portfolio Risk Analytics
- Implements **Value-at-Risk (VaR)** for portfolio risk estimation.
- Tracks portfolio exposure and risk-related metrics.
- Provides risk-management workflows alongside simulated trading.

### 🤖 Predictive Analytics
- Integrates **machine-learning-based stock forecasting** with trading workflows.
- Supports predictive market analysis for Nifty 50 equities.
- Connects model outputs with portfolio and trading decisions.

### 🧠 Sentiment & Behavioral Analytics
- Analyzes behavioral and sentiment signals alongside quantitative market factors.
- Provides additional context for equity and portfolio decisions.

### 📚 Financial Learning & Research
- Includes educational modules covering quantitative finance and systematic trading.
- Provides research-oriented insights into portfolio construction, risk, and market analysis.

---

## Technology Stack

### Frontend
- **Next.js / React**
- TypeScript
- Tailwind CSS
- Vite
- Charting & data-visualization components

### Backend
- **Go**
- REST APIs
- SQLite / database layer
- Authentication and portfolio services

### Quantitative & ML
- Python
- NumPy
- Pandas
- Scikit-learn
- Quantitative screening and predictive modeling

---

## Architecture

```text
                    ┌─────────────────────┐
                    │      FINVEST        │
                    │   Web Application   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Next.js / React   │
                    │   Trading Dashboard  │
                    └──────────┬──────────┘
                               │
                         REST API Layer
                               │
                               ▼
                    ┌─────────────────────┐
                    │      Go Backend     │
                    │ Portfolio & Trading │
                    └──────┬───────┬──────┘
                           │       │
              ┌────────────┘       └────────────┐
              ▼                                 ▼
     ┌─────────────────┐               ┌─────────────────┐
     │ Quant Analytics │               │  Risk Analytics │
     │ Stock Screening │               │      VaR        │
     └────────┬────────┘               └────────┬────────┘
              │                                 │
              └──────────────┬──────────────────┘
                             ▼
                    ┌─────────────────────┐
                    │ Predictive Analytics │
                    │  & Market Signals   │
                    └─────────────────────┘
