# **Customer Segmentation & Sales Trend Analysis**

## **Project Overview**
This project focuses on analyzing customer purchasing behavior, segmenting customers based on spending patterns, and forecasting sales trends. The goal is to provide data-driven insights for business decision-making.

## **Technologies Used**
- **Programming Language:** Python, SQL  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels  
- **Database:** MySQL  
- **Visualization Tools:** Power BI, Tableau  

## **Dataset**
The dataset contains customer transaction data with key attributes:
- `Customer_ID` – Unique customer identifier  
- `Age` – Customer’s age  
- `Gender` – Male/Female  
- `Annual_Income` – Customer’s annual earnings  
- `Spending_Score` – A rating of spending behavior (1-100)  
- `Purchase_Amount` – Total purchase value  
- `Purchase_Date` – Date of last purchase  
- `Region` – Geographic location  

## **Project Workflow**
### **Step 1: Data Extraction & Cleaning**
- Loaded data from **MySQL** into Python using `pandas`.
- Handled missing values and ensured proper **data types**.

### **Step 2: Exploratory Data Analysis (EDA)**
- Visualized **purchase distributions, income levels, and spending scores**.
- Used **scatter plots and histograms** to identify spending trends.

### **Step 3: Customer Segmentation (K-Means Clustering)**
- Standardized `Annual_Income` and `Spending_Score`.
- Applied **K-Means clustering** to segment customers into **high, medium, and low spenders**.
- Visualized customer clusters using **scatter plots**.

### **Step 4: Sales Forecasting (Time Series Analysis)**
- Resampled sales data to **monthly** and built an **ARIMA model**.
- Predicted **future sales trends** for the next **6 months**.
- Plotted actual vs. forecasted sales using **line charts**.

### **Step 5: Data Visualization in Tableau & Power BI**
- **Customer Segmentation Dashboard** (Scatter plot of income vs. spending score).
- **Sales Trend Dashboard** (Time-series analysis with forecasting).
- **Regional Sales Analysis** (Map visualization of purchase amounts).

## **Installation & Setup**
### **1️⃣ MySQL Database Setup**
Run the following SQL commands to create the database and table:
```sql
CREATE DATABASE sales_db;
USE sales_db;

CREATE TABLE customer_sales (
    Customer_ID INT PRIMARY KEY,
    Age INT,
    Gender VARCHAR(10),
    Annual_Income FLOAT,
    Spending_Score FLOAT,
    Purchase_Amount FLOAT,
    Purchase_Date DATE,
    Region VARCHAR(50)
);```

```
pip install pandas numpy seaborn matplotlib scikit-learn statsmodels mysql-connector-python
```

```
python customer_analysis.py


## **Expected Outcomes**
- **Customer Segmentation** helps businesses **target the right customers** for promotions.  
- **Sales Trend Analysis** enables businesses to **forecast revenue** and plan strategies.  
- **Power BI/Tableau Dashboards** provide **interactive insights** for better decision-making.  

## **Conclusion**
This project provides a **data-driven approach** to understanding customer behavior and optimizing business strategy. The combination of **clustering, forecasting, and visualization** allows companies to improve **marketing, retention, and sales performance**.  

## **License**
This project is open-source and free to use under the **MIT License**.  

## **Author**  
👤 **U. Aravindhakumar**  
📧 **msdaravind92@gmail.com**  
🔗 [**LinkedIn**](https://www.linkedin.com/in/aravindhakumar-u)
