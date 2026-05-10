# E-Commerce Sales Analysis
### Exploratory Data Analysis on Brazilian E-Commerce Public Dataset (Olist)

---

## Overview

This project presents a comprehensive exploratory data analysis of a real-world e-commerce dataset containing over 100,000 orders placed between 2016 and 2018 on the Olist platform — one of Brazil's largest e-commerce marketplaces.

The analysis covers the full data analyst workflow: data cleaning, transformation, exploratory analysis, and business insight generation through structured visualizations.

---

## Objectives

- Identify sales trends and seasonal patterns across a two-year period
- Analyze product category performance and revenue contribution
- Examine customer geographic distribution and purchasing behavior
- Evaluate order delivery performance and customer satisfaction scores
- Surface actionable business insights from raw transactional data

---

## Dataset

**Source:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

| File | Description | Rows |
|---|---|---|
| olist_orders_dataset.csv | Order status and timestamps | 99,441 |
| olist_order_items_dataset.csv | Items per order, price, freight | 112,650 |
| olist_products_dataset.csv | Product categories and dimensions | 32,951 |
| olist_customers_dataset.csv | Customer location data | 99,441 |
| olist_order_reviews_dataset.csv | Customer review scores | 100,000+ |

---

## Project Structure

```
ecommerce-sales-analysis/
│
├── data/
│   ├── raw/                  # Original downloaded datasets
│   └── processed/            # Cleaned and merged datasets
│
├── notebooks/
│   └── ecommerce_analysis.ipynb   # Main analysis notebook
│
├── images/
│   └── ...                   # Exported visualization outputs
│
├── requirements.txt          # Python dependencies
└── README.md
```

---

## Analysis Workflow

```
Data Loading  →  Data Cleaning  →  Feature Engineering  →  EDA  →  Visualization  →  Insights
```

**1. Data Cleaning**
- Handle missing values across all tables
- Standardize date formats and data types
- Remove duplicate records
- Merge multiple tables into a unified analytical dataset

**2. Feature Engineering**
- Extract time-based features: year, month, day of week, hour
- Calculate delivery duration (order to delivery)
- Compute revenue per order

**3. Exploratory Data Analysis**
- Monthly and yearly revenue trends
- Top-performing product categories by revenue and volume
- Customer distribution by state
- Delivery performance analysis
- Review score distribution and correlation with delivery time

**4. Visualization**
- Time series revenue chart
- Category revenue bar chart (horizontal)
- Geographic heatmap by state
- Delivery time distribution
- Correlation heatmap

---

## Key Findings

> Full findings are documented inside the notebook.

- Peak sales consistently occur in Q4, with November showing the highest single-month revenue
- Health & Beauty and Watches & Gifts are the top two revenue-generating categories
- 93% of orders are delivered before the estimated delivery date
- Lower review scores are strongly correlated with delayed deliveries
- Sao Paulo accounts for approximately 42% of total orders

---

## Tools & Libraries

| Tool | Purpose |
|---|---|
| Python 3.10+ | Core programming language |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical computation |
| Matplotlib | Base visualization layer |
| Seaborn | Statistical visualizations |
| Jupyter / Google Colab | Interactive development environment |

---

## How to Run

**Option 1 — Google Colab (Recommended)**

1. Open the notebook directly in Colab:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)
2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
3. Upload to Colab and run all cells

**Option 2 — Local (VS Code)**

```bash
git clone https://github.com/andremusari276-coder/ecommerce-sales-analysis.git
cd ecommerce-sales-analysis
pip install -r requirements.txt
jupyter notebook notebooks/ecommerce_analysis.ipynb
```

---

## Requirements

```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
jupyter>=1.0.0
```

---

## Author

**Andre Musari**  
Data Science Student — Semester 2  
[GitHub](https://github.com/andremusari276-coder) · [LinkedIn](https://linkedin.com/in/andr0031) · [Kaggle](https://kaggle.com/andremusari)

---

*This project is part of an ongoing data science portfolio. Dataset is publicly available under CC BY-NC-SA 4.0 license.*
