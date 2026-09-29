# 🛍️ Customer Shopping Trends Data Analysis — SQL, Python & Power BI

## 📌 Project Overview

This project is an **end-to-end Data Analytics portfolio project** focused on analyzing customer shopping behavior and retail sales data.

The objective is to transform raw customer transaction data into **meaningful business insights** using **SQL, Python, and Power BI**. The project covers the complete data analytics workflow — from data cleaning and exploratory analysis to SQL-based business analysis and interactive dashboard development.

The analysis helps understand **customer purchasing patterns, sales performance, product preferences, customer demographics, subscription behavior, discounts, shipping methods, and overall shopping trends**.

This project demonstrates practical skills required for a **Data Analyst / Business Analyst / BI Analyst** role, including data cleaning, data exploration, SQL querying, visualization, KPI development, and business insight generation.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Analyze customer shopping behavior and purchasing patterns.
* Clean and prepare raw retail data for analysis.
* Identify important customer and product trends.
* Analyze sales performance across different categories.
* Understand customer demographics and their relationship with purchasing behavior.
* Analyze the impact of discounts on purchasing decisions.
* Compare different shipping methods and their usage.
* Analyze customer subscription behavior.
* Identify frequently purchased products and high-performing categories.
* Create meaningful business KPIs.
* Build an interactive Power BI dashboard.
* Generate actionable insights that can support business decision-making.

---

## 🗂️ Dataset

The dataset contains customer shopping transaction information from a retail environment.

### Key Attributes

Some of the major fields used in the analysis include:

| Column                 | Description                                       |
| ---------------------- | ------------------------------------------------- |
| Customer ID            | Unique identifier for each customer               |
| Age                    | Age of the customer                               |
| Gender                 | Gender of the customer                            |
| Item Purchased         | Product purchased by the customer                 |
| Category               | Product category                                  |
| Purchase Amount        | Amount spent on the transaction                   |
| Location               | Customer location                                 |
| Size                   | Size of the purchased product                     |
| Color                  | Product color                                     |
| Season                 | Season during which the purchase was made         |
| Review Rating          | Customer rating for the purchased product         |
| Subscription Status    | Whether the customer has a subscription           |
| Payment Method         | Payment method used                               |
| Shipping Type          | Shipping method selected                          |
| Discount Applied       | Whether a discount was applied                    |
| Promo Code Used        | Whether a promotional code was used               |
| Previous Purchases     | Number of previous purchases made by the customer |
| Frequency of Purchases | Customer purchase frequency                       |

---

# 🔄 Project Workflow

The project follows a complete data analytics pipeline:

```text
Raw Dataset
     ↓
Data Understanding
     ↓
Data Cleaning & Preprocessing
     ↓
Exploratory Data Analysis
     ↓
SQL Data Analysis
     ↓
Business Questions
     ↓
Power BI Data Modeling
     ↓
Dashboard & Visualization
     ↓
Business Insights
     ↓
Recommendations
```

---

# 🐍 1. Data Analysis Using Python

Python was used for **data cleaning, preprocessing, exploratory data analysis (EDA), and statistical analysis**.

### Libraries Used

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

### Data Cleaning

The following data preparation tasks were performed:

* Loaded the raw dataset using Pandas.
* Inspected dataset structure and data types.
* Checked for missing values.
* Identified duplicate records.
* Checked unique values in categorical columns.
* Corrected inconsistent data formats.
* Converted columns to appropriate data types.
* Created derived columns where required.
* Prepared the cleaned dataset for SQL and Power BI analysis.

### Exploratory Data Analysis

The Python analysis explored:

* Customer demographics
* Product categories
* Purchase amounts
* Seasonal purchasing behavior
* Customer ratings
* Discount usage
* Subscription status
* Payment methods
* Shipping preferences
* Purchase frequency
* Customer purchasing patterns

### Example Python Analysis

```python
import pandas as pd

df = pd.read_csv("shopping_trends.csv")

# Dataset overview
print(df.head())
print(df.info())

# Check missing values
print(df.isnull().sum())

# Check duplicate records
print(df.duplicated().sum())

# Category analysis
print(df["Category"].value_counts())

# Average purchase amount by category
category_sales = df.groupby("Category")["Purchase Amount"].mean()

print(category_sales)
```

---

# 🗄️ 2. SQL Data Analysis

SQL was used to perform structured analysis and answer important **business questions** from the cleaned dataset.

The SQL analysis focuses on aggregation, filtering, grouping, sorting, conditional logic, and analytical queries.

