# 🛒 E-Commerce Health Check

## 📊 Mini-Capstone Data Science Project

This project performs an **E-Commerce Health Check** using the **Olist Brazilian E-Commerce Public Dataset**.

The analysis focuses on customer behavior, product revenue, order-value patterns, delivery performance, customer satisfaction, and order trends.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze top-performing products by revenue
- Calculate the repeat customer rate
- Analyze monthly order trends
- Study order-value distribution
- Analyze the relationship between delivery time and customer review scores
- Detect order-value outliers
- Calculate a 95% confidence interval for average order value
- Compare weekday and weekend order volumes
- Generate business insights and recommendations

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **SQL**
- **SQLite**
- **Google Colab / Jupyter Notebook**

---

## 📁 Dataset

**Dataset:** Olist Brazilian E-Commerce Public Dataset

The dataset contains information related to:

- Orders
- Customers
- Products
- Order Items
- Reviews
- Payments
- Sellers
- Geolocation
- Product Categories

The original dataset is not included in this repository.

---

## 🔍 Data Analysis Process

### 1. Data Loading & Cleaning

The datasets were loaded using Pandas and inspected for:

- Missing values
- Duplicate records
- Data types
- Date columns

Date columns were converted into proper datetime format for analysis.

### 2. Data Merging

Multiple datasets were combined using common identifiers such as:

- `order_id`
- `customer_id`
- `customer_unique_id`
- `product_id`

### 3. Order Value Analysis

Order value was calculated using:

- Product price
- Freight value

The distribution of order values was analyzed using descriptive statistics and a histogram.

### 4. Product Revenue Analysis

SQL and Python were used to identify the highest-revenue products.

### 5. Customer Analysis

The repeat customer rate was calculated using `customer_unique_id` to correctly identify customers who placed multiple orders.

### 6. Delivery & Review Analysis

Delivery time was compared with customer review scores using correlation analysis.

### 7. Outlier Detection

The **IQR (Interquartile Range)** method was used to identify unusual order values.

### 8. Statistical Analysis

A **95% confidence interval** was calculated for the average order value.

### 9. Weekday vs Weekend Analysis

Order volumes were compared between weekdays and weekends.

---

## 📈 Key Results

| Metric | Result |
|---|---:|
| Average Order Value | ₹160.58 |
| Median Order Value | ₹105.29 |
| 95% Confidence Interval | ₹159.20 – ₹161.95 |
| Repeat Customer Rate | 3.12% |
| Delivery–Review Correlation | -0.33 |
| Weekday Orders | 76,594 |
| Weekend Orders | 22,847 |
| Order-Value Outliers | 7,775 |
| Highest Product Revenue | ₹63,885 |

---

## 💡 Key Findings

### 1. Low Repeat Customer Rate

The repeat customer rate is **3.12%**, indicating that most customers placed only one order.

### 2. Delivery Time and Customer Satisfaction

The correlation between delivery time and review score is **-0.33**. Longer delivery times are generally associated with lower review scores.

> Correlation does not establish causation.

### 3. Right-Skewed Order Values

The average order value is **₹160.58**, while the median is **₹105.29**. The higher mean indicates that some high-value orders increase the average.

### 4. Weekday Orders Dominate

There were **76,594 weekday orders** compared with **22,847 weekend orders**. Approximately 77% of orders occurred on weekdays.

### 5. High-Revenue Products

The highest-revenue product generated **₹63,885** in product revenue, showing that some products contribute significantly to sales revenue.

---

## 🧮 SQL Analysis

SQL was used for:

- Top 10 products by revenue
- Repeat customer rate
- Monthly order trends

The SQL analysis demonstrates the use of:

- `SELECT`
- `JOIN`
- `GROUP BY`
- `ORDER BY`
- `LIMIT`
- `CASE`
- `CTE`
- Window functions such as `RANK()`

---

## 💼 Business Recommendation

The analysis suggests focusing on **customer retention and delivery performance**.

Possible actions include:

- Introducing targeted offers for existing customers
- Improving delivery speed
- Monitoring high-value products
- Maintaining availability of important revenue-generating products

---

## 📂 Repository Contents

```text
e-commerce-health-check/
│
├── E-Commerce Health Check.ipynb
├── E_Commerce_Health_Check_Final_Report.pdf
└── README.md
