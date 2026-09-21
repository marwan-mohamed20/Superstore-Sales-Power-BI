# 📊 Superstore Commercial Performance & Operations Analytics (2016 – 2019)

> **An enterprise multi-page Business Intelligence dashboard analyzing $2.30M in revenue, profitability drivers, customer lifetime value, category distribution, and return behavior across the US retail market.**

---

## 📌 Executive Summary

This end-to-end Power BI analytics project evaluates the four-year commercial performance of a nationwide retail business (Superstore) between **2016 and 2019**. 

By tracking **\$2.30M** in revenue across **5K+ transactions** and **38K units sold**, the dashboard provides management with granular visibility into gross margins, customer segmentation, regional variances, and logistics challenges such as product return rates.

---

## 📈 Core Executive KPIs

| KPI Metric | Recorded Figure | Strategic Context |
| :--- | :--- | :--- |
| **Total Revenue (Sales)** | **\$2.30M** | Aggregate revenue across all categories and territories |
| **Total Net Profit** | **\$286.40K** | Net income generated across the 4-year lifecycle |
| **Overall Profit Margin** | **12.47%** | Healthy operational margin (~12.5%) |
| **Total Orders** | **5,000 (5K)** | Completed order lifecycles |
| **Total Units Sold** | **38,000 (38K)** | Total merchandise volume delivered |
| **Customer Base** | **793** | Unique active enterprise and retail accounts |
| **Returned Quantity** | **3,000 (3K)** | Units returned across 296 returned order incidents |

---

## 🖥️ Dashboard Architecture & Detailed Modules

The report is architected into 5 distinct operational views connected via custom UI sidebar navigation:

```
Superstore Analytics Suite
 ├── 🏠 Home Page (Executive Summary & YoY Trajectory)
 ├── 💰 Sales Dashboard (Macro Trends & City Rankings)
 ├── 📦 Category Dashboard (Margin Distribution & State Penetration)
 ├── 👥 Customer Insights (Segment Lifetime Value & Regional Margins)
 └── 🔄 Returns Dashboard (Reverse Logistics, Root-Cause Sub-Categories)
```

---

### 1. 🏠 Home Page (Executive Overview)
* **Objective:** High-level executive snapshot summarizing core business health and annual growth trajectory.
* **YoY Revenue Progression:**
  * **2016:** ~\$0.5M
  * **2017:** ~\$0.5M (Running total hits \$1.0M)
  * **2018:** ~\$0.6M (Running total hits \$1.6M)
  * **2019:** ~\$0.7M (Running total closes at **\$2.3M**)
* **Key Observations:** Consistent positive trajectory in annual billings, culminating in accelerated top-line performance in 2019.

---

### 2. 💰 Sales Dashboard
* **Running Cumulative Total:** Visualizes the smooth progression of revenue accumulating to the \$2.30M milestone by December.
* **Monthly Seasonality:** 
  * Strong seasonal spikes occurring in **March (\$0.21M)**, **September (\$0.31M)**, and annual peaks in **November (\$0.35M)** and **December (\$0.33M)**.
* **Category Contribution:**
  * **Technology:** **\$836.15K (36.4%)** *(Dominant revenue driver)*
  * **Furniture:** **\$742.00K (32.3%)**
  * **Office Supplies:** **\$719.05K (31.3%)**
* **Top 10 Performing Cities:**
  1. **New York City:** \$0.26M
  2. **Los Angeles:** \$0.18M
  3. **Seattle:** \$0.12M
  4. **San Francisco:** \$0.11M
  5. **Philadelphia:** \$0.11M
  *(Followed by Houston, Chicago, San Diego, Jacksonville, and Springfield).*

---

### 3. 📦 Category & Sub-Category Dashboard
* **Product Line Breakdown:**
  * **Top 5 Sub-Categories by Sales:** Phones (\$0.33M), Chairs (\$0.33M), Storage (\$0.22M), Tables (\$0.21M), and Binders (\$0.20M).
* **Order Volume by Category:**
  * **Office Supplies:** **4K orders (53.08%)** *(Highest volume)*
  * **Furniture:** **2K orders (25.02%)**
  * **Technology:** **2K orders (21.90%)**
* **Financial Matrix Analysis:**
  * **Technology** delivers the healthiest profit ratio, climbing to **34.85%** of total profits in 2019.
  * **Furniture** carries substantial margin erosion due to logistics and discounting, dropping its profit contribution to **16.36%** in 2019 despite holding nearly 30% of sales.

---

### 4. 👥 Customer Insights
* **Revenue by Target Segment:**
  * **Consumer:** **\$1.16M (44.95%)** | Net Profit: **\$0.13M**
  * **Corporate:** **\$706.15K (27.33%)** | Net Profit: **\$0.09M**
  * **Home Office:** **\$429.65K (16.63%)** | Net Profit: **\$0.06M**
* **Top Account Champions:**
  * **Sean Miller:** \$25K (Leading individual account)
  * **Tamara Chand:** \$19K
  * **Raymond Buch & Tom Ashbrook:** \$15K each
* **Cross-Regional Matrix Insights:**
  * The **West Region** is the company's powerhouse, accounting for **32.16%** of total orders and generating **37.86%** of total net profits.
  * The **Central Region** experiences compressed margins (Consumer segment margins sink to ~3.40%).

---

### 5. 🔄 Returns Dashboard (Reverse Logistics)
* **Scale of Returns:** **3K units** returned across **296 orders**.
* **Segment Vulnerability:**
  * **Consumer:** **52.87% (~2K units)**
  * **Corporate:** **32.23% (~1K units)**
  * **Home Office:** **14.90% (<0.5K units)**
* **Problematic Inventory Items:**
  * **Primary Category:** **Office Supplies**
  * **High Return Sub-Categories:** Binders (**558 units**), Paper (**453 units**), Furnishings (**277 units**).
* **Target Variance:** Current return run-rate stands at **184 units**, exceeding target expectations of 103.50 units (-77.78% variance).

---

## 💡 Strategic Recommendations

1. **Re-evaluate Furniture Pricing & Freight Contracts:**
   * Tables and Chairs contribute heavily to gross sales (\$0.54M combined) but drag down operational profit margins. Renegotiate bulk carrier shipping rates and curb extreme seasonal promotional discounts.
2. **Implement Return Prevention in High-Frequency Office Goods:**
   * Binders and Paper alone account for over 1,000 returned units. Audit packaging integrity and online product catalog descriptions to minimize ordering errors and transit damage.
3. **Double Down on Western Region Expansion:**
   * Because the West region produces ~38% of company profitability with top-tier profit margins (>13%), reallocate marketing and enterprise sales budgets to this territory.

---

## 🛠️ Data Architecture & Tech Stack

* **Tool:** Microsoft Power BI Desktop
* **Data Modeling:** Star Schema design connecting Sales Fact Table, Products Dimension, Customers Dimension, and Calendar Dimension.
* **Analytical Modeling:** DAX measures (Running Totals, YoY Variances, Margin %, Target Divergence).
* **UI/UX Design:** Custom warm-clay theme with unified card containers, KPI navigation bar, and conditional formatting heatmaps.