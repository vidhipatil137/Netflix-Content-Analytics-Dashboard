# 📊 Netflix Content Analytics Dashboard

An end-to-end Excel project analyzing Netflix's content catalog (8,800+ titles) — 
from raw, messy data to a fully interactive dashboard.

## 🎯 Overview

This project takes the raw Kaggle "Netflix Titles" dataset and transforms it into 
a clean, analysis-ready dataset using Power Query, then builds PivotTables, KPIs, 
and an interactive dashboard with slicers.

## 🛠️ Tools & Skills Used

- **Power Query** — data cleaning & transformation
- **PivotTables** — data summarization
- **Excel Formulas** — COUNTA, COUNTIF, COUNTIFS, AVERAGEIFS
- **Charts** — Line, Bar, Column, Pie
- **Slicers** — interactive filtering
- **Dashboard Design** — custom KPI cards, Netflix-themed color palette

## 🧹 Data Cleaning Process

1. Imported raw CSV via Power Query (kept original untouched in `Raw_Data` sheet)
2. Fixed missing values in `director`, `cast`, `country`, and `rating` columns
3. Identified and fixed a real data quality issue — 3 rows had their `rating` 
   and `duration` values swapped due to a source formatting quirk
4. Fixed a CSV parsing error caused by an embedded line break in one title field 
   (adjusted `QuoteStyle` in the Power Query source step)
5. Split the `duration` column into `Duration_Value` (number) and `Duration_Unit` 
   (min/Season) for proper numeric analysis
6. Converted `date_added` from text to a proper Date type

## 📈 Key KPIs

| Metric | Value |
|---|---|
| Total Titles | 8,807 |
| Total Movies | 6,131 |
| Total TV Shows | 2,676 |
| Movies % | 69.6% |
| Avg. Movie Duration | 99.6 min |
| Titles Added in 2021 | 592 |

## 📊 Dashboard Features

- Movies vs TV Shows split
- Content added trend by release year
- Top 10 countries by number of titles
- Rating distribution
- Top genres
- Interactive slicers: Type, Release Year, Rating

## 📁 Files

- `Netflix_Data_Analysis_Project.xlsx` — full project (Raw Data, Cleaned Data, 
  PivotTables, KPIs, Dashboard)
- Dashboard screenshot (for quick preview without opening Excel)

## 💡 Key Insight

Movies make up nearly 70% of Netflix's catalog, and content additions peaked 
sharply around 2019-2020 before slowing down.
