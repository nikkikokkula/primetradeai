# Primetrade Performance Analysis
## Trader Performance vs Market Sentiment

![Dashboard Preview](prime%20trade%20ai/charts/chart1_pnl_winrate_by_sentiment.png)

## Project Overview
This project analyzes how Bitcoin market sentiment (Fear vs Greed) affects trader behavior and trading performance. Using historical trading data and market sentiment indices, we identify patterns and propose actionable investment strategies.

## 🚀 Key Features
- **Sentiment Impact Analysis**: How market fear/greed correlates with profitability.
- **Trader Behavior Modeling**: Analysis of leverage, frequency, and bias under different market conditions.
- **Trader Segmentation**: Clustering traders into behavioral archetypes using KMeans.
- **Interactive Dashboard**: A Streamlit-based interface for exploring the data.

## 📊 Dataset Description
The analysis is based on two primary datasets:
1. **Bitcoin Market Sentiment**: Daily Fear & Greed Index values.
2. **Historical Trader Data**: Detailed logs of trader executions, including PnL, leverage, and timestamps. (Note: This repository contains a sampled version <25MB for optimal compatibility).

## 🛠️ Setup & Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/primetrade-assignment.git
   cd primetrade-assignment
   ```
2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Analysis**:
   Open the Jupyter notebook `primetrade_analysis.ipynb` and run all cells.

## 🧠 Methodology
1. **Data Integration**: Merged historical trading data with daily Bitcoin Fear & Greed Index values using a time-series alignment.
2. **Feature Engineering**: 
   - Calculated proxy leverage (Size USD / Start Position).
   - Classified trades into "Win/Loss" and "Long/Short".
   - Aggregated daily performance metrics per trader.
3. **Trader Segmentation**: Used behavioral metrics (frequency, leverage, consistency) to group traders.
4. **Sentiment Correlation**: Conducted comparative analysis of PnL and Win Rates across Fear, Neutral, and Greed market states.

## 📈 Key Insights & Strategies
- **Insight**: High-leverage traders suffer the most during "Fear" periods.
- **Strategy**: Reduce leverage exposure during Fear sentiment days to protect capital.
- **Insight**: Momentum-based traders excel during "Greed" periods.
- **Strategy**: Increase trading frequency for consistent traders during Greed sentiment to maximize momentum gains.

## 📁 Repository Structure
```
├── prime trade ai/
│   ├── fear_greed_index.csv    # Sentiment data
│   ├── historical_data.csv      # Trader execution logs
│   └── charts/                  # Generated visualizations
├── primetrade_analysis.ipynb    # Main analysis notebook
├── requirements.txt             # Python dependencies
├── .gitignore                  # Files to ignore in git
└── LICENSE                      # MIT License terms
```

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

