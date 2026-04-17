# 📣 Promo Campaign Analysis

## 📌 Project Overview

The goal of this project is to explore and analyze a **Market Promotional Campaign dataset**.  
I've focused on understanding **campaign performance, customer response, sales impact, and ROI** across different promotion types.  
This EDA helps us understand which promotional strategies drive the most value.

---

## 📂 Dataset

- **Source**: Market Dataset (provided)
- **Key Columns** used:
  - `campaign_type` – Type of promotion
  - `start_date / end_date` – Campaign duration
  - `spend` – Amount spent on the campaign
  - `revenue` – Revenue generated
  - `conversions` – Number of customer conversions
  - `channel` – Marketing channel used (e.g., social media, email, TV)

---

## ⚙️ Data Preparation

1. **Loaded dataset** and inspected shape, data types, and missing values.
2. **Converted date columns** into datetime format for time-based analysis.
3. **Created new features**:
   - `profit = revenue – spend`
   - `roi = profit / spend` (return on investment)
   - `conversion_rate = conversions / impressions`
   - `duration` extracted from `start_date` and `end_date`
4. **Handled missing values** by coercing invalid entries into `NaN`.

---

## 📊 Exploratory Data Analysis

### 🔹 1. Overall Distribution

- Most campaigns have **moderate spend and moderate returns**.
- A few high-performing campaigns dominate overall revenue.

📌 *Tools*: `histplot`, KDE plots

---

### 🔹 2. Campaign Performance by Type

- Compared average revenue, spend, and ROI across campaign types.
- 📈 Found that certain campaign types consistently outperform others.

📌 *Tools*: `groupby`, bar plots

---

### 🔹 3. Top 10 Best Performing Campaigns

- Identified the campaigns with the highest profit and ROI.
- Visualized with horizontal bar charts.

📌 *Tools*: `sort_values`, `barplot`

---

### 🔹 4. Correlation Analysis

- Explored relationships between spend, revenue, conversions, and duration.
- High spend does not always guarantee high ROI.

📌 *Tools*: `heatmap`

---

### 🔹 5. Trends Over Time

- Analyzed how campaign performance changed over time.
- Identified peak periods for promotions.

📌 *Tools*: `groupby`, line plots

---

## 📌 Key Insights

1. 📣 **Not all campaigns are equally effective** – a few drive the majority of results.
2. 💰 **Spend and revenue show moderate correlation** – strategy matters more than budget.
3. 📈 **Certain time periods see higher campaign success** – timing is key.
4. ⚖️ **High spend ≠ high ROI** – smaller, targeted campaigns sometimes outperform large ones.

---

## 🛠️ Tools & Libraries

- **Python 3**
- **Pandas** → data cleaning, feature engineering
- **Matplotlib / Seaborn** → visualization
- **NumPy** → numeric operations
- **SQL** → data querying
- **Power BI / Excel** → dashboards and reporting

---

## ✅ Conclusion

This project demonstrates how to:

- Clean and preprocess marketing campaign data.
- Perform ROI and performance analysis with Pandas.
- Use EDA to uncover trends and actionable insights in promotional data.

---
