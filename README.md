# Customer Shopping Behavior Analysis

## Overview
This project focuses on analyzing customer shopping behavior to identify purchasing patterns, revenue trends, product preferences, discount usage, and customer loyalty. It follows an end-to-end data analytics workflow using Python, PostgreSQL, and Power BI to transform raw data into meaningful business insights.

## Dataset
- **Dataset:** `customer_shopping_behavior.csv`
- **Total Records:** 3,900
- **Original Columns:** 18
- **Key Attributes:** Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount, Location, Review Rating, Subscription Status, Shipping Type, Discount Applied, Previous Purchases, Payment Method, and Purchase Frequency.

## Tools & Technologies
- **Python:** Data analysis and preprocessing
- **Pandas:** Data manipulation and cleaning
- **JupyterLab:** Interactive analysis
- **PostgreSQL:** SQL queries and business analysis
- **pgAdmin 4:** Database management
- **Power BI:** Interactive dashboard and data visualization
- **Gamma:** Presentation creation

## Project Workflow

### 1. Data Loading
Imported the customer shopping dataset into Python using Pandas and examined its structure, columns, and data types.

### 2. Exploratory Data Analysis (EDA)
Performed exploratory analysis using descriptive statistics, data distributions, and missing-value checks to understand customer purchasing patterns.

### 3. Data Cleaning & Transformation
- Identified and handled missing values in review ratings.
- Filled missing review ratings using category-wise median values.
- Standardized column names for easier analysis.
- Created additional features, including age groups and purchase frequency in days.
- Prepared the cleaned dataset for SQL analysis and visualization.

### 4. SQL Analysis Using PostgreSQL
Executed SQL queries to answer key business questions, including:
- Revenue comparison by gender and age group.
- Average purchase amount by shipping type.
- Spending patterns of subscribers and non-subscribers.
- Top-rated products and discount usage by product.
- Customer segmentation into New, Returning, and Loyal customers.
- Most-purchased products within each category.
- Subscription behavior among repeat buyers.

### 5. Power BI Dashboard
Built an interactive Power BI dashboard to present customer purchasing behavior, revenue patterns, product performance, and customer segmentation in a clear and visual format.

### 6. Reporting & Presentation
Prepared a project report summarizing the methodology and analysis. Created a presentation using Gamma to communicate the key findings and business implications.

## Dashboard
The Power BI dashboard provides a visual overview of customer shopping behavior and supports analysis of:
- Customer purchasing patterns.
- Revenue and purchase amounts.
- Product and category performance.
- Customer demographics and loyalty.
- Subscription and discount behavior.
- Shipping preferences.

**Dashboard File:** `customer_behavior_Dashboard.pbix`

Open the file in Power BI Desktop to explore the dashboard.

## Results
- Analyzed 3,900 customer purchase records across 18 original columns.
- Identified 37 missing values in the review rating column and handled them using category-wise median imputation.
- Prepared the dataset for further analysis by standardizing column names and creating additional analytical features.
- Used PostgreSQL queries to investigate revenue, product ratings, discount usage, customer loyalty, shipping preferences, and subscription behavior.
- Developed a Power BI dashboard to communicate customer behavior patterns and support data-driven decision-making.

## How to Run

### Prerequisites
Install the following tools:
- Python
- JupyterLab
- PostgreSQL
- pgAdmin 4
- Power BI Desktop

### Step 1: Clone the Repository
```bash
git clone <your-repository-url>
cd customer-shopping-behavior-analysis
```

### Step 2: Install Python Libraries
```bash
pip install pandas jupyter
```

### Step 3: Load the Dataset
Place `customer_shopping_behavior.csv` in the project directory.

Load it into Python using:

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")
```

### Step 4: Run the Notebook
Start JupyterLab:

```bash
jupyter lab
```

Open `Customer_Shopping_Behavior_Analysis.ipynb` and execute the cells in order.

### Step 5: Run SQL Queries
1. Create a database in PostgreSQL.
2. Import the cleaned dataset into a table named `customer`.
3. Open `customer_behavior_SQL_queries.sql` in pgAdmin 4.
4. Execute the queries to explore the results.

Ensure that the database table uses the column names expected by the SQL queries.

### Step 6: Open the Dashboard
Open `customer_behavior_Dashboard.pbix` in Power BI Desktop to explore the visualizations.

## Project Structure
```text
customer-shopping-behavior-analysis/
├── customer_shopping_behavior.csv
├── Customer_Shopping_Behavior_Analysis.ipynb
├── customer_behavior_SQL_queries.sql
├── customer_behavior_Dashboard.pbix
├── report.pdf
├── presentation.pdf
└── README.md
```

*Replace the report and presentation filenames with the actual filenames included in your repository.*

## Future Improvements
- Add automated data-quality checks.
- Develop reusable SQL views for key business metrics.
- Document additional findings and actionable recommendations.
- Publish dashboard screenshots and a project walkthrough.

## Author
**Piyush Kumar Anand**

Data Analytics Project | Python | SQL | PostgreSQL | Power BI

- LinkedIn: <https://www.linkedin.com/in/piyush-kumar-anand-816b8a339>

