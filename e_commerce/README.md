# 🛒 E-Commerce Sales & Profitability Analysis

An exploratory data analysis (EDA) project on a US-based e-commerce store's transactional data, built using Python. The project uncovers sales trends, profitability patterns, the impact of discounting, and regional performance — with actionable business recommendations.

---

## 📁 Dataset

**File:** `e_commerce_project_dataset.csv`  
**Source:** Superstore Sales Dataset (commonly used for retail analytics practice)  
**Size:** 9,994 rows × 21 columns

| Column | Description |
|---|---|
| Order ID / Customer ID | Unique identifiers |
| Order Date / Ship Date | Transaction and shipping timestamps |
| Ship Mode | Standard, Second, First Class, Same Day |
| Segment | Customer type — Consumer, Corporate, Home Office |
| Region / State / City | Geographic breakdown |
| Category / Sub-Category | Product classification (3 categories, 17 sub-categories) |
| Sales | Revenue per order line |
| Quantity | Units sold |
| Discount | Discount applied (0 to 0.8) |
| Profit | Net profit per order line |

---

## 🛠️ Tech Stack

- **Python**
- **Pandas** — data manipulation and aggregation
- **NumPy** — numerical operations
- **Matplotlib** — static charts
- **Seaborn** — statistical visualizations
- **Datetime** — date parsing and feature engineering

---
## 🔧 Preprocessing

* Parsed `Order Date` & `Ship Date` to `datetime`
* Confirmed zero nulls and zero duplicates
* Extracted `Order Year`, `Order Month`, `Order Day of Week`

---
## 📊 Analyses Performed

### 1. Monthly Sales Analysis
- Identified peak and low sales months across the year
- **November** is the highest sales month (₹352,461); **February** is the lowest (₹59,751)

### 2. Sales by Product Category
- Technology leads in total sales, followed closely by Furniture and Office Supplies
- All three categories are within a comparable range (~₹7–8.4L)

### 3. Sales by Sub-Category
- **Phones** (Technology) top all sub-categories in sales
- **Fasteners** (Office Supplies) are the lowest

### 4. Monthly Profit Analysis
- **December** is the most profitable month; **January** generates the least profit
- Profit trend does not perfectly mirror sales — margins vary by month

### 5. Profit by Category & Sub-Category
- **Technology** is the most profitable category; **Furniture** the least
- **Copiers** are the most profitable sub-category; **Tables** are loss-making

### 6. Customer Segment Analysis
- **Consumer** segment drives both the highest sales and highest profit
- **Home Office** segment is the smallest across both metrics

### 7. Sales-to-Profit Ratio by Segment
- Consumer segment has the highest ratio (8.66x), Home Office the lowest (7.13x)

### 8. Top 10 States by Average Profit
- Geographic breakdown to identify the most profitable states for the business

### 9. Discount vs Profit (Regression Analysis)
- Clear negative correlation between discount rate and profit
- Discounts above **20%** consistently produce **loss-making orders**

---

## 💡 Key Business Findings

| Finding | Insight |
|---|---|
| Discounts > 20% = losses | Average profit flips negative at medium–high discount bands |
| Furniture margin: only 2.49% | Technology and Office Supplies earn 17%+ margins |
| Tables & Bookcases are loss-making | Negative profit margin sub-categories despite decent sales |

### Business Recommendations
- **Cap discounts at 20%** across all categories; eliminate deep discounts (40%+) entirely
- **Review Furniture pricing**, especially Tables and Bookcases — every sale loses money
- **Focus marketing on the Consumer segment** — highest ROI per sales dollar

---
## 📉 Visualisations

Each analysis is backed by charts for clear interpretation:

- **Bar charts** — monthly sales & profit, category/sub-category comparisons, top 10 states by profit
- **Line plots** — sales and profit trends across months (with dot markers for profit trend)
- **Pie / Donut charts** — proportional share of sales, profit, and sales-to-profit ratio by category and segment
- **Grouped bar chart** — side-by-side sales and profit comparison across customer segments
- **Regression plot** — scatter plot with fitted regression line showing the negative relationship between discount rate and profit
---
## 🗂️ Project Structure

```

├── e_commerce_project_code.ipynb   # Main analysis notebook
├── e_commerce_project_dataset.csv  # Raw dataset
├── e_commerce_project_code.pdf     # Code file in pdf form
└── README.md
```

---

