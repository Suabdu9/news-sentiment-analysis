# News Sentiment Analysis and Stock Price Prediction

## Project Overview

This project analyzes the relationship between financial news sentiment and stock market movement using exploratory data analysis, technical indicators, and natural language processing techniques.

The workflow combines financial news headlines with historical stock price data to investigate whether news sentiment has a measurable relationship with daily stock returns.

The project was completed as part of the KAIM Week 1 Challenge.

---

# Business Objective

Financial markets are heavily influenced by information flow, investor perception, and breaking news. This project aims to explore whether sentiment extracted from financial news headlines can help explain stock price movement.

The analysis focuses on:

- Exploring financial news publishing patterns
- Analyzing stock price behavior using technical indicators
- Measuring sentiment from financial news headlines
- Quantifying the relationship between sentiment and stock returns

The project demonstrates how NLP-based sentiment analysis and quantitative financial analysis can be integrated for market intelligence research.

---

# Project Structure

```text
news-sentiment-analysis/
├── .github/
│   └── workflows/
│       └── unittests.yml
├── data/
│   └── raw/
│       ├── financeData/
│       └── newsData/
├── notebooks/
│   ├── task_1_eda.ipynb
│   ├── AAPL_analysis.ipynb
│   ├── AMZN_analysis.ipynb
│   ├── GOOG_analysis.ipynb
│   ├── META_analysis.ipynb
│   ├── NVDA_analysis.ipynb
│   ├── AAPL_sentiment_analysis.ipynb
│   ├── AMZN_sentiment_analysis.ipynb
│   ├── GOOG_sentiment_analysis.ipynb
│   ├── META_sentiment_analysis.ipynb
│   └── NVDA_sentiment_analysis.ipynb
├── scripts/
├── src/
├── tests/
├── requirements.txt
├── README.md
└── .gitignore

# Tasks Completed

## Task 1 — Exploratory Data Analysis (EDA)

Performed exploratory analysis on the financial news dataset to identify publishing patterns and headline characteristics.

Completed analyses include:

- Headline length analysis
- Publisher activity analysis
- Publication trend analysis
- Time-based publishing patterns
- Data quality assessment and preprocessing

Visualizations were created to better understand publishing behavior and temporal activity trends.

---

## Task 2 — Quantitative Stock Analysis

Performed technical analysis on multiple stock datasets using financial indicators and return metrics.

### Companies analyzed

- AAPL
- AMZN
- GOOG
- META
- NVDA

### Indicators and metrics used

- Simple Moving Average (SMA)
- Relative Strength Index (RSI)
- MACD
- Daily Returns
- Volatility
- Cumulative Returns

The analysis explored momentum, trend behavior, volatility, and long-term stock performance.

---

## Task 3 — Sentiment and Correlation Analysis

Implemented a sentiment analysis and stock correlation workflow using financial news headlines and stock price data.

### Completed workflow

- Sentiment scoring using TextBlob
- Sentiment categorization
- Date normalization and alignment
- Weekend and holiday adjustment
- Daily stock return calculation
- Pearson correlation analysis
- Scatter plot visualization
- Sentiment-category return comparison

The workflow investigated relationships between financial news sentiment and stock market movement.

---

# Requirements

Core dependencies are listed in `requirements.txt`.

### Main libraries used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- nltk
- textblob
- scipy
- ta
- Jupyter Notebook

---

# Environment Setup

## Clone Repository

```bash
git clone <repository-link>
```

## Navigate Into Project

```bash
cd news-sentiment-analysis
```

## Create Virtual Environment

```bash
python -m venv venv
```

## Activate Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Launch Jupyter Notebook

```bash
jupyter notebook
```

---

# Reproducing the Analysis

1. Open the `notebooks` directory
2. Run the Task 1 EDA notebook
3. Run the Task 2 stock analysis notebooks
4. Run the Task 3 sentiment analysis notebooks
5. Review generated visualizations and statistical outputs

---

# Key Findings

- Financial news activity varied significantly across publishers and time periods.
- Different companies demonstrated different volatility and momentum characteristics.
- Financial headlines contained a mixture of positive, neutral, and negative sentiment.
- Correlation between sentiment and stock returns was generally weak, suggesting that stock movement is influenced by multiple additional factors.
- Sentiment analysis still provides useful contextual information for understanding market behavior and investor reaction patterns.

---

# Notes

- The news dataset used the historical ticker symbol `FB` for Meta Platforms, while the stock dataset used the updated `META` naming convention.
- Weekend and holiday news items were aligned to the next available trading day during correlation analysis.

---

# Author

Sumeya