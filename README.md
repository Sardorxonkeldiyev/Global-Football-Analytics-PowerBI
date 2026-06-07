# ⚽ International Football Performance & Elo Ratings Analytics Dashboard

An advanced, interactive Power BI dashboard analyzing historical and current football data from **1990 to 2026**. This project provides deep insights into team rankings, global match trends, and tactical balances (offense vs. defense) on both global and national levels.

## 🚀 Key Features & Pages

### 1. 🗺️ Global Overview
* **Top 10 Nations:** Visualizes top-performing countries based on their maximum Elo ratings.
* **Confederation Share:** Analyzes match distribution and dominance among UEFA, CONMEBOL, AFC, CAF, CONCACAF, and OFC using an interactive Donut Chart.
* **Scoring Leaders:** Funnel chart representation of the highest-scoring nations in football history.
* **Global Growth Trend:** Area chart demonstrating the rise of international matches over the decades.

### 2. 🇺🇿 Uzbekistan National Team Analysis (Special Focus)
* Detailed historical trend of Uzbekistan's Elo rating and world ranking.
* **KPI Center:** Real-time metrics including Current Rating (1727), World Rank (38), Total Matches (365), and an advanced DAX-calculated **Win Rate (49.32%)**.
* **Attack vs. Defense:** Bar-by-bar annual comparison of goals scored vs. goals conceded.

### 3. 🎯 Offense and Defense Analysis
* **Tactical Correlation:** Advanced Scatter Plot analyzing team styles by mapping scoring efficiency against defensive stability.
* **Defensive Vulnerabilities:** Highlights the Top 10 countries with the most goals conceded.
* **Confederation Efficiency:** Compares the average goal-scoring power across different continental federations.

## 🛠️ Tech Stack & DAX Formulas Used
* **Tool:** Microsoft Power BI Desktop
* **Data Transformation:** Power Query (Data cleaning, handling snapshots, date parsing, and eliminating anomalies via advanced filtering).
* **Key DAX Measure:**
```dax
  Win_Rate = DIVIDE(SUM('elo_ratings_wc2026'[wins]), SUM('elo_ratings_wc2026'[matches_total]), 0)
  ---
  📸 Dashboard Preview
<img width="1273" height="712" alt="Global Overview WC (1990-2026)" src="https://github.com/user-attachments/assets/94e43268-74b5-4f46-93c8-fb5866e1ecd9" />

More ... --> Screenshots folder

🗃️ Dataset Source
The analysis is driven by historical Elo rating snapshots and international match logs up to the year 2026.
