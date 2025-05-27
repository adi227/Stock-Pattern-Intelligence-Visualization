# 📊 Stock Pattern Intelligence Visualization

An advanced Tableau-based dashboard project that visualizes and predicts long-term stock performance trends across major tech companies. This platform helps financial analysts and investors explore stock behavior using historical data and technical indicators, and now includes **regression-based stock trend predictions**.

---

## 📁 Dataset Overview

- **Source**: [Yahoo Finance](https://finance.yahoo.com/)
- **File**: `combined_stock_data.csv`
- **Companies**: Amazon, Apple, Meta, Google, Microsoft, Nvidia, Tesla
- **Records**: ~38,000 daily entries from 1997–2020
- **Features Used**: Closing price, volume, MA50, MA200, percentage changes, etc.

---

## 🔍 Key Insights & Research Questions

1. **📈 How have stock closing prices changed over time?**  
   → Multi-line/area chart with company/date filters

2. **📊 How does average trading volume vary by company?**  
   → Stacked bar chart, year range filter

3. **📉 What’s the correlation between price and volume change?**  
   → Scatter plot visualizing volatility/sentiment

4. **📐 Do MA crossovers indicate momentum shifts?**  
   → Dual-line chart with forecast toggles (MA50 vs MA200)

5. **🔮 Can we classify stock risk levels as High/Medium/Low?**  
   → Implemented via advanced regression-based scoring to tag stock performance categories  
   → Classification logic:  
      - **High**: Large positive change + high volume  
      - **Medium**: Moderate fluctuations  
      - **Low**: Stable prices with minimal change  
   → Labels generated using thresholds on regression model output (linear/logistic)

---

## 🛠 Dashboard Features

- Fully interactive Tableau dashboard
- Company, Year, and Forecast toggle filters
- Hover tooltips and dynamic tool containers
- MA forecasting with trend lines and confidence intervals
- **Stock trend prediction** (H/M/L) integrated using classification overlays or tooltips

📸 *Visual preview available on page 8 of the report*

---

## 👤 User Persona

**Name**: Priya Nair  
**Role**: Investment Research Analyst  
**Use Case**: Monitor stock signals, assess volatility, and make informed trade decisions

---

## 📚 Design & Principles

- UCD (User-Centered Design, ISO 9241-210:2010)
- Nielsen’s Heuristics (system feedback, flexibility)
- Shneiderman’s Visual Mantra (overview > zoom/filter > details-on-demand)

---

## 🔧 Tech Stack

- **Tableau**: Visualization, forecasting, filtering
- **Regression Modeling**: Scikit-learn (Python), exported to Tableau
- **Excel/CSV**: Data prep
- **Prediction Logic**: Derived thresholds from regression-based scoring

---

## ⚖️ Tableau vs Shiny (R)

| Feature                     | Tableau                          | Shiny (R)                          |
|----------------------------|----------------------------------|------------------------------------|
| Forecasting                | ✔ Built-in MA prediction         | ✖ Requires manual setup            |
| MA Crossover Detection     | ✔ Visual + logic integration     | ✖ Manual; no dynamic crossover     |
| Risk Labeling              | ✔ With regression overlays       | ✖ Basic interactivity only         |
| Interactivity              | ✔ Filters, tooltips, drilldowns  | ✔ Functional, less visual polish   |


