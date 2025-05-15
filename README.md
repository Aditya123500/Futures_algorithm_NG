Natural Gas Futures Trading Strategy

Overview

This repository contains a backtesting framework for trading Natural Gas futures (NG1 & NG2) using a systematic strategy. It leverages market regime detection, technical indicators, fundamental data, and advanced risk management to optimize trade execution while dynamically switching between contracts.

Key Features





Dynamic Contract Switching: Seamlessly transitions between NG1 and NG2 to avoid expiration issues, leveraging their high correlation (0.995).



Market Regime Detection: Uses CUSUM with V-Mask to identify trending or mean-reverting conditions.



Signal Generation:





Technical Indicators: EMA, SMA, MACD, Volatility, Jerk, Velocity.



Fundamental Data: COT reports, storage levels (BCF), weather data (HDD/CDD).



Noise Filtering: Fractal Dimension Indicator (FDI) avoids chaotic market conditions.



Risk Management:





Stop-Loss (3%) and Take-Profit (6%) to control risk.



Kelly Criterion for dynamic position sizing (12-trade window).



Margin checks (10% initial, 8% maintenance) to prevent liquidation.



Performance Metrics: Tracks Sharpe Ratio, Sortino Ratio, Max Drawdown, and more.

Performance Metrics







Metric



Value





Total Trades



256





Winning Trades



112





Win Rate (%)



43.75





Profit Percentage (%)



273.99





Sharpe Ratio



1.79





Sortino Ratio



0.77





Max Drawdown



$88,138.00





Max Drawdown (%)



38.19





Final Balance



$186,996.00

Key Takeaways:





Strong profitability with a 273.99% return on $50,000 initial capital.



Moderate risk-adjusted returns (Sharpe: 1.79, Sortino: 0.77).



Drawdown (38.19%) indicates room for risk optimization.

Hypotheses





High Correlation: NG1 and NG2 move nearly identically (0.995 correlation), enabling smooth rollovers.



Signal Continuity: Trading signals remain valid across contract switches.



Noise Filtering: FDI improves trade quality by avoiding erratic market conditions.
