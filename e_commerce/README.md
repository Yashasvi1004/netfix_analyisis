# 🛒 E-Commerce Sales & Profit Analysis

Exploratory data analysis on a US-based e-commerce store dataset using Python — covering sales, profit, customer segments, and product performance.

---

## 📁 Files

| File | Description |
|---|---|
| `e_commerce_project_code.ipynb` | Main analysis notebook |
| `e commerce project dataset.csv` | Source dataset (9,994 records, 21 columns) |

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|---|---|
| **Pandas** | Data loading, cleaning, groupby aggregations |
| **NumPy** | Numerical support |
| **Matplotlib** | Bar charts, pie charts, line plots |
| **Seaborn** | Styled bar plots, line plots with markers |
| **Jupyter Notebook** | Interactive analysis environment |

---

## 📊 Dataset Columns

`Row ID` · `Order ID` · `Order Date` · `Ship Date` · `Ship Mode` · `Customer ID` · `Customer Name` · `Segment` · `Country` · `City` · `State` · `Postal Code` · `Region` · `Product ID` · `Category` · `Sub-Category` · `Product Name` · `Sales` · `Quantity` · `Discount` · `Profit`

---

## 🔧 Preprocessing

- Parsed `Order Date` & `Ship Date` to `datetime`
- Confirmed zero nulls and zero duplicates
- Extracted `Order Year`, `Order Month`, `Order Day of Week`

---

## 📈 Key Findings

| # | Question | Finding |
|---|---|---|
| 1 | Monthly Sales | Highest: **November** ($352,461) · Lowest: **February** ($59,751) |
| 2 | Sales by Category | Highest: **Technology** · Lowest: **Office Supplies** |
| 3 | Sales by Sub-Category | Highest: **Phones** · Lowest: **Fasteners** |
| 4 | Monthly Profit | Highest: **December** · Lowest: **January** |
| 5 | Profit by Category | Highest: **Technology** · Lowest: **Furniture** |
| 6 | Profit by Sub-Category | Highest: **Copiers** · Lowest: **Tables** |
| 7 | Sales & Profit by Segment (incl. Ratio) | Sales & Profit — Highest: **Consumer** · Lowest: **Home Office** · Ratio — Consumer: 8.66 · Home Office: 7.13 |

---

## 📉 Visualizations

Each analysis is backed by charts for clear interpretation:
- **Line plots** — monthly sales and profit trends over the year
- **Bar charts** — category, sub-category, and segment comparisons
- **Pie / Donut charts** — proportional share of sales, profit, and sales-to-profit ratio by segment and category
