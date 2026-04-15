# 📊 Trader Performance vs Market Sentiment

## 📌 Objective

This project analyzes the relationship between **Bitcoin market sentiment (Fear/Greed Index)** and **trader behavior & performance** on Hyperliquid.
The goal is to uncover patterns that can help design smarter trading strategies.

---

## 📂 Datasets Used

### 1. Market Sentiment Dataset

* Contains daily Bitcoin sentiment classification:

  * Extreme Fear
  * Fear
  * Neutral
  * Greed
  * Extreme Greed

### 2. Trader Dataset (Hyperliquid)

* Includes:

  * Account
  * Symbol
  * Execution Price
  * Trade Size
  * Side (Long/Short)
  * Closed PnL
  * Leverage
  * Timestamp

---

## ⚙️ Methodology

### 🧹 Data Preparation

* Loaded and cleaned both datasets
* Removed duplicates and handled missing values
* Converted date/time columns to proper datetime format
* Created a numerical sentiment score:

  * Extreme Fear = 0
  * Fear = 1
  * Neutral = 2
  * Greed = 3
  * Extreme Greed = 4

---

### 📊 Feature Engineering

* Daily PnL per trader
* Trade frequency (trades per day)
* Average trade size
* Leverage distribution
* Long/Short ratio

---

### 🔍 Analysis Performed

* Compared trader performance across:

  * Fear vs Greed days
* Analyzed behavioral changes:

  * Trade frequency
  * Leverage usage
  * Position bias (Long/Short)
* Identified trader segments:

  * High vs Low leverage traders
  * Frequent vs Infrequent traders
  * Consistent vs Inconsistent performers

---

## 📈 Key Insights

1. **Market sentiment follows cyclical patterns**, shifting between fear and greed phases.
2. **Extreme Fear periods often precede recovery**, suggesting potential contrarian opportunities.
3. **Trader behavior changes with sentiment**:

   * Higher caution during fear phases
   * More aggressive positions during greed phases

---

## 🧠 Strategy Recommendations

1. **Risk Management Strategy**

   * Reduce leverage during Fear and Extreme Fear periods
   * Protect capital during uncertain market conditions

2. **Opportunity Strategy**

   * Increase participation during Neutral to Greed transitions
   * Identify reversal opportunities during Extreme Fear

> Sentiment alone is not sufficient, but when combined with trader behavior, it can significantly improve decision-making.

---

## 📊 Visualizations

### Market Sentiment Trend

![Sentiment Trend](outputs/sentiment_trend.png)

### Sentiment Distribution

![Distribution](outputs/sentiment_distribution.png)

---

## 🛠️ Tools & Technologies

* Python (Pandas, NumPy)
* Matplotlib / Seaborn
* Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/trader-performance-vs-market-sentiment.git
```

2. Open the notebook:

```
jupyter notebook
```

3. Run all cells to reproduce the analysis

---

## 📌 Conclusion

This analysis highlights how **market sentiment influences trading behavior and performance**.
Combining sentiment data with trading metrics can help build more informed and adaptive trading strategies.

---

## 👤 Author

Baleshwar Gehlot
