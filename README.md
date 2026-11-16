# Exploratory Data Analysis (EDA) — Sample Superstore Dataset

## Project Overview
This project performs Exploratory Data Analysis (EDA) on the **Sample Superstore Dataset** as part of the **Veda Technology Data Analytics Track**. The goal is to explore the dataset visually and statistically to uncover hidden patterns, seasonal trends, discount impacts, and profitability outliers before drawing business conclusions.

## Tools & Technologies Used
* **Python**
* **Pandas & NumPy** — Data loading, date formatting, missing/duplicate checks, and summary statistics
* **Matplotlib & Seaborn** — Statistical charts and visual exploration
* **Google Colab / Jupyter Notebook** — Interactive analysis and documentation

## Approach & Methodology
1. **Data Preparation & Summary Statistics:** 
   * Loaded the `Sample - Superstore.csv` dataset and converted `Order Date` into datetime format to enable monthly time-series tracking.
   * Verified data cleanliness by checking for missing values and duplicate records.
   * Generated descriptive statistics (`.describe()`) across `Sales`, `Quantity`, `Discount`, and `Profit`.

2. **Visual & Statistical Exploration:**
   * **Correlation Heatmap:** Examined linear relationships between numerical metrics (`Sales`, `Quantity`, `Discount`, and `Profit`).
   * **Discount Distribution Histogram:** Analyzed how frequently different discount rates are applied across customer orders.
   * **Category Profit Boxplot:** Identified interquartile spreads and extreme profit/loss outliers across `Furniture`, `Office Supplies`, and `Technology`.
   * **Monthly Sales vs. Profit Line Chart:** Tracked multi-year revenue and profit performance across months to identify seasonality.
   * **Discount vs. Profit Line Plot by Category:** Pinpointed the exact discount thresholds where product categories become unprofitable.

## Key Outcomes (Top 3 Insights)
1. **Discounts Above 20% Destroy Profitability:** Orders with 0% to 20% discounts maintain healthy positive margins, whereas discounts of 30% or higher push average order profit into negative territory across all categories—most severely in Furniture and Technology.
2. **Strong Q4 Seasonality Drives Annual Revenue:** Sales consistently surge between September and December each year (driven by back-to-school and holiday demand) before dropping sharply in January and February. Inventory and promotional budgets should be weighted toward Q4.
3. **Technology Drives High Upside, Furniture Needs Margin Review:** Technology generates the highest positive profit outliers and scales effectively, while Furniture suffers from frequent negative outliers and razor-thin median margins, highlighting a need to audit shipping costs and cap discounts on bulky items.

## Repository Contents
* `Superstore_EDA.ipynb` — Complete Jupyter Notebook containing Python code, summary statistics, 5 visualizations, observations, and final insights.
* `Sample - Superstore.csv` — Raw dataset used for the analysis.
* `README.md` — Project documentation summarizing the objective, approach, and key findings.
