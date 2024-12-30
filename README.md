# Online_Retail_Analysis
Analyzed online retail transactional data with 100,000 rows to uncover key insights about customer behavior, product performance, and revenue trends.
# Online Retail Data Analysis and Visualization

This project focuses on analyzing an online retail dataset with 100,000 rows of transactional data. The objective is to uncover actionable insights about customer behavior, product performance, and revenue trends, utilizing a combination of Python, SQL, Power BI, and Excel.

## Table of Contents

1. [Overview](#overview)
2. [Dataset Description](#dataset-description)
3. [Tools and Technologies](#tools-and-technologies)
4. [Key Steps](#key-steps)
    - [Step 1: Data Cleaning and Preparation](#step-1-data-cleaning-and-preparation)
    - [Step 2: Database Setup](#step-2-database-setup)
    - [Step 3: Exploratory Data Analysis (EDA)](#step-3-exploratory-data-analysis-eda)
    - [Step 4: Visualization with Power BI](#step-4-visualization-with-power-bi)
5. [Key Insights](#key-insights)
6. [Future Enhancements](#future-enhancements)
7. [How to Use](#how-to-use)

---

## Overview

This project demonstrates an end-to-end data analysis workflow:
- **Objective**: Analyze transactional data to deliver actionable business insights.
- **Outcome**: Built an interactive Power BI dashboard to visualize revenue trends, customer segmentation, and product performance.

---

## Dataset Description

The dataset contains 581,000 rows of transactional data from an online retail business. Key columns include:
- `InvoiceNo`: Unique invoice numbers for transactions.
- `StockCode`: Product codes.
- `Description`: Product descriptions.
- `Quantity`: Quantity of items purchased.
- `InvoiceDate`: Date and time of the transaction.
- `UnitPrice`: Price per item.
- `CustomerID`: Unique identifier for customers.
- `Country`: Country of the customer.

---

## Tools and Technologies

- **Python**: Data cleaning and preparation using Pandas and NumPy.
- **SQL (Microsoft SQL Server)**: Database creation and exploratory data analysis.
- **Power BI**: Interactive dashboard development for data visualization.
- **Excel**: Initial data review and handling of subsets.

---

## Key Steps

### Step 1: Data Cleaning and Preparation

Performed in Python using Pandas:
- Removed duplicate rows and rows with missing values.
- Converted data types (e.g., `InvoiceDate` to datetime, `CustomerID` to integer).
- Removed outliers (negative values in `Quantity` and `UnitPrice`).
- Saved the cleaned dataset as `cleaned_retail_data.csv`.

### Step 2: Database Setup

- Imported the cleaned dataset into Microsoft SQL Server.
- Created a database called `OnlineRetail`.
- Performed SQL queries to analyze trends, calculate metrics, and segment customers.

### Step 3: Exploratory Data Analysis (EDA)

Key SQL queries:
- Total revenue calculation: `SUM(Quantity * UnitPrice)`.
- Monthly revenue trends.
- Customer segmentation by total spending.

### Step 4: Visualization with Power BI

- Imported the SQL queries into Power BI.
- Created visuals to represent:
  - Revenue trends over time.
  - Top-selling products and customers.
  - Regional performance by country.
  - Average basket size (revenue per order).

---

## Key Insights

1. **Revenue Trends**:
   - Peak sales occurred during the holiday season.
   - Weekday sales were higher than weekend sales.
2. **Top Products**:
   - Identified products contributing the most to revenue.
3. **Customer Segmentation**:
   - Top 10 customers accounted for a significant portion of total revenue.
4. **Regional Performance**:
   - Majority of sales came from the UK.

---

## Future Enhancements

- Implement predictive models to forecast sales trends.
- Perform advanced customer segmentation using clustering techniques.
- Automate data updates in Power BI for real-time insights.

---

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/online-retail-analysis.git
   ```

2. **Set Up the Environment**:
   - Install Python dependencies:
     ```bash
     pip install pandas numpy
     ```
   - Set up Microsoft SQL Server and import the `cleaned_retail_data.csv` file.

3. **Run the Python Scripts**:
   - Use the provided scripts to clean and prepare the dataset.

4. **Analyze with SQL**:
   - Import the SQL queries into your database.

5. **Visualize with Power BI**:
   - Open the provided Power BI file (`OnlineRetailDashboard.pbix`) to explore the dashboard.

---

Feel free to fork this repository and adapt it to your needs! For any questions or suggestions, please reach out via LinkedIn or GitHub Issues.
