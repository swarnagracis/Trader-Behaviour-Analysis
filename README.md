# Trader Sentiment & Behavioral Performance Analysis

## Project Overview

This project analyzes the relationship between market sentiment (Fear/Greed Index) and trader behavior using trade-level data.

The objectives were to:
- Examine how sentiment impacts trading behavior and profitability
- Segment traders based on exposure, activity, and consistency
- Build a predictive model for next-day profitability

---

## Methodology

### 1. Data Processing
- Aggregated trade-level data into daily trader metrics
- Engineered behavioral features:
  - Daily PnL
  - Win rate
  - Trade count
  - Long ratio
- Merged market sentiment classification (Extreme Fear → Extreme Greed)

### 2. Statistical Analysis
- Compared performance across sentiment regimes
- Conducted ANOVA tests for significance
- Evaluated behavioral shifts under different market conditions

### 3. Trader Segmentation
Traders were segmented into:
- High vs Low Exposure
- Frequent vs Infrequent Activity
- Consistent vs Inconsistent Performance

### 4. Predictive Modeling
- Built a Logistic Regression model
- Target: Next-day profitability (binary)
- Features: Sentiment + behavioral metrics
- Model Accuracy: ~69%

---

## Key Insights

- Sentiment significantly impacts trading behavior (p < 0.001).
- Performance differences across sentiment regimes were not statistically significant.
- Frequent traders outperform infrequent traders.
- Consistent traders show more stable profitability.
- Same-day win rate strongly predicts next-day profitability.

---

## Outputs

The repository includes:
- Notebook with full analysis
- Output charts (in `/outputs`)
- Model performance tables
- Confusion matrix visualization

---

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/trader-sentiment-analysis.git
cd trader-sentiment-analysis
```

### 2. Create virtual environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate     # Mac/Linux
venv\Scripts\activate        # Windows
```

### 3. Install dependencies

```bash
pip install pandas numpy matplotlib scikit-learn scipy
```

## How to Run

```bash
jupyter notebook notebooks/sentiment_trader_analysis.ipynb
```
