# 🎬 Netflix Content Strategy & Analytics - Final Case Study

**A Comprehensive Data Analytics Project for the SWYNEX Technologies Virtual Internship.**

## 1. Problem Statement
The streaming industry is highly competitive. To maintain market leadership, streaming platforms must constantly adapt their content libraries to match viewer preferences and global trends. The objective of this project is to analyze the Netflix catalog to uncover key trends in content distribution, geographical reach, and target demographics, ultimately providing actionable business insights for future content acquisition strategies.

## 2. Dataset Information
* **Source:** Kaggle (Netflix Movies and TV Shows Dataset)
* **Size:** 7,770 records across 12 attributes.
* **Key Variables:** `show_id`, `type` (Movie/TV Show), `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `genres`.

## 3. Data Cleaning & Preparation
The raw data contained inconsistencies which were resolved using **Python (Pandas)**:
* **Duplicate Removal:** Identified and dropped exact duplicate rows to maintain data integrity.
* **Handling Missing Values:** 
  * Imputed missing `director`, `cast`, and `country` values with 'Unknown'.
  * Dropped records with missing critical temporal data (`date_added`).
* **Data Type Standardization:** Parsed messy string dates into proper Python `DateTime` objects for accurate time-series analysis.

## 4. Exploratory Data Analysis (EDA)
Using **Matplotlib** and **Seaborn**, statistical analysis was performed to uncover initial patterns:
* Calculated the distinct ratio of Movies to TV Shows.
* Identified peak release years and content growth velocity.
* Mapped the top 10 content-producing nations.
* *Code and initial charts are available in the `Python_EDA/` folder.*

## 5. Interactive Dashboard (Power BI)
An interactive, dark-themed Power BI dashboard was developed to visualize the findings for business stakeholders. 

### 📊 Dashboard Previews

**1. Content Distribution & Yearly Trends Overview**
![Dashboard 1](PowerBI_Dashboard/pb1.png)

**2. Global Reach & Demographics**
![Dashboard 2](PowerBI_Dashboard/pb2.jpeg)

**3. Release Trends & Top Countries Treemap**
![Dashboard 3](PowerBI_Dashboard/pb3.jpeg)

## 6. Key Business Insights
Based on the end-to-end analysis, here are the top 5 strategic insights:
1. **Movie-Centric Library:** Movies dominate the platform, constituting **69.14%** (5,372 titles) of the catalog compared to **30.86%** for TV Shows.
2. **Key Geographical Markets:** The **United States** (3,287 titles) and **India** (990 titles) are the primary drivers of content volume, highlighting India's critical role in Netflix's international expansion strategy.
3. **Targeting Mature Audiences:** Over 60% of the content is rated **TV-MA** (2,861 titles) and **TV-14** (1,928 titles), indicating a strong strategic focus on mature, young-adult, and adult demographics rather than children's programming.
4. **Acquisition Boom (2017-2019):** There was an aggressive spike in content acquisition peaking around 2017-2019, followed by a stabilization period.
5. **Genre Popularity:** **International Movies (2,437)** and **Dramas (2,105)** are the most saturated genres, reinforcing the platform's global and narrative-driven approach.

---
**Tools Used Throughout the Project:** Python, Pandas, Matplotlib, Seaborn, Google Colab, Microsoft Power BI.
