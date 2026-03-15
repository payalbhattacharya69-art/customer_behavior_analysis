# customer_behavior_analysis
data analysis project showcasing customer behavior analysis using python, sql and power Bi.

Here is a **simple, professional, recruiter-friendly README** you can use for your **Data Analytics Project**.

---

# Data Analytics Project

## Overview

This project demonstrates an **end-to-end data analytics workflow**. The goal is to extract meaningful insights from raw data using Python, SQL, and data visualization tools.

The project includes:

* Loading and analyzing data in Python
* Performing **Exploratory Data Analysis (EDA)**
* Cleaning and transforming data
* Writing SQL queries for analysis
* Building an **interactive dashboard in Microsoft Power BI Desktop**
* Creating a report and presentation using Gamma

This project showcases practical **data analytics skills used in real-world business scenarios**.

---

## Dataset

The dataset contains customer transaction information such as:

* Customer demographics
* Products purchased
* Purchase amounts
* Discounts applied
* Transaction dates

The dataset is used to analyze **sales trends, customer behavior, and revenue patterns**.

---

## Tools & Technologies

This project uses the following tools:

* **Programming:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Databases:** PostgreSQL / MySQL / Microsoft SQL Server
* **Visualization:** Microsoft Power BI Desktop
* **Presentation:** Gamma

---

## Project Workflow / Steps

### 1. Data Loading

The dataset is loaded into Python using Pandas.

Example:

```python
import pandas as pd

df = pd.read_csv("dataset.csv")
df.head()
```

---

### 2. Exploratory Data Analysis (EDA)

EDA helps understand the dataset and identify patterns.

Key steps:

* Checking dataset structure
* Summary statistics
* Identifying missing values
* Visualizing trends and distributions

Example:

```python
df.info()
df.describe()
```

---

### 3. Data Cleaning

Data cleaning ensures the dataset is accurate and ready for analysis.

Tasks performed:

* Handling missing values
* Removing duplicates
* Correcting data types
* Standardizing column names

---

### 4. SQL Data Analysis

The cleaned dataset is loaded into databases like:

* PostgreSQL
* MySQL
* Microsoft SQL Server

SQL queries are used to analyze:

* Total revenue
* Customer purchase patterns
* Discount rates
* Top products

Example SQL query:

```sql
SELECT item_purchased,
ROUND(100 * SUM(CASE WHEN discount_applied = 'yes' THEN 1 ELSE 0 END)/COUNT(*),2) AS discount_rate
FROM customer
GROUP BY item_purchased
ORDER BY discount_rate DESC;
```

---

## Dashboard

An interactive dashboard is built using **Microsoft Power BI Desktop**.

Dashboard features include:

* Total revenue overview
* Sales by product category
* Customer demographics
* Discount analysis
* Purchase trends over time

The dashboard allows users to **filter and explore insights interactively**.

---

## Results & Insights

Key insights from the analysis include:

* Identification of **top-selling products**
* Customer groups contributing the most revenue
* Impact of **discounts on sales**
* Trends in customer purchasing behavior

These insights help support **data-driven decision making**.

---

## Report & Presentation

The final insights are documented and presented through:

* Analytical report
* Business presentation created using Gamma

The presentation summarizes:

* Business problem
* Analysis performed
* Key insights
* Recommendations

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/data-analytics-project.git
```

### 2. Install required Python libraries

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Run the Python analysis script

```bash
python analysis.py
```

### 4. Load data into SQL database

Import the cleaned dataset into:

* PostgreSQL
* MySQL
* or Microsoft SQL Server

Run the SQL queries provided in the project.

### 5. Open the dashboard

Open the `.pbix` file using **Microsoft Power BI Desktop** to view the interactive dashboard.

---

## Project Outcome

This project demonstrates the complete **data analytics pipeline**:

**Data → Cleaning → Analysis → Visualization → Business Insights**

It highlights practical skills in **Python, SQL, and Power BI**, making it suitable for **data analyst portfolios and interviews**.

---

If you want, I can also help you create a **🔥 stronger “GitHub-ready” README that looks like a real Data Analyst portfolio project (with badges, images, folder structure, and screenshots).** That will impress recruiters much more.
