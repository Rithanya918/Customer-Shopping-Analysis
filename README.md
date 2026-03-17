# Customer-Shopping-Analysis

![Customer Behavior Dashboard](https://github.com/user-attachments/assets/0b358de8-bc72-400c-b84e-575be52a7e8f)

> Analyzing 3,900 retail transactions to uncover spending patterns, customer segments, and product preferences using Python, SQL, and Power BI.

---

## Tools Used
| Tool | Purpose |
|------|---------|
| Python (Pandas, NumPy) | Data cleaning & feature engineering |
| PostgreSQL | Business SQL queries |
| Power BI | Interactive dashboard |

---

## Dataset
- **3,900 rows | 18 columns**
- Key fields: Age, Gender, Category, Purchase Amount, Season, Discount Applied, Subscription Status, Shipping Type, Review Rating

---

## Python — Data Preparation
- Imputed 37 missing `review_rating` values using median per category
- Renamed columns to `snake_case`
- Created `age_group` and `purchase_frequency_days` features
- Dropped redundant `promo_code_used` column
- Loaded cleaned data into PostgreSQL via SQLAlchemy

---

## Power BI Dashboard — Questions & Insights

**Overall KPIs:** 3.9K customers | $59.8 avg purchase | 3.75 avg rating

| Visual | Business Question | Insight |
|--------|------------------|---------|
| Subscription Donut | How split are subscribers vs. non-subscribers? | 73% non-subscribers yet spend equally ($59.87 vs $59.49) — large untapped conversion opportunity |
| Revenue by Category | Which category drives the most revenue? | Clothing leads at $104K; Outerwear lags at $19K — seasonal campaigns needed |
| Sales by Category | Which category has the most transactions? | Clothing (3,403K) far outpaces others — concentration risk if demand drops |
| Revenue by Age Group | Which age group spends the most? | Young Adults lead at $62K; all groups within $7K — broad demographic appeal |
| Sales by Age Group | Which age group orders most frequently? | Young Adults place the most orders — primary target for marketing |

---

## Key Recommendations
- **Convert repeat buyers** — 2,518 repeat buyers are non-subscribers; target with loyalty perks
- **Reduce discount dependency** — Hat & Sneakers have ~50% discount rate; consider bundling instead
- **Grow Outerwear & Footwear** — invest in seasonal promotions to close the revenue gap
- **Target Young Adult & Male segments** — highest revenue and order volume demographics

