# 🏏 T20 World Cup Analytics Dashboard

This project offers a comprehensive Power BI dashboard analyzing T20 World Cup performance using structured datasets and DAX metrics. It integrates data from various sources and applies Python-based preprocessing.

---

## 🚀 Tech Stack

<img src="image.png" alt="Tech Stack" width="500"/>

![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Web Scraping](https://img.shields.io/badge/web%20scraping-beautifulsoup-brightgreen?style=for-the-badge)

---

## 📁 Project Structure

- `T20 Analytics Dashboard.pbix` – Main Power BI Report
- `t20_data_preprocessing.ipynb` – Preprocessing using Pandas
- `DAX Measures and Calculated columns.xlsx` – Custom DAX KPIs
- `dim_match_summary.csv`, `dim_players.csv`, `fact_bating_summary.csv`, `fact_bowling_summary.csv` – Structured input data

---

## 📊 Dashboard Features

- Top batsmen and bowlers performance
- Match-by-match summary insights
- Team-wise comparison visuals
- Interactive slicers for team, player, and match filters

---

## 🧪 Preprocessing Highlights

- Merged match and player data
- Formatted dates, null handling, and data types
- Output structured for optimal Power BI ingestion

---

## 🔍 DAX Highlights

```dax
Total Runs = SUM(fact_bating_summary[runs])
Strike Rate = [Total Runs] / [Balls] * 100
Economy = [Runs] / [Overs]
Wickets = SUM(fact_bowling_summary[wickets])
