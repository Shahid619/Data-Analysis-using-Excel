

## 🛒 Superstore Sales Analysis

### 📘 Overview

This project analyzes the **Superstore Sales Dataset** from Kaggle to uncover insights about sales performance, profitability, customer segments, and product trends across regions.

The main goal is to understand **what drives profit**, **where losses occur**, and **how factors like discounts, ship modes, and time affect business performance**.

---

### 📂 Dataset Information

* **Source:** [Superstore Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
* **Rows:** ~6k+ orders
* **Columns:** Order ID, Order Date, Ship Date, Region, Segment, Category, Sub-Category, Product Name, Sales, , Ship Mode, etc.
* **Time Period:** Multi-year sales record (2015 - 2020 approx.)

---

### 🧮 Tools Used

* **Microsoft Excel**

  * Data cleaning (fixing dates, removing duplicates)
  * Pivot tables for grouping and aggregation
  * Functions: `SUMIF`, `AVERAGEIF`, `MONTH`, `YEAR`, `IF`
  * Charts: Column, Line, Pie, and Scatter plots

---

## 📊 Analysis Summary

### 🧾 **1. Sales & Profit Overview**

* **Total Sales:** (sum of all sales values)
* **Total Profit:** (sum of all profit values)
* **Insight:** The store generates strong overall sales, but profit varies across categories.
* **Top Categories:** *Technology* and *Office Supplies* perform best in both sales and profit.
* **Observation:** Some sub-categories, despite high sales (like Furniture), yield lower profits due to heavy discounts or shipping costs.

---

### 🌍 **2. Regional & Segment Analysis**

* **Highest Revenue Region:** The *West* region brings the most revenue.
* **Top Segment:** *Consumer* and *Corporate* segments lead in both sales and profit.
* **Loss-making Regions:** A few *Central* region entries show negative profit — possibly due to higher discounting or delivery cost.
* **Conclusion:** Focus marketing and inventory toward West and South regions for better ROI.

---

### 💸 **3. Discount Impact**

* **Finding:** Higher discounts do **not always lead to higher sales** — often they reduce profit margins.
* **Correlation:** Negative correlation between *discount* and *profit* → more discount = less profit.
* **Visual:** A scatter plot (Discount vs Profit) clearly shows profit dropping as discount rises.
* **Business Insight:** Discounts should be more targeted — only for underperforming items, not across all categories.

---

### 📅 **4. Time-based Trends**

* **Trend Analysis:**

  * Sales increase toward the **end of each year**, possibly due to holiday season spikes.
  * Profits follow a similar pattern but with sharper dips in discount-heavy months.
* **Tools Used:**

  * Extracted *Month* and *Year* using Excel’s `=MONTH()` and `=YEAR()` functions.
  * Created a *Line Chart* to visualize month-over-month change.
* **Insight:** The business is seasonal — strong in Q4 each year.

---

### 🏆 **5. Top Performing Products**

* **Most Profitable Products:** A few technology and office supply items (like printers and accessories) contribute heavily to total profit.
* **Method:** Pivot Table → Rows = Product Name → Values = Sum of Profit → Sorted descending.
* **Insight:** These top items are the company’s core drivers; they should be prioritized for stock and marketing.

---

### 🚚 **6. Shipping & Delivery Analysis**

* **Ship Mode Effect:**

  * *Standard Class* is used most frequently and generates consistent sales.
  * *Same Day* mode is faster but adds cost — sometimes reducing profit.
* **Delivery Time Check:**

  * Calculated using: `=Ship Date - Order Date`
  * Longer delivery time doesn’t necessarily reduce sales, but fast shipping helps customer satisfaction.
* **Insight:** The company should balance cost and delivery speed for better efficiency.

---

## 💡 Key Business Insights

1. **Technology** and **Office Supplies** are the top-performing categories.
2. The **West Region** and **Consumer Segment** generate the most revenue.
3. **Discounts** reduce profit — avoid over-discounting.
4. **End-of-year months** bring the highest sales and profits.
5. A few **high-profit products** drive most of the revenue — focus on these.
6. **Same Day shipping** adds speed but reduces margin — optimize logistics.

---

## 📈 Visualization Ideas

To make your findings stand out, you can add these charts in Excel:

* Bar Chart → *Top 10 Products by Profit*
* Line Chart → *Monthly Sales and Profit Trends*
* Pie Chart → *Sales Share by Region*
* Scatter Plot → *Discount vs Profit*

---

## 🧰 Project Files

| File                       | Description                        |
| -------------------------- | ---------------------------------- |
| `superstore_sales_raw.csv` | Original dataset from Kaggle       |
| `superstore_cleaned.xlsx`  | Cleaned and formatted data         |
| `superstore_cleaned.xlsx` | Pivot tables, formulas, and charts |
| `README.md`                | Project summary and insights       |

---

## 🧑‍💻 Conclusion

This project demonstrates how data analytics can turn raw retail data into **clear business insights** using simple Excel tools.

Even without advanced coding, understanding *how sales, discounts, and regions interact* provides huge value in making data-driven decisions.


