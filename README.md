# SPY Implied Volatility Surface Analysis

A comprehensive quantitative analysis of SPY (S&P 500 ETF) options volatility surface using the Black-Scholes model and numerical methods.

##  Project Overview

This project implements a complete volatility surface analysis pipeline, from data extraction to interactive 3D visualization. It demonstrates advanced quantitative finance techniques applicable to options pricing, risk management, and trading strategies.

##  Key Features

- **Real-Time Data Extraction**: Automated download of SPY options data via Yahoo Finance API
- **Black-Scholes Pricing**: Implementation of the classic option pricing model
- **Implied Volatility Calculation**: Robust computation using Brent's root-finding method
- **Volatility Smile Analysis**: Examination of volatility patterns across strikes for multiple maturities (30, 60, 90 days)
- **Interactive 3D Surface**: Plotly-based visualization allowing exploration of the complete volatility structure
- **Greeks Computation**: Delta, Gamma, Vega, and Theta sensitivities for risk management

## Main Results

### Volatility Smile Evolution
The analysis reveals that the volatility smile **flattens progressively** as maturity increases, consistent with:
- Mean reversion in volatility
- Risk dilution over longer time horizons
- Market microstructure dynamics

### Greeks Patterns
- **Delta**: Smooth transition from 0 (OTM) to 1 (ITM)
- **Gamma**: Peak at ATM, indicating maximum hedging requirements
- **Vega**: Highest for ATM options, crucial for volatility trading
- **Theta**: Most negative at ATM, representing time decay

##  Technologies

- **Python 3.14**
- **Data & Computation**: `yfinance`, `pandas`, `numpy`, `scipy`
- **Visualization**: `matplotlib`, `plotly`
- **Financial Models**: Black-Scholes, Brent's optimization method

##  Project Structure

```
 Volatility_Professional.ipynb    # Main analysis notebook
 README.md                         # Project documentation
```

##  Getting Started

### Prerequisites
```bash
pip install yfinance pandas numpy scipy matplotlib plotly jupyter
```

### Running the Analysis
```bash
jupyter notebook Volatility_Professional.ipynb
```

##  Methodology

1. **Data Collection**: Extract SPY options data for 3 maturities (30, 60, 90 days)
2. **Filtering**: Keep only liquid options (volume > 0) within ±10% of ATM
3. **IV Calculation**: Use Brent's method to solve for implied volatility
4. **Visualization**: Generate volatility smiles and 3D surface
5. **Greeks Analysis**: Compute and visualize option sensitivities

##  Applications

This analysis is directly relevant to:
- **Options Pricing**: Consistent valuation across all strikes and maturities
- **Risk Management**: Greeks-based hedging and VaR calculation
- **Trading Strategies**: Volatility arbitrage and skew trading
- **Market Analysis**: Sentiment extraction from volatility patterns

##  Key Concepts

- **Volatility Smile**: Pattern where implied volatility varies with strike price
- **Volatility Surface**: 3D representation of IV across strike and maturity
- **Greeks**: Option price sensitivities (Delta, Gamma, Vega, Theta)
- **Brent's Method**: Robust root-finding algorithm for IV calculation

##  Author

**Louison Robert**  
Master 1 Finance, Université Paris-Saclay

##  Contact

[louison-robert@outlook.com]

## License

This project is available for educational and professional purposes.

---

⭐ If you find this project useful, please consider giving it a star on GitHub!
