# 🍕 FoodiePK — Lahore Food Delivery Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green?style=flat&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-1.24-orange?style=flat&logo=numpy)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat)

> **Exploratory Data Analysis (EDA)** on a simulated food delivery dataset inspired by Lahore's food scene.  
> Analyzed **2,000 orders** across **15 restaurants**, **10 areas**, and **10 food categories** using Python, Pandas & NumPy.

---

## 📁 Project Structure

```
FoodiePK-Analysis/
│
├── lahore_foodie_data.csv       # Raw dataset (2000 orders)
├── FoodiePK_Analysis.ipynb      # Main analysis notebook
└── README.md                    # Project documentation
```

---

## 📊 Dataset Overview

| Feature | Details |
|---------|---------|
| 📦 Total Orders | 2,000 |
| 🏙️ City | Lahore |
| 🏘️ Areas Covered | Gulberg, DHA, Johar Town, Model Town, Bahria Town & more |
| 🍽️ Restaurants | 15 popular Lahore restaurants |
| 🗓️ Time Period | Jan – Dec (Full Year) |
| 💰 Currency | PKR (Pakistani Rupee) |

### Columns

| Column | Description |
|--------|-------------|
| `Order_ID` | Unique order identifier |
| `Month` | Month of order |
| `City` | City (Lahore) |
| `Area` | Delivery area |
| `Restaurant` | Restaurant name |
| `Food_Category` | Biryani, Karahi, BBQ, Burger, Pizza, etc. |
| `Item_Name` | Specific menu item |
| `Quantity` | Number of items |
| `Unit_Price` | Price per item (PKR) |
| `Discount` | Discount applied (0–20%) |
| `Delivery_Fee` | Delivery charges |
| `Subtotal` | Price × Quantity |
| `Total_Amount` | Final bill amount |
| `Cost` | Restaurant's cost |
| `Profit` | Net profit per order |
| `Meal_Time` | Breakfast / Lunch / Dinner / Late Night |
| `Order_Status` | Delivered / Cancelled |
| `Payment_Method` | JazzCash / EasyPaisa / COD / Card |
| `Rating` | Customer rating (3.0–5.0 ⭐) |

---

## 🔍 Analysis Performed

### Step 1 — Data Loading
- Loaded CSV using Pandas
- Previewed data with `head()`, `shape`, `dtypes`

### Step 2 — Data Cleaning
- Checked missing values → `isnull().sum()`
- Checked duplicates → `duplicated().sum()`
- Rating nulls are valid (Cancelled orders have no rating)

### Step 3 — Basic KPIs
- Total Orders, Total Sales, Total Profit
- Average Order Value
- Overall Profit Margin %

### Step 4 — Food Category Analysis
- Orders per category
- Most & least profitable category
- Average order value per category

### Step 5 — Restaurant Analysis
- Top 5 by Sales, Profit & Rating

### Step 6 — Monthly Trend
- Orders & profit month-by-month
- Best performing month

### Step 7 — Meal Time Analysis
- Peak order times
- Late Night food preferences

### Step 8 — Payment Method Analysis
- Most popular payment methods
- Profit by payment method

### Step 9 — Cancelled Orders
- Cancellation rate %
- Cancellations by category & area

### Step 10 — Discount Impact
- Correlation between discount & profit
- Average profit at high discount levels

### Step 11 — Rating Analysis
- Best & worst rated restaurants
- Correlation between rating & profit

### Step 12 — Area-wise Performance
- Most orders by area
- Most profitable areas
- Highest average order value areas

---

## 💡 Key Insights

| # | Insight | Finding |
|---|---------|---------|
| 1 | 🍖 Most Profitable Category | **BBQ** generates highest profit |
| 2 | 🏪 Top Restaurant | **Charcoal Grill** — highest sales & profit |
| 3 | 📅 Best Month | **December** — peak sales & orders |
| 4 | 🌙 Late Night Favourite | **Burger** most ordered late night |
| 5 | 💳 Top Payment Method | **JazzCash** most popular & profitable |
| 6 | ❌ Most Cancellations | **Shawarma** category & **DHA** area |
| 7 | 🏷️ Discount Impact | Negative correlation — more discount = less profit |
| 8 | ⭐ Best Rated Restaurant | **Charcoal Grill** — highest avg rating |
| 9 | 🏘️ Best Area | **Bahria Town** — most orders & profit |
| 10 | 📊 Overall Profit Margin | **~42.5%** |

---

## 🛠️ Tools & Libraries

```python
import pandas as pd    # Data manipulation & analysis
import numpy as np     # Numerical operations
```

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/yourusername/FoodiePK-Analysis.git
cd FoodiePK-Analysis
```

2. Install dependencies
```bash
pip install pandas numpy jupyter
```

3. Launch Jupyter Notebook
```bash
jupyter notebook FoodiePK_Analysis.ipynb
```

---

## 👨‍💻 Author

**Hadeed Malik**  
📧 hadeedmalik503@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/hadeed-malik-28b11731b/) | [GitHub](https://github.com/hadeed101)

---

*This project was built for Data Analysis practice using real-world inspired Pakistani food delivery data.*
