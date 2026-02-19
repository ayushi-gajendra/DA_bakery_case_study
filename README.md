# 🥖 Strategic Market Expansion: South Korean Bakery Analysis
### *Bridging Stakeholder Intuition with Data-Driven Reality*

![Excel](https://img.shields.io/badge/Tools-Excel%20|%20Google%20Sheets-green)
![Data Analysis](https://img.shields.io/badge/Lifecycle-Full%20Data%20Analysis-blue)
![Business Intelligence](https://img.shields.io/badge/Domain-Business%20Intelligence-orange)
![Business Case](https://img.shields.io/badge/Industry-Retail%20&%20F&B-purple)

---

## 🎯 Executive Summary

**The Mission:** Validate a market entry strategy for a South Korean bakery facing stakeholder pressure to prioritize Croissants.

**The Approach:** Managed the full data analysis lifecycle—from cleaning raw Kaggle transaction data to performing a comparative performance analysis of product categories.

**The Pivot:** The data successfully challenged the investor’s assumptions. While Croissants are a stable performer, **Angbutter** — a culturally resonant favorite—emerged as the primary revenue engine, outperforming Croissants by a staggering **307%**.

**The Impact:** Delivered a data-backed recommendation that protects the bakery from an outdated "niche" strategy, ensuring the product mix aligns with actual consumer spending habits.

---

## 📖 Background & Business Case

### **The Challenge: Stakeholder Bias vs. Market Reality**

A South Korean bakery is currently in high-stakes negotiations with a primary investor. Drawing on market trends from the 1980s, the investor is firmly convinced that Croissants are the ultimate driver of success and has proposed a business model centered exclusively on this single product.

While stakeholder alignment is critical for securing capital, basing a 2026 business strategy on "gut feeling" and decades-old nostalgia introduces significant financial risk. As the lead analyst, my objective was to move beyond subjective "vibe" checks and provide an independent, evidence-based view of the current market.

### **The Strategy: Data-Driven Validation**

I conducted this analysis to stress-test the investor's hypothesis. By examining 2,421 transaction records, I aimed to decode the "Sales DNA" of the bakery to determine if a Croissant-centric model would maximize ROI or if a strategic pivot was necessary to capture modern consumer demand.

---

## 🛠️ Phase 1: Problem Definition & Context
Using the **Rumsfeld Matrix**, I categorized the business requirements to mitigate risk:

* **Known-Knowns:** Opening a bakery in the competitive Korean market requires high operational efficiency.
* **Known-Unknowns:** We knew which items were on the menu, but didn't know the exact customer "Rush Hours" or product-mix preferences.
* **The Challenge (Stakeholder Bias):** The main investor was convinced Croissants were the only path to success. My objective was to determine if this "gut feeling" aligned with market data.

**Impact of Domain Knowledge:** Understanding the local Korean preference for "Angbutter" (Pretzel with red beans and gourmet butter) was critical in contextualizing why Western-style staples (Croissants) might not be the #1 performer.

---

## ⚙️ Phase 2: Data Preprocessing & Scoping
The dataset was sourced from Kaggle (modified) and consisted of **2,421 rows** and **31 core features**
https://www.kaggle.com/datasets/hosubjeong/bakery-sales/data

* **Scoping/Gap Analysis:** The raw `datetime` column was too broad for operational planning.
* **Feature Engineering:** I engineered four new features—`Year`, `Month`, `Day`, and `Hour`—to perform a granular time-series analysis.
* **Cleaning:** Removed empty rows to ensure 100% data integrity.
* **Key Fields Analyzed:**
  * Temporal: datetime, day of week, hour.
  * Financial: total (Total purchase amount in Korean Won).
  * Inventory: 31 items including Angbutter, Plain Bread, Americano, Croissants, Tiramisu, etc.

---
## ⚙️ Phase 3: Analytical Insights

### 📊 Time Trends & Peak Operations
* **Objective:** Identify peak hours and high-traffic days to optimize staffing and inventory.
* **Analysis:** Aggregated total income using `SUMIF` functions across hours and days of the week.
* **Key Findings:**
  * **Peak Velocity:** Data revealed a sharp peak at **11:00 AM**. 
  * **Weekly Rhythm:** Sunday is the highest-grossing day, suggesting the bakery serves as a "weekend destination" rather than just a weekday commuter stop.
  * **Recommendation:** Align labor shifts to front-load staffing between 10:00 AM and 1:30 PM.
* **Visualizations:**
<p align="center">
  <img src="Total Revenue by Operating Hour (1,000s ₩).png" width="45%" /> 
  <img src="Weekly Revenue Distribution (1,000s ₩).png" width="45%"/>
</p>

### 📉 Product Popularity & Market Demand
* **Objective:** Determine the most popular food and beverage items to validate product-market fit.
* **Analysis:** Calculated total unit sales for all menu items and visualized distribution via bar charts.
* **Key Findings:**
    * **Angbutter** is the top-selling food item, significantly outperforming croissants.
    * **Americanos** are the most popular beverage choice, with a clear preference for hot drinks over cold ones.
* **Visualizations:**
<p align="center">
  <img src="Food Item Popularity.png" width="45%" /> 
  <img src="Beverage Popularity.png" width="45%"/>
</p
 
### 🔗 Hourly Sales Dynamics
* **Objective:** Analyze the relationship between food and drink sales to refine afternoon strategies.
* **Analysis:** Computed the proportion of food versus drink sales per hour to track consumption shifts.
* **Key Findings:**
    * Food items consistently make up approximately **90%** of total items sold.
    * **Sales Decay:** Food sales decrease significantly after the morning rush.
    * **Resilient Beverages:** Drink sales remain stable, peaking again at **2:00 PM** (The "Coffee Break" surge).
    * **Strategic Pivot:** The bakery should shift from a "Food Focus" in the morning to a "Beverage Focus" in the afternoon to capture higher margins.
* **Visualizations:**
<p align="center">
  <img src="Hourly Sales Volume.png" width="45%" /> 
  <img src="Product Mix Dynamics.png" width="45%"/>
</p
 
---

## 💡 Phase 4: Interpretation & Recommendations
Based on the analysis, I provided the following strategic roadmap to the stakeholders:

1.  **Inventory Optimization:** Prioritize Angbutter production and stock-up for the 11:00 AM rush to avoid stock-outs on the highest-margin item.
2.  **Labor Allocation:** Increase staffing for the Sunday peak and the 2:00 PM "Coffee Break" window to handle beverage demand.
3.  **Pivot Marketing:** Instead of a "Croissant-only" shop, use Croissants as a "Staple" draw while marketing Angbutter as the "Signature" driver
4.  **Bundle Strategies:** Launch "Americano + Angbutter" morning combos to capitalize on the 11 AM rush.

---

## 🛠️ Technical Skills Demonstrated
* **Advanced Formulas:** `SUMIF`, `COUNTIF`, and Absolute/Relative Cell Referencing for dynamic modeling.
* **Statistical Analysis:** Proportional Mix analysis and Time-Series segmentation.
* **Visualization:** 100% Stacked Bar Charts, Multi-variable Line Charts, and Executive Dashboards.
* **Frameworks:** Data Analysis Lifecycle, Rumsfeld Matrix, Scoping/Gap Analysis.


