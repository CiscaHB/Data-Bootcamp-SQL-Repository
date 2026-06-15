# 📊 SQL Retail & Sales Analysis Project

## 📌 Overview
This project was completed as part of a **Data Technician Bootcamp**, focusing on developing core SQL skills to manage, query, and analyse structured data. The work involved interacting with real-world style datasets (including **Northwind retail and sales data**) to extract insights that support business decision-making.

The project demonstrates the ability to design relational databases, write efficient SQL queries, and generate meaningful insights from customer, product, and sales data.

## 🛠️ Key Skills Demonstrated

### 🔍 Data Querying
- Used **`SELECT` statements** to retrieve full datasets and specific columns for reporting  
- Applied **`WHERE` clauses** to filter datasets (e.g., high-value products, customer locations)  
- Leveraged **`ORDER BY`** to sort results for analysis (e.g., most recent orders, top-priced products)  

Example:
```sql
SELECT *
FROM products
WHERE price > 50
ORDER BY price DESC;
````

 [\[Week 3 Dat...QLWorkbook \| Word\]](https://b2wcompletetraining057-my.sharepoint.com/personal/ciscahuman_bootcamp_leepgroup_com/_layouts/15/Doc.aspx?sourcedoc=%7BA75CCA6B-6F74-4E92-99AB-78B4A8DC38F5%7D&file=Week%203%20Databases%20and%20MySQLWorkbook.docx&action=default&mobileredirect=true)

***

### 📊 Aggregation & Data Summarisation

* Applied **`GROUP BY`** to aggregate data and identify trends
* Used functions such as `COUNT()` and `SUM()` to analyse sales and product volumes
* Generated insights such as:
  * Number of products per category
  * Total quantity sold per product

Example:

```sql
SELECT c.CategoryName, COUNT(p.ProductID) AS NoOfProducts
FROM products p
JOIN categories c ON p.CategoryID = c.CategoryID
GROUP BY c.CategoryName;
```

 [\[Week 3 Dat...QLWorkbook \| Word\]](https://b2wcompletetraining057-my.sharepoint.com/personal/ciscahuman_bootcamp_leepgroup_com/_layouts/15/Doc.aspx?sourcedoc=%7BA75CCA6B-6F74-4E92-99AB-78B4A8DC38F5%7D&file=Week%203%20Databases%20and%20MySQLWorkbook.docx&action=default&mobileredirect=true)

***

### 🔗 Working with Relationships (JOINs)

* Combined data across multiple tables using **SQL JOINs**
* Implemented:
  * **INNER JOIN** to retrieve matching records across tables
  * **LEFT JOIN** to include all records from one table even when there are no matches
* Built comprehensive reports combining:
  * Customers, orders, and employees
  * Products, categories, and suppliers

Example:

```sql
SELECT o.OrderID, o.OrderDate, c.CustomerName, e.FirstName
FROM orders o
JOIN customers c ON o.customerID = c.customerID
JOIN employees e ON o.employeeID = e.employeeID;
```

 [\[Week 3 Dat...QLWorkbook \| Word\]](https://b2wcompletetraining057-my.sharepoint.com/personal/ciscahuman_bootcamp_leepgroup_com/_layouts/15/Doc.aspx?sourcedoc=%7BA75CCA6B-6F74-4E92-99AB-78B4A8DC38F5%7D&file=Week%203%20Databases%20and%20MySQLWorkbook.docx&action=default&mobileredirect=true)

***

## 📈 Business Insights & Use Cases

Using SQL, the project explored practical retail and sales scenarios, including:

* 📦 **Product Analysis**
  * Identifying high-value and mid-range products
  * Classifying products by category and supplier

* 🧑‍🤝‍🧑 **Customer Insights**
  * Segmenting customers by location (e.g., UK & USA markets)
  * Supporting targeted marketing campaigns

* 🧾 **Sales & Order Analysis**
  * Tracking order trends over time
  * Analysing product demand and sales volume
  * Generating detailed order reports with customer and employee data

* 🌍 **Data Exploration**
  * Querying large datasets to identify patterns (e.g., population and geographic analysis in global datasets)

These tasks demonstrate how SQL can be used to transform raw data into **actionable business insights**. [\[Week 3 Dat...QLWorkbook \| Word\]](https://b2wcompletetraining057-my.sharepoint.com/personal/ciscahuman_bootcamp_leepgroup_com/_layouts/15/Doc.aspx?sourcedoc=%7BA75CCA6B-6F74-4E92-99AB-78B4A8DC38F5%7D&file=Week%203%20Databases%20and%20MySQLWorkbook.docx&action=default&mobileredirect=true)

***

## 🧠 What I Learned

* How to structure and query relational databases effectively
* The importance of clean, well-defined data relationships
* Writing efficient and readable SQL queries for real-world scenarios
* Using SQL to support **data-driven decision-making**

***

## 🚀 Tools & Technologies

* MySQL / MySQL Workbench
* Northwind Sample Database
* World Database (for global data analysis)

***

## ✅ Conclusion

This project highlights foundational SQL skills essential for a **Data Analyst or Data Technician role**. By combining filtering, sorting, aggregation, and joins, I was able to extract valuable insights from retail and sales data and present them in a structured, meaningful way.

***

```
```
