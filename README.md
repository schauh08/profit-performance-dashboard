# profit-performance-dashboard

README.md

Profit Performance Dashboard

An end-to-end interactive dashboard built in Power BI that visualizes profit trends, identifies top-performing categories and products, and enables filtering by region to view profit trends overtime.

Table of Contents

1. Project Overview

2. Features

3. Tech Stack

4. Repository Structure

5. Installation & Setup

6. Usage

7. File Descriptions

8. Authors

9. License

Project Overview

Objective: Provide executives with a comprehensive view of profit performance across time, product categories, and regions.

Data Source: Superstore dataset (~50K rows) containing order details, product information, and profit metrics.

Outcome: Interactive dashboard that reduced manual reporting effort and highlighted profit trends over time by region and key profit drivers by category and name.

Features

Trend analysis of profit over time (yearly/monthly/quarterly).

Top 3 profit-driving categories and top 5 products within each category.

Filtering by region, and product name.

Tech Stack

Data Cleaning & Modeling: Python (pandas, SQLAlchemy), SQLite

Dashboard & Visualization: Power BI Desktop (.pbix)

Version Control: Git & GitHub

Documentation: Markdown, Jupyter Notebooks

Repository Structure

profit-performance-dashboard/
├── data/
│   ├── raw/                   # Original Superstore CSV
│   └── processed/             # Cleaned CSV and exports (e.g., top3_by_profit.csv)
├── notebooks/                 # Jupyter notebooks for ETL, analysis, and SQL
│   ├── 01-inspection.ipynb    
│   ├── 02-table-creation.ipynb 
├── dashboard/                 # Final Power BI dashboard (.pbix)
├── reports/                   # Executive summary (.pdf)
├── sales-performance-dashboard.pbix  # Power BI dashboard file
├── requirements.txt           # Python dependencies
└── README.md

Installation & Setup

Clone the repository

git clone https://github.com/schauh08/profit-performance-dashboard.git
cd profit-performance-dashboard

Create & activate a virtual environment

python -m venv venv
source venv/bin/activate   # Mac/Linux
.\venv\Scripts\activate  # Windows PowerShell

Install dependencies:

pip install -r requirements.txt

Launch JupyterLab

jupyter lab

Usage

Run notebooks in order:

01-inspection.ipynb for data inspection, cleaning, and exporting superstore_clean.csv

02-table-creation.ipynb for building SQLite tables and exporting category_data.csv

Open profit-performance-dashboard.pbix in Power BI Desktop to explore the dashboard.

File Descriptions

data/raw/: Original downloaded Superstore CSV

data/processed/superstore_clean.csv: Cleaned and filtered dataset

data/processed/category_data.csv: Export of top-3 categories and top-5 products by profit

notebooks/: Step-by-step ETL and analysis

profit-performance-dashboard.pbix: Final interactive Power BI dashboard

reports/: One-page executive summary PDF

Authors:

Shaaf Chauhan – Data Analyst & Developer

License

Distributed under the MIT License.
