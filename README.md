# 🛍️ Customer_Behavior_Analysis

> An end-to-end data analytics project analyzing customer shopping behavior through Python, MySQL, Power BI, and a professional presentation — uncovering insights to drive smarter business decisions.

---

## 📌 Overview

This project explores transactional retail data to understand **how customers shop**, **what they buy**, and **how businesses can improve revenue and retention**. The full analytics pipeline covers:

- Data loading & cleaning in **Python**
- Exploratory Data Analysis (**EDA**)
- Business queries in **MySQL Workbench**
- Interactive **Power BI Dashboard**
- Professional **Report & PPT** using Gamma

---

## 📂 Dataset

| Property | Details |
|---|---|
| **Total Records** | 3,900 transactions |
| **Total Features** | 18 columns |
| **Missing Values** | 37 (Review Rating column) |

### Key Features:
- **Demographics** — Age, Gender, Location, Subscription Status
- **Purchase Info** — Item, Category, Amount (USD), Season, Size, Color
- **Behavior** — Discount Applied, Promo Code, Frequency, Review Rating, Shipping Type

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| 🐍 **Python (Pandas)** | Data loading, cleaning, EDA, feature engineering |
| 🗄️ **MySQL Workbench** | SQL queries & business analysis |
| 📊 **Power BI** | Interactive dashboard & visual insights |
| 📄 **Gamma** | Report & PowerPoint presentation |
| 🐙 **GitHub** | Version control & project hosting |

---

## 🔢 Project Steps

### Step 1 — Data Loading & EDA (Python)
- Imported dataset using `pandas`
- Used `df.info()` and `df.describe()` for initial exploration
- Identified **37 missing values** in the `Review Rating` column

### Step 2 — Data Cleaning (Python)
- Imputed missing ratings using **category-wise median**
- Renamed all columns to **snake_case** for consistency
- Engineered new features:
  - `age_group` — binned customer ages into groups
  - `purchase_frequency_days` — derived from purchase frequency data
- Dropped redundant column `promo_code_used` (duplicate of `discount_applied`)

### Step 3 — Database Integration
- Connected Python script to **MySQL Workbench**
- Loaded cleaned DataFrame into MySQL for structured querying

### Step 4 — SQL Business Analysis (MySQL Workbench)

| # | Query | Insight |
|---|---|---|
| 1 | Revenue by Gender | Male: $157,890 \| Female: $75,191 |
| 2 | High-Spending Discount Users | 839 customers spent above average with discounts |
| 3 | Top 5 Products by Rating | Gloves (3.86), Sandals (3.84), Boots (3.82) |
| 4 | Shipping Type Comparison | Express $60.48 \| Standard $58.46 |
| 5 | Subscribers vs Non-Subscribers | 1,053 subscribers \| 2,847 non-subscribers |
| 6 | Discount-Dependent Products | Hat 50% \| Sneakers 49.66% \| Coat 49.07% |
| 7 | Customer Segmentation | Loyal: 3,116 \| Returning: 701 \| New: 83 |
| 8 | Top 3 Products per Category | Jewelry, Blouse, Sandals, Jacket lead categories |
| 9 | Repeat Buyers & Subscriptions | Non-subscribers dominate repeat buying (2,518) |
| 10 | Revenue by Age Group | Young Adults top revenue at $62,143 |

### Step 5 — Power BI Dashboard
- Built an interactive dashboard with slicers, KPI cards, bar charts, and a donut chart
- See [Dashboard](#-dashboard) section below

### Step 6 — Report & Presentation
- Created a professional project report using **Gamma**
- Built a clean, visual **PowerPoint presentation** summarizing all findings

---



