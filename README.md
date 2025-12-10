# Sales Analysis Power BI Project

This project contains a Power BI dashboard and the associated datasets used to analyze sales performance, customer demographics, and product trends. The analysis is based on transactional order data and customer profiles.

## 📂 Files Included

* **`My First Dashboard.pbix`**: The main Power BI report file containing visualizations and the data model.
* **`orders.csv`**: The transactional dataset containing details of individual sales.
* **`customers.csv`**: The dimension dataset containing customer information and location details.

## 📊 Data Structure

### 1. Orders Data (`orders.csv`)
This file contains sales transactions. The key columns are:
* `order_id`: Unique identifier for each transaction (e.g., O0001).
* `order_date`: Date the order was placed.
* `customer_id`: Foreign key linking to the Customers table.
* `product_name`: Name of the item sold (e.g., iPhone 16, Dell XPS 15).
* `product_category`: Category of the product (e.g., Smartphone, Laptop, Accessory).
* `quantity`: Number of units purchased.
* `sales`: Total revenue for the transaction.

### 2. Customers Data (`customers.csv`)
This file contains customer details. The key columns are:
* `customer_id`: Unique identifier for the customer (Links to `orders.csv`).
* `first_name` & `last_name`: Customer's full name.
* `country`, `state`, `city`: Geographic location of the customer.
* `score`: A customer score/rating metric.

## 🚀 Getting Started

1.  **Prerequisites**: Ensure you have [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) installed.
2.  **Open the Report**: Double-click `My First Dashboard.pbix` to open the project.
3.  **Data Connection**:
    * If the dashboard does not load data immediately, you may need to refresh the data source settings.
    * Go to **Home** > **Transform Data** > **Data Source Settings** and ensure the file paths for `orders.csv` and `customers.csv` match the location where you saved them on your computer.

## 📈 Analysis Overview

The dashboard is designed to provide insights into:
* **Sales Performance**: Total revenue analysis over time (yearly/monthly trends).
* **Product Insights**: Best-selling products and top-performing categories (e.g., Laptops, Smartphones).
* **Geographic Distribution**: Sales breakdown by Country, State, and City (featuring US, China, Germany, etc.).
* **Customer Insights**: Analysis of high-value customers based on sales volume and scores.

## 🤝 Contributing

Feel free to update the datasets or add new visualizations to the `.pbix` file to extend the analysis.
