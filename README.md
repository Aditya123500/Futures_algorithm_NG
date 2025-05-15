# 📈 Natural Gas Futures Trading Strategy

A comprehensive backtesting framework for trading **Natural Gas Futures (NG1 & NG2)** using a systematic, data-driven approach. This strategy combines **market regime detection**, **technical and fundamental indicators**, and **advanced risk management** to optimize performance and ensure continuity across futures contracts.

---

## 🔍 Overview

This system is built to simulate real-world trading conditions and includes:

- **Dynamic Contract Switching**: Seamlessly switches between **NG1** (front month) and **NG2** (next month) to manage expiries, leveraging their high correlation (**0.995**).
- **Market Regime Detection**: Uses **CUSUM with V-Mask** to identify trending vs. mean-reverting conditions.
- **Signal Generation**:
  - **Technical Indicators**: EMA, SMA, MACD, Volatility, Jerk, Velocity
  - **Fundamental Inputs**: COT reports, storage levels (BCF), weather data (HDD/CDD)
  - **Noise Filtering**: **Fractal Dimension Indicator (FDI)** to avoid chaotic market regimes
- **Risk Management**:
  - Stop-Loss (**3%**) and Take-Profit (**6%**) limits
  - **Kelly Criterion** for dynamic lot sizing (rolling 12-trade window)
  - **Margin Check Logic**: 10% initial & 8% maintenance margin enforcement
- **Performance Metrics**:
  - Sharpe Ratio, Sortino Ratio, Max Drawdown, Win Rate, Profitability, etc.

---

## 📊 Strategy Performance

| **Metric**               | **Value**         |
|--------------------------|-------------------|
| Total Trades             | 256               |
| Winning Trades           | 112               |
| Win Rate (%)             | 43.75%            |
| Profit Percentage (%)    | 273.99%           |
| Sharpe Ratio             | 1.79              |
| Max Drawdown ($)         | $88,138.00        |
| Max Drawdown (%)         | 38.19%            |
| Final Balance ($)        | $186,996.00       |

---

## 🔑 Key Takeaways

- ✅ **Strong Profitability**: +273.99% return on $50,000 initial capital  
- ⚖️ **Moderate Risk-Adjusted Returns**: Sharpe 1.79 
---

## 🧠 Hypotheses & Insights

- **High Correlation**: NG1 and NG2 futures exhibit 0.995 correlation → smooth rollover behavior
- **Signal Continuity**: Core signals remain valid across NG1/NG2 switchovers
- **Noise Filtering**: FDI improves quality by avoiding high-volatility, random-like market states

---

## 👨‍💻 Author

**Aditya Arya**  
Indian Institute of Technology Jodhpur  
Core Member, Quant Club

---



