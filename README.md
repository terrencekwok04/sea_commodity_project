# SE Asian Commodity Price Transmission & Singapore Food Security   

## What this project investigates   

Singapore imports more than 90% of its food, making domestic food prices sensitive to supply shocks originating in agricultural markets thousands of kilometres away. This project asks two questions:   

1. **What seasonal patterns drive prices in SE Asian physical commodity markets?**    How predictably do Vietnamese robusta coffee futures dip during harvest    season, and when does Malaysian palm oil production tighten during monsoon periods?

2. **How much of a commodity price shock reaches Singapore consumers?**    If global palm oil prices spike 10%, how much of that eventually shows up    in Singapore supermarket prices, and with how long a lag?

## Key Findings   

**Module 1 (Supply Dynamics):** STL seasonal decomposition of 10 years of monthly data reveals [your actual finding — e.g., 'a consistent USD 45/tonne seasonal trough in ICE Robusta coffee futures between October and January', driven by Vietnamese Central Highlands harvest export surges.]   

**Module 2 (Basis Analysis):** Cross-commodity correlation between coffee and palm oil is strongly positive during macro volatility regimes (2021–2022 commodity supercycle, r = [X]) but breaks down during commodity-specific supply events (2022 Indonesian palm oil export ban).   

**Module 3 (Import Concentration):** Singapore's poultry imports show HHI of approximately [X], reflecting near-monopoly dependence on Malaysia. The 2022 Malaysian chicken export ban — which caused actual supermarket shortages — is a direct empirical validation of this concentration risk. 

**Module 4 (CPI Pass-Through):** A 6-variable VAR model estimates that a 1% increase in global palm oil prices leads to a cumulative [X]% increase in Singapore oils & fats CPI over 12 months. Rice pass-through is lower ([X]%), consistent with Singapore's strategic stockpile buffering effect.   

## Data Sources   
| Source | Data | URL | 
|--------|------|-----| 
| ICE Futures Europe | Robusta Coffee front-month futures | Via Yahoo Finance (RC=F) |
| World Bank | Palm oil and rice monthly prices (Pink Sheet) | worldbank.org/en/research/commodity-markets |
| UN Comtrade | Vietnam coffee export volumes | comtrade.un.org | 
| MPOB | Malaysian palm oil supply/demand | bepi.mpob.gov.my | 
| SingStat | Singapore merchandise imports by country | singstat.gov.sg | 
| SingStat | Singapore food CPI sub-indices | singstat.gov.sg |   

## Technical Stack   
- **Python 3.11** with pandas, numpy, matplotlib, seaborn
- **Statsmodels** for STL seasonal decomposition and VAR modelling
- **yfinance** for futures price data retrieval
- **Jupyter Notebooks** for analysis and documentation

## How to Run   
1. Clone the repository: `git clone
https://github.com/YOUR_USERNAME/sea-commodity-analysis`
2. Install dependencies: `pip install -r requirements.txt`
3. Download raw data from the sources listed above and place in `data/raw/`
4. Run notebooks in order: module1 → module2 → module3 → module4

## Structure   
``` 
notebooks/ Jupyter notebooks, one per module 
data/processed/ Cleaned, analysis-ready datasets 
outputs/charts/ All generated visualisations (PNG, 150 DPI) 
outputs/policy_brief/  Final policy brief PDF 
```   
--- 
*Independent research project | Kwok Kit Leung, Terrence | NTU Economics & Data Science*