### SQL Concepts Used

* `SELECT`
* `WHERE`
* `GROUP BY`
* `ORDER BY`
* `HAVING`
* `CASE`
* Aggregate functions
* `COUNT()`
* `SUM()`
* `AVG()`
* `MIN()`
* `MAX()`
* Subqueries
* Common Table Expressions (CTEs)
* Window Functions
* Joins

---

## 📊 Business Questions Answered Using SQL

Some of the key business questions include:

### Customer Analysis

1. How many customers are present in the dataset?
2. What is the average customer age?
3. What is the distribution of customers by gender?
4. Which locations have the highest number of customers?
5. Which customers have made the highest number of previous purchases?

### Product Analysis

6. Which products are purchased most frequently?
7. Which product categories generate the highest sales?
8. What is the average purchase amount for each category?
9. Which products have the highest average ratings?
10. Which products have the highest purchase frequency?

### Sales Analysis

11. What is the total purchase amount?
12. What is the average transaction value?
13. Which categories have the highest revenue?
14. How does purchase amount vary across seasons?
15. Which locations generate the highest sales?

### Discount & Promotion Analysis

16. How many customers used discounts?
17. What percentage of purchases involved a discount?
18. How does the average purchase amount differ between discounted and non-discounted purchases?
19. How many customers used promotional codes?
20. What products are most frequently purchased using promotions?

### Subscription Analysis

21. How many customers have an active subscription?
22. Do subscribed customers spend more than non-subscribed customers?
23. What is the average purchase amount for subscribers vs. non-subscribers?
24. Which categories are most popular among subscribers?

### Shipping & Payment Analysis

25. Which shipping method is most commonly selected?
26. Which payment method is most frequently used?
27. What is the average purchase amount for different payment methods?
28. Which shipping methods are associated with higher-value purchases?

---

# 📈 3. Power BI Dashboard

Power BI was used to create an **interactive business intelligence dashboard** that summarizes the major findings from the analysis.

The dashboard allows users to explore customer shopping behavior through interactive visualizations and filters.

## 📌 Key KPIs

The dashboard includes important KPIs such as:

* **Total Customers**
* **Total Sales**
* **Average Purchase Amount**
* **Average Customer Rating**
* **Total Purchases**
* **Subscription Rate**
* **Discount Usage Rate**
* **Average Customer Age**

---

## 📊 Dashboard Visualizations

The dashboard contains visualizations such as:

### Customer Demographics

* Customers by Gender
* Customers by Age Group
* Customers by Location

### Sales Analysis

* Sales by Product Category
* Sales by Season
* Average Purchase Amount by Category
* Sales Distribution

### Product Analysis

* Top Purchased Products
* Product Category Performance
* Product Ratings

### Customer Behavior

* Purchase Frequency
* Previous Purchases
* Subscription Status
* Discount Usage

### Payment & Shipping

* Payment Method Distribution
* Shipping Method Distribution
* Purchase Amount by Payment Method

---

# 🎛️ Interactive Filters

The Power BI dashboard provides interactive slicers/filters for:

* Gender
* Age Group
* Category
* Location
* Season
* Subscription Status
* Discount Status
* Payment Method
* Shipping Type

Users can select different combinations of filters to analyze specific customer segments.

---

# 🔍 Key Business Insights

The analysis is designed to identify insights such as:

* Which product categories contribute most to overall sales.
* Which customer segments make more purchases.
* Differences in purchasing behavior between subscribed and non-subscribed customers.
* The relationship between discounts and purchase behavior.
* The most frequently used payment methods.
* Customer preferences for different shipping methods.
* Seasonal changes in customer purchasing patterns.
* Products and categories with stronger customer ratings.
* Locations with higher customer activity.
* Differences in spending behavior across customer segments.

> **Note:** Specific numerical findings are available in the SQL analysis and Power BI dashboard.

---

# 💡 Business Recommendations

Based on the analysis, businesses can use the findings to:

* Develop targeted marketing campaigns for high-value customer segments.
* Improve customer retention through subscription programs.
* Optimize discount and promotional strategies.
* Focus inventory on high-performing products and categories.
* Develop seasonal marketing campaigns.
* Improve personalized product recommendations.
* Optimize shipping options based on customer preferences.
* Identify opportunities for increasing customer lifetime value.
* Use customer ratings to improve product offerings.

---

# 🛠️ Tools & Technologies

