# 🛒 E-commerce Data Analysis (SQL + Python)

📌 Project Overview

This project analyzes an e-commerce dataset using SQL and Python to extract meaningful business insights. The data is stored in a MySQL database and queried using Python for analysis and visualization.

The goal is to answer real-world business questions like customer distribution, sales trends, and payment behavior.

---

⚙️ Tech Stack

- Python
- MySQL
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

📂 Dataset

The project uses multiple CSV files:

- "customers.csv"
- "orders.csv"
- "order_items.csv"
- "products.csv"
- "payments.csv"
- "sellers.csv"

These files are imported into a MySQL database for querying.

---

🛠️ Setup Instructions

1. Install Dependencies

pip install pandas numpy matplotlib seaborn mysql-connector-python

2. Setup MySQL Database

- Create a MySQL database
- Import CSV files into tables
- Ensure table names match:
  - customers
  - orders
  - order_items
  - products
  - payments
  - sellers

3. Configure Database Connection

Update your credentials in the notebook:

mysql.connector.connect(
    host='localhost',
    username='your_username',
    password='your_password',
    database='your_database'
)

---

📊 Key Analysis Performed

1. Customer Insights

- List of unique cities where customers are located

2. Order Analysis

- Total number of orders placed in a specific year (e.g., 2017)

3. Sales Analysis

- Total sales per product category

4. Payment Behavior

- Percentage of orders paid in installments

---

📈 Sample Queries

Unique Customer Cities

SELECT DISTINCT customer_city FROM customers;

Orders in 2017

SELECT COUNT(order_id)
FROM orders
WHERE YEAR(order_purchase_timestamp) = 2017;

Sales per Category

SELECT 
    products.product_category AS category,
    ROUND(SUM(payments.payment_value), 2) AS sales
FROM products
JOIN order_items ON products.product_id = order_items.product_id
JOIN payments ON payments.order_id = order_items.order_id
GROUP BY category;

---

📊 Visualization

The project uses:

- Matplotlib
- Seaborn

To generate:

- Sales distribution charts
- Category performance graphs
- Trend analysis plots

---

🎯 Key Insights

- Customer base is spread across multiple cities
- Order volume varies significantly year-wise
- Certain product categories dominate revenue
- Installment payments form a notable portion of transactions

---

🚀 Future Improvements

- Add dashboard using Power BI / Tableau
- Implement predictive analytics (sales forecasting)
- Build recommendation system
- Deploy as a web dashboard using Django or Flask

---

👨‍💻 Author

Charka Mahesh

BTech - Computer Science & Data Science

Skills: Python, SQL, Data Analysis, Visualization

---

📌 Note

This project is designed for learning and portfolio demonstration purposes. Data used is for analysis practice only.
