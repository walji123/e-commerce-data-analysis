# E-Commerce Sales Performance & Customer Behavior Analysis

A comprehensive exploratory data analysis (EDA) and business intelligence project conducted in Python (Google Colab) using `pandas`, `matplotlib`, and `seaborn`. This analysis investigates transaction records to uncover revenue drivers, customer purchasing habits, product performance, and actionable commercial opportunities.

---

## Project Overview

- **Environment:** Google Colab / Jupyter Notebook
- **Core Stack:** Python 3, Pandas, NumPy, Matplotlib, Seaborn
- **Objective:** Evaluate transaction-level e-commerce data to identify key factors influencing sales performance, customer segment value, and operational growth opportunities.

---

## Analysis Workflow & Structure

### 1. Dataset Understanding & Inspection
- Verified structure using `.head()`, `.tail()`, `.sample()`, `.info()`, and `.describe()`.
- Classified variables into identifiers, numerical values, categorical features, and datetime fields.

### 2. Data Cleaning & Preprocessing
- **Missing Data:** Quantified null counts and percentages; applied domain-justified imputation or removal strategies.
- **Deduplication:** Checked and handled repeated transaction records to preserve data integrity.
- **Standardization:** Normalized text fields (case formatting, trimming whitespace) and standardized categorical values and column headers.

### 3. Feature Engineering & Business Metrics
- Computed transaction revenue: $\text{Revenue} = \text{Quantity} \times \text{Price}$.
- Derived customer-level KPIs including **Average Order Value (AOV)**, **Revenue per Customer**, and **Order Frequency**.
- Calculated parametric and non-parametric summary statistics (mean, median, standard deviation, IQR).

### 4. Sales & Product Performance
- **Category Benchmarking:** Aggregated total revenue, sales volume, and transaction counts across categories.
- **Top 10 Product Ranking:** Identified and evaluated top-performing SKUs by volume and revenue contribution.
- **Time-Series Decomposition:** Extracted temporal components (month, day of week, hour) to diagnose peak purchasing windows.

### 5. Customer Behavior & Segmentation
- Identified high-value customers (top 10 by lifetime spend) vs. typical buyer distributions.
- Built multi-level aggregations and pivot tables to evaluate product cross-purchasing and category affinity across customer segments.

### 6. Payment & Geographic Insights
- Analyzed transaction share and revenue variance across payment methods.
- Assessed regional revenue contribution and top-selling categories by location.

### 7. Visualizations
1. **Bar Chart:** Category revenue breakdown & top 10 products.
2. **Distribution Plot:** Transaction value and customer spending distributions (skewness/outlier analysis).
3. **Time-Series Chart:** Monthly and day-of-week sales trendlines.
4. **Custom Chart:** Heatmap / Boxplot assessing multidimensional performance metrics.

---

## Key Findings & Strategic Recommendations

- **Top Insights:** Synthesized core revenue drivers, high-margin product categories, and temporal purchase spikes.
- **Business Recommendations:** Targeted inventory optimization, customer retention strategies for top-tier spenders, and preferred payment method promotions.
- **Methodological Reflection:** Summary of applied pandas techniques, data pipeline limitations, and proposed next steps (e.g., RFM segmentation, predictive CLV modeling).

---

## Repository Structure

```text
├── notebooks/
│   └── ecommerce_sales_analysis.ipynb   # Main Google Colab notebook
├── data/
│   └── E_commerce_dataset.csv          # Raw transaction dataset
├── visuals/                            # Exported charts and figures
└── README.md                           # Project documentation
