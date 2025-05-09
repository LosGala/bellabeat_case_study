# 📊 Bellabeat Case Study - Google Data Analytics Capstone Project

![Bellabeat Logo](Bellabeat.png)

**Author**: Mario Ariel Galarza Mancedo  
**Date**: January 19, 2024  
**Certificate Program**: Google Data Analytics Professional Certificate  
**Dataset**: [FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit)

---

## 🔍 Introduction

This case study is part of the Capstone Project for the Google Data Analytics Professional Certificate. The goal is to analyze consumer data from FitBit fitness trackers and derive insights that could guide **Bellabeat**, a wellness tech company for women, in improving its **marketing strategy**.

---

## 🧠 Business Task

Bellabeat wants to better understand how consumers use fitness tracking technology. By analyzing FitBit data, we aim to:

- Identify trends in fitness tracker usage.
- Explore how these trends may relate to Bellabeat users.
- Provide data-driven recommendations to support Bellabeat's marketing efforts.

---

## 🎯 Business Objectives

- What are the key trends in FitBit user behavior?
- How can these trends inform Bellabeat’s product and marketing strategies?
- How can Bellabeat leverage these insights to grow their market?

---

## 📁 Data Overview

- **Source**: Publicly available dataset from [Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit)
- **Timeframe**: March 12, 2016 – May 12, 2016
- **Participants**: 30 consenting users (33 unique IDs found)
- **Files**: 18 CSV files (only `dailyActivity_merged.csv` used for this analysis)

### Limitations

- Small and outdated dataset (from 2016)
- Data collected via third-party survey (Amazon Mechanical Turk)
- Limited sample size and demographic representation

> **Conclusion**: While the dataset is limited in scope and reliability, it still provides a basis for basic trend analysis.

---

## 🧰 Tools Used

- **Language**: Python
- **Libraries**:
  - `pandas` for data manipulation
  - `numpy` for numerical operations
  - `matplotlib` for data visualization
  - `datetime` for date formatting and time series analysis

---

## 🧹 Data Cleaning & Processing

- Converted `ActivityDate` to datetime format
- Extracted day of the week for time pattern analysis
- Created new columns:
  - `total_mins` = sum of active and sedentary minutes
  - `total_hours` = `total_mins` converted to hours
- Standardized and renamed column headers for consistency

---

## 📊 Analysis Preview

- Data consists of 940 daily activity records.
- Average daily steps and calories burned per user are being analyzed.
- Users’ activity patterns across weekdays vs. weekends are explored.
- Initial findings suggest correlations between activity minutes and calories burned.

---

## 📈 Key Insights (to be expanded)

- Users tend to be **more active during weekdays**, particularly Tuesdays and Wednesdays.
- There is a **positive correlation** between very active minutes and calories burned.
- Sedentary minutes remain high across all days, suggesting a target area for product messaging.

---

## 🧩 Next Steps

- Extend analysis to include `sleep` and `heart rate` data.
- Generate visual dashboards for trend exploration.
- Develop marketing recommendations tailored to identified user behaviors.

---

## 📎 Project Structure

