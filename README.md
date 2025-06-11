# 📊 Stock Market Sentiment Analysis Dashboard

This Power BI project presents a **Stock Price Sentiment Analysis** based on social media (Twitter) data. It provides a visual summary of public sentiment toward various stocks, helping investors and analysts make informed decisions based on public perception and news trends.

---

## 🚀 Project Objective

To analyze the **sentiment of tweets** related to selected stocks and visualize the public opinion distribution (Positive, Neutral, Negative) in a clear and interactive dashboard. This enables real-time understanding of market psychology.

---

## 📌 Key Features

- 🔎 **Sentiment Breakdown**: Bar chart showing sentiment distribution (Positive, Neutral, Negative) for each stock.
- 🧠 **Word Cloud**: Highlights the most frequently occurring terms in tweets to reveal trending topics.
- 📈 **Stock and Tweet Count**: KPI cards display the total number of analyzed stocks and tweets.
- 🧭 **Interactive Filters**: Dropdown slicers for selecting specific stocks or sentiments.
- 📊 **Donut Chart**: Shows overall sentiment distribution across all tweets.
- 🧾 **Live Tweet Viewer**: Scrollable table to read individual tweets by sentiment category.

---

## 🧠 Tools & Technologies Used

- **Power BI Desktop** for dashboard design and interactivity
- **Python / NLP** (assumed for backend sentiment analysis)
- **DAX** for calculated measures and KPIs
- **Data Cleaning** & Preprocessing via Power Query Editor

---

## 📊 Insights Gained

- Majority sentiment was **positive** (51.56%) across 10 stocks and 320 tweets.
- Stocks like **RCAT, ELF, DKNG** showed higher positive mentions.
- Key words like `growth`, `target`, `price`, and `market` dominated the discussion.

---

## 🧩 Potential Enhancements

- Integration with **real-time Twitter API** for continuous monitoring
- **Sentiment scoring** instead of just categories
- Historical trend analysis of sentiment vs stock price changes

---

## 💡 Learnings & Takeaways

This project enhanced my understanding of:
- Combining **NLP with BI tools** for social media analysis
- Using **Power BI visualizations** to communicate insights clearly
- The importance of sentiment in stock price perception
---

## 🔗 Connect With Me

📧 Email:kutarmareajinkya52@gmail.com
💼 LinkedIn: [Ajinkya Kutarmare](https://www.linkedin.com/in/ajinkya-kutarmare-107540258?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

---

> “In the world of finance, data tells stories. This dashboard helps decode them.”

# 📈 Stock Market Sentiment Analysis using Twitter Data

This project presents a **Stock Sentiment Tracking System** that scrapes live tweets from X (formerly Twitter), performs sentiment analysis using the VADER model, and visualizes insights through a dynamic Power BI dashboard.

> **By Ajinkya Kutarmare**

---

## 🎯 Project Objective

### ✅ Business Goals
- Enhance **investment decision-making** by analyzing public sentiment from social media.
- Detect **positive/negative trends** in stock discussions to anticipate market movements.
- Support **portfolio risk assessment** based on public opinion shifts.
- Provide **real-time market sentiment** for 10 actively discussed stocks.

### 🛠️ Technical Goals
- Implement an **automated pipeline** using web scraping and NLP.
- Use **Selenium** for real-time tweet scraping.
- Apply **VADER sentiment analysis** to classify tweets.
- Store results in structured CSVs and visualize them using **Power BI**.

---

## 🔍 Methodology

### 1. 🕸 Web Scraping
- Tweets were collected using Selenium targeting keywords like `$RCAT`, `$DKNG`, etc.
- The scraper supports randomized delays, retries, and scrolling for dynamic loading.
- Tweets were stored with the stock symbol, text, and timestamp.

### 2. 💬 Sentiment Analysis
- Each tweet was passed through the **VADER** model (a lexicon-based sentiment analyzer).
- Tweets were categorized as **Positive**, **Neutral**, or **Negative**.
- Output was saved to `stock_sentiment.csv` for further analysis.

### 3. 📊 Power BI Dashboard
- Key visuals include:
  - Sentiment bar charts by stock
  - Donut chart of sentiment distribution
  - Word cloud of frequent stock-related terms
  - Live tweet table
  - KPI tiles (# of stocks and # of tweets)

---

## 📊 Dashboard Insights

| Metric                  | Value         |
|-------------------------|---------------|
| 📈 Total Tweets         | 320           |
| 🏦 Stocks Analyzed      | 10            |
| 😀 Positive Sentiment   | 51.56%        |
| 😐 Neutral Sentiment    | 36.25%        |
| 😠 Negative Sentiment   | 12.19%        |

### 📌 Per Stock Highlights
- **DKNG**: 52% positive. Investors are bullish due to strong earnings and CEO confidence.
- **ARDX**: 74% positive. High optimism due to analyst ratings and product performance.
- **ELF**: 58% positive. Despite some sales concerns, growth outlook remains strong.
- **HIMS**: 52% positive. Undervalued stock with aggressive marketing strategies.
- **RCAT**: 49% positive. Positive buzz around drone tech, but concerns on volatility.
- **LYFT**: 60% positive. Considered a potential buy-the-dip or acquisition target.
- **TMDX**, **PDD**, **INDI**, **WRBY**: Mixed sentiments with optimism tempered by market concerns.

---

## ☁️ Word Cloud

The dashboard includes a **Word Cloud** visual that highlights top keywords such as:
`market`, `growth`, `undervalued`, `buy`, `target`, `earnings`, `CEO`, `stock`, etc.

---

## 🧠 Tools & Technologies

- 🐍 Python (Selenium, Pandas, VADER)
- 📄 CSV for intermediate datasets
- 📊 Power BI for interactive visualization
- 💡 NLP (Natural Language Processing) for sentiment classification

---

## 🛠️ File Structure

```plaintext
📁 Project Files
├── web_scraping_code.py           # Scraper for tweets
├── sentimental_analysis.py       # VADER-based sentiment classifier
├── stocks_tweets.csv             # Raw scraped tweets
├── stock_sentiment.csv           # Sentiment-labeled data
├── wordcloud_data.py             # Word cloud generator
├── wordcloud_data.csv
└── Power_BI.pbi                  # Power BI dashboard file