| Tool                 | Purpose                                 |
| -------------------- | --------------------------------------- |
| **Python**           | Data cleaning, preprocessing & EDA      |
| **Pandas**           | Data manipulation                       |
| **NumPy**            | Numerical analysis                      |
| **Matplotlib**       | Data visualization                      |
| **Seaborn**          | Statistical visualization               |
| **SQL**              | Business analysis & querying            |
| **Power BI**         | Dashboard & interactive visualization   |
| **Jupyter Notebook** | Python analysis environment             |
| **Git & GitHub**     | Version control & project documentation |

---

# 📁 Project Structure

```text
customer-trends-data-analysis/
│
├── 📂 data/
│   ├── shopping_trends.csv
│   └── cleaned_shopping_trends.csv
│
├── 📂 python/
│   └── customer_trends_analysis.ipynb
│
├── 📂 sql/
│   └── customer_trends_analysis.sql
│
├── 📂 powerbi/
│   └── customer_shopping_trends.pbix
│
├── 📂 dashboard/
│   └── dashboard_screenshot.png
│
├── 📂 reports/
│   └── analysis_report.pdf
│
└── README.md
```

---

# 🚀 End-to-End Implementation

The project can be reproduced using the following steps:

### Step 1 — Clone the Repository

```bash
git clone https://github.com/your-username/customer-trends-data-analysis.git
```

### Step 2 — Install Python Libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Step 3 — Run the Python Notebook

Open:

```text
python/customer_trends_analysis.ipynb
```

Run the notebook to perform:

```text
Data Loading
     ↓
Data Cleaning
     ↓
EDA
     ↓
Data Visualization
     ↓
Export Clean Dataset
```

### Step 4 — Run SQL Queries

Import the cleaned dataset into your preferred SQL database and execute:

```text
sql/customer_trends_analysis.sql
```

### Step 5 — Open Power BI

Open:

```text
powerbi/customer_shopping_trends.pbix
```

Refresh the dataset and interact with the dashboard.

---

# 📊 Skills Demonstrated

This project demonstrates practical experience in:

### Data Analytics

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis
* Statistical Analysis
* Data Interpretation
* Business Analysis

### SQL

* Data Aggregation
* Filtering
* Grouping
* Conditional Analysis
* Subqueries
* CTEs
* Window Functions
* Business Query Development

### Python

* Pandas
* NumPy
* Data Manipulation
* Data Visualization
* Exploratory Data Analysis

### Power BI

* Dashboard Development
* KPI Creation
* Interactive Filters
* Data Visualization
* Business Intelligence
* Data Storytelling

### Business Skills

* Problem Solving
* Analytical Thinking
* Business Insight Generation
* Data-Driven Decision Making
* Reporting & Visualization

---

# 🎓 What I Learned

Through this project, I gained practical experience in building a complete analytics solution from raw data to business insights.

The project helped strengthen my understanding of:

* How to work with real-world retail datasets.
* How to clean and prepare data for analysis.
* How to use Python for exploratory data analysis.
* How to write SQL queries to solve business problems.
* How to transform analytical results into meaningful KPIs.
* How to build interactive dashboards using Power BI.
* How to communicate data-driven insights to business stakeholders.
* How different tools can be combined into an end-to-end data analytics workflow.

---

# 🔮 Future Improvements

Possible future enhancements include:

* Customer segmentation using **RFM Analysis**.
* Customer clustering using **Machine Learning**.
* Customer lifetime value prediction.
* Sales forecasting.
* Churn prediction.
* Recommendation systems.
* Automated Power BI data refresh.
* Advanced DAX measures.
* Deployment of the dashboard through Power BI Service.
* Automated ETL pipeline for regularly updated retail data.

---

# 👩‍💻 Author

**Sakshi**

Aspiring **Data Analyst | Data Scientist | AI/ML Engineer**

### Technical Interests

* Data Analytics
* SQL
* Python
* Power BI
* Machine Learning
* Artificial Intelligence
* Data Visualization
* Business Intelligence

---

## ⭐ If You Find This Project Useful

If this project helped you understand an end-to-end data analytics workflow, consider giving the repository a ⭐ **Star** and exploring the other projects in the repository.

---

## 📌 Project Summary

**Customer Shopping Trends Data Analysis** is an end-to-end retail analytics project that combines **Python, SQL, and Power BI** to transform raw customer transaction data into actionable business insights.

The project demonstrates the complete journey:

**Raw Data → Cleaning → EDA → SQL Analysis → KPI Development → Power BI Dashboard → Business Insights → Recommendations**

