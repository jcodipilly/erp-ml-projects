# AI/ML Learning Portfolio

This repository documents my step-by-step journey into AI/ML and Deep Learning, starting with Python and Pandas foundations and progressing into ERP-flavored projects.

## 📂 Structure
- **Day 1 Setup** – Environment installation and test notebook
- **Day 2 Basics** – Python + Pandas warm-up exercises
- **ERP Projects** – Realistic datasets (orders, invoices, shipments) applied to ML models
- **Deep Learning** – Intro notebooks with Keras/PyTorch

## 🎯 Goals
- Build strong foundations in Python, Pandas, and scikit-learn
- Apply ML concepts to ERP-style datasets
- Document each step clearly for learning and portfolio purposes
- Transition into deep learning and MLOps practices

## 🚀 How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/jcodipilly/erp-ml-projects.git
2. Open notebooks in Jupyter or VS Code.
3. Follow along with documented steps and examples.   

✨ Notes
All notebooks are self-contained and include explanations in Markdown cells.
Datasets are either synthetic (ERP-style) or public open datasets.
This repo is part of my continuous learning journey into AI/ML and system architecture.

📊 ERP-Style Data Analysis with Pandas
This section tracks my ERP-style learning journey using Python and Pandas, with synthetic datasets for Orders, Invoices, and Shipping. Each day builds on the last, adding new logic and insights.

📅 Day 1: Setup
Created sample datasets for Orders and Invoices
Practiced basic DataFrame creation and display

📅 Day 2: Sorting, Filtering, Grouping
Techniques:
Sort by Amount
Filter by Status = Pending
Group by Customer (sum of Amount)
Add new Discount column
Key Learning: .groupby() + .reset_index() for clean summaries

📅 Day 3: Orders + Invoices Merge
Merged Orders and Invoices on OrderID using pd.merge()
Handled missing values (NaN, NaT)
Identified incomplete records (missing ShipDate or InvoiceDate)
Key Learning: SQL-style joins with Pandas

📅 Day 4: Shipping Delays & Discounts
Calculated shipping delay using .dt.days
Flagged late shipments (> 5 days)
Grouped late shipments by Customer
Applied 10% discount for late deliveries
Summarized discounts by Customer
Filtered unpaid invoices
Key Learning: Conditional logic with .apply() and datetime handling

📊 Day 5: Visualizing Shipping Delays, Discounts, and Invoices
This notebook demonstrates how visualizations can turn ERP-style data into actionable insights. Using the merged Orders + Invoices dataset (merged_df), I explore fulfillment performance, customer impact, and financial health through three key charts:

🔹 Shipping Delay Distribution
Histogram showing how quickly orders are shipped
Late shipments flagged at >2 days (adjustable threshold)
Highlights fulfillment bottlenecks

🔹 Discounts by Customer
Bar chart of total discounts applied due to late shipments
Reveals which customers were most impacted
Validates business logic for conditional discounts

🔹 Paid vs Unpaid Invoices
Pie chart showing proportion of paid vs unpaid invoices
Snapshot of financial health and outstanding liabilities

Each chart is followed by a Markdown explanation to guide the reader through the logic and insights. This milestone sets the stage for predictive analysis in future steps (e.g., forecasting late shipments or payment delays).
