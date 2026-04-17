# Bitcoin Market Sentiment vs Trader Performance

## Overview

In this project, I analyzed how market sentiment (Fear vs Greed) affects trader behavior and performance.

The idea was to combine sentiment data with actual trading data and see if traders behave differently in different market conditions, and whether that impacts profitability.

---

## Approach

First, I cleaned both datasets and converted timestamps into a common date format.  
Then I merged them on a daily level so that each trading activity could be linked with the corresponding market sentiment.

After that, I created a few key metrics:
- Daily PnL  
- Win rate (percentage of profitable trades)  
- Trade count  
- Trade size (used as a proxy for risk since leverage was not available)

I then compared these metrics across Fear and Greed conditions and also looked at different types of traders (frequent vs infrequent, high vs low activity).

---

## Key Findings

- Trading activity increases during Greed periods, indicating higher market participation.
- Traders tend to behave more cautiously during Fear periods (smaller trade sizes).
- Profitability patterns vary, but Fear phases often show more stable outcomes.
- Greed phases show higher volatility, suggesting riskier behavior.
- Frequent traders are more affected by changes in sentiment.

---

## Strategy Ideas

Based on the analysis:

- A contrarian approach can work well: look for opportunities during Fear phases.
- Be cautious during Greed periods as overtrading and volatility increase.
- Managing trade size is important, especially in uncertain market conditions.

---

## Bonus Work

I also built a simple machine learning model to predict whether a trade will be profitable or not using:
- Sentiment
- Trade size
- Trader activity

The model achieved around 62% accuracy, which suggests that sentiment and behavior do have some predictive value, but other factors are also important.

I also tried clustering traders into different groups based on their behavior.

---

## How to Run

## How to Run

1. Install required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn

2. Open Jupyter Notebook:
jupyter notebook

3. Open the file:
analysis.ipynb

4. Run all cells to see results and visualizations 
