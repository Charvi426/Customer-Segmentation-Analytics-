# Customer-Segmentation-Analytics
Consumer behavior analysis and customer segmentation project using Python, PostgreSQL, Power BI, and K-Means clustering to analyze purchasing patterns, customer loyalty, and revenue insights.

## Project Overview

This project analyzes retail customer data to identify purchasing trends, customer loyalty patterns, discount effectiveness, and revenue insights. In addition to SQL-based business analytics, K-Means clustering was applied to segment customers into meaningful behavioral groups.

The project combines:
- Data Cleaning using Pandas
- SQL Analysis using PostgreSQL
- Data Visualization using Power BI
- K-Means Clustering

---

## Tech Stack

- Python
- Pandas
- PostgreSQL
- Power BI
- Scikit-learn
- NumPy
- Matplotlib

---

## Dataset Features

The dataset contains customer purchase and demographic information such as:

- Customer ID
- Gender
- Age Group
- Category
- Purchase Amount (USD)
- Previous Purchases
- Review Rating
- Subscription Status
- Discount Applied
- Shipping Type
- Payment Method
- Frequency of Purchases

---

## Project Workflow

### 1. Data Cleaning & Preprocessing
- Handled missing values
- Converted categorical purchase frequency into numerical values
- Performed feature engineering for clustering

### 2. SQL-Based Consumer Behavior Analysis
Performed analytical queries in PostgreSQL to analyze:
- Revenue by gender
- Revenue by age group
- Subscription behavior
- Discount effectiveness
- Shipping type analysis
- Top-performing products
- Customer loyalty patterns

### 3. Dashboard Development
Built an interactive Power BI dashboard with:
- Revenue analysis
- Customer demographics
- Product insights
- Subscription analysis
- Payment and shipping insights

### 4. Customer Segmentation using K-Means
Applied K-Means clustering using:
- Purchase Amount
- Previous Purchases
- Purchase Frequency

Validation on the current CSV showed that the raw three-feature K-Means setup is the strongest variant for this dataset.

Compared clustering variants:
- Raw K-Means on the three core features: Silhouette Score 0.521
- Standardized + log-transformed K-Means: Silhouette Score 0.274
- Best k from elbow/silhouette sweep: k = 8, Silhouette Score 0.314
- Best alternative feature combo tested: base features only, Silhouette Score 0.274
- GMM on the same scaled features: Silhouette Score 0.313

Identified four customer groups:
- High-Value Loyal Customers
- Budget Loyal Customers
- Occasional Premium Buyers
- Seasonal Customers

Cluster quality was evaluated using the Silhouette Score. The notebook previously recorded 0.358; the current cleaned data and validation run produced a stronger raw baseline of 0.521.

---

## Key Insights

- High-Value Loyal Customers generated the highest revenue and showed the strongest purchase loyalty.
- Budget Loyal Customers purchased frequently but spent less per transaction.
- Occasional Premium Buyers made fewer purchases but had higher spending per order.
- Seasonal Customers exhibited infrequent purchasing behavior.

---

## Dashboard Preview

### Executive Overview Dashboard
Includes:
- Total Revenue
- Customer Demographics
- Revenue by Category
- Subscription Analysis
- Payment & Shipping Insights

### Customer Segmentation Dashboard
Includes:
- Revenue by Cluster
- Customer Count by Cluster
- Average Purchase Amount by Cluster
- K-Means Scatter Plot
- Subscription Analysis by Cluster

---

## Machine Learning Details

### Clustering Algorithm
- K-Means Clustering

### Features Used
- Purchase Amount (USD)
- Previous Purchases
- Purchase Frequency Days

### Evaluation Metric
- Silhouette Score: 0.521 on the current validated raw baseline

### Screenshots

<img width="1111" height="624" alt="image" src="https://github.com/user-attachments/assets/93dd8481-61aa-4a8b-b941-3c4560123124" />
<img width="1109" height="627" alt="image" src="https://github.com/user-attachments/assets/22198c03-d174-42ee-b7bd-605d93b7cd22" />


## Author

Charvi
