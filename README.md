# Financial News and Stock Price Analysis

## Project Overview

This project analyzes the relationship between financial news sentiment and stock market behavior by combining exploratory data analysis (EDA), technical financial analysis, and natural language processing techniques.

The project focuses on:

* Exploring large-scale financial news headline datasets
* Identifying publication trends and publisher activity
* Performing quantitative stock price analysis using technical indicators
* Computing financial performance metrics
* Investigating potential relationships between news sentiment and stock price movement

---

# Business Objective

Financial markets react rapidly to news events, analyst reports, earnings announcements, and broader economic developments. The objective of this project is to explore whether financial news sentiment can provide meaningful insight into stock price behavior and market trends.

By integrating natural language processing with quantitative financial analysis, the project aims to better understand how information flow may influence investor behavior and market activity.

---

# Project Structure

```text
news-sentiment-analysis/
├── .vscode/
├── .github/
│   └── workflows/
├── data/
│   └── raw/
├── notebooks/
│   ├── eda.ipynb
│   └── financial_analysis.ipynb
├── reports/
│   └── interim_report.md
├── src/
├── tests/
├── scripts/
├── requirements.txt
├── README.md
└── .gitignore
```

---

# Data Sources

## Financial News Dataset

The news dataset contains:

* Financial news headlines
* Publisher information
* Publication timestamps
* Stock references

This dataset is used for exploratory analysis and sentiment analysis.

## Historical Stock Price Dataset

The stock datasets contain:

* Open prices
* High prices
* Low prices
* Close prices
* Trading volume
* Date information

These datasets are used for technical analysis and financial metric computation.

---

# Tasks Completed

## Task 1 — Exploratory Data Analysis

The following analyses were completed:

* Dataset inspection and preprocessing
* Headline length analysis
* Publisher activity analysis
* Publication trend analysis
* Publication-hour analysis
* Keyword and topic pattern analysis

### Key Findings

* Financial news headlines are generally concise and information-dense.
* A small number of publishers contribute a large proportion of articles.
* Publication frequency shows noticeable spikes during periods of increased market activity.
* Common keywords strongly relate to earnings, stock prices, and market performance.

---

## Task 2 — Quantitative Financial Analysis

Technical analysis was performed using reusable workflows applied across multiple stock datasets.

### Technical Indicators

* Simple Moving Average (SMA)
* Exponential Moving Average (EMA)
* Relative Strength Index (RSI)
* Moving Average Convergence Divergence (MACD)

### Additional Financial Metrics

* Daily Returns
* Cumulative Returns
* Volatility-related metrics

### Key Findings

* Several stocks exhibited strong long-term upward trends.
* RSI and MACD revealed multiple momentum shifts and volatility changes.
* Technical indicators successfully highlighted trend behavior and market movement patterns.

---

# Data Preparation and Quality Issues

Several preprocessing and cleaning steps were performed during the project:

* Removed unnecessary index columns
* Converted date columns into datetime format
* Standardized timestamps for time-series analysis
* Generated derived analytical features
* Prepared reusable workflows for multi-stock analysis

### Challenges Encountered

* Mixed datetime formats within the news dataset
* Timestamp normalization inconsistencies
* CI/CD dependency conflicts caused by Windows-specific packages
* Large file tracking issues caused by dataset commits

These issues were resolved through preprocessing improvements, dependency cleanup, and Git workflow adjustments.

---

# Reusable Multi-Stock Workflow

A reusable analysis pipeline was implemented to efficiently apply preprocessing, technical indicator computation, and visualization steps across multiple stock datasets.

This approach improves:

* Scalability
* Consistency
* Maintainability
* Reproducibility

---

# Visualizations

The project includes multiple analytical visualizations, including:

* Headline length distributions
* Publisher activity charts
* Publication trend analysis
* Keyword frequency plots
* Stock price trend plots
* SMA and EMA trend visualizations
* RSI momentum analysis plots
* MACD indicator plots
* Cumulative return trend analysis

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook
* TA Library (`ta`)
* Git & GitHub
* GitHub Actions

---

# Installation

Clone the repository:

```bash
git clone <repository-url>
cd news-sentiment-analysis
```

Create virtual environment:

```bash
python -m venv venv
```

Activate virtual environment:

### Windows

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Run notebooks in the following order:

1. `notebooks/eda.ipynb`
2. `notebooks/financial_analysis.ipynb`

---

# CI/CD Workflow

GitHub Actions was configured to automate dependency installation and repository checks during pushes and pull requests.

Workflow configuration:

```text
.github/workflows/unittests.yml
```

---

# My Contributions

My contributions to the project include:

* Data preprocessing and cleaning
* Exploratory data analysis
* Technical indicator implementation
* Reusable workflow development
* Financial metric computation
* Visualization and interpretation
* Git workflow management
* CI/CD setup using GitHub Actions
* Interim report preparation
* Repository documentation

---

# Next Steps

The next phase of the project will focus on:

* Sentiment analysis of financial news headlines
* Sentiment score computation using NLP techniques
* Correlation analysis between sentiment and stock price movement
* Integration of news and financial datasets
* Final reporting and interpretation
