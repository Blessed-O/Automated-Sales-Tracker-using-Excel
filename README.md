# Automated-Sales-Tracker-using-Excel
# Table of Content
- [Project Overview](https://github.com/Blessed-O/Automated-Sales-Tracker-using-Excel/blob/main/README.md#project-overview)

- [Dashboard](https://github.com/Blessed-O/Automated-Sales-Tracker-using-Excel/blob/main/README.md#dashboard)

- [Key Features](https://github.com/Blessed-O/Automated-Sales-Tracker-using-Excel/blob/main/README.md#key-features)
# Project Overview
Managing sales and inventory manually can be overwhelming, especially for small businesses. This project is an automated Excel-based Sales Tracker & Inventory Management System built for my business, BOXITBYLOLA (a gifting brand). This system simplifies sales tracking, automates stock updates, and generates real-time insights through a dynamic dashboard.
# Dashboard
![Dashboard](https://github.com/user-attachments/assets/e247c23e-cee2-40e0-b139-257b074fd6b5)
# Key Features
## Automated Sales & Purchase Entry
This system eliminates manual data entry by automating the sales and purchase recording process.

- **Macros & VBA Automation:** Recorded macros are assigned to the “SUBMIT” buttons, allowing users to enter sales or purchase details once, and the data is automatically recorded in the respective tables. This reduces human error and saves time.

- **Dynamic Data Validation:** Instead of manually searching for products, the system ensures that selecting a Product Category from a dropdown menu dynamically filters and displays only the relevant products under that category.

- **Automated Price Lookup with XLOOKUP:** When a product is selected, its price or cost is automatically retrieved from the product table using the XLOOKUP function, eliminating the need for manual price entry.

- **Real-Time Total Calculation:** Once a user inputs the quantity, the PRODUCT() function instantly calculates the total sales (Quantity × Price) and total cost (Quantity × Price) for each entry, ensuring accuracy without the need for manual computation.

![image](https://github.com/user-attachments/assets/55368e37-e4f7-44b4-ad16-acdb0628622d)

# Inventory Management System
The inventory system ensures real-time tracking of stock levels, preventing overstocking or running out of stock.

- **Real-Time Stock Updates with SUMIF():** The system automatically sums up the total purchases and total sales for each product using SUMIF(), giving an accurate count of items in stock at any moment.

- **Stock Level Calculation:** The remaining stock quantity is dynamically calculated using the formula: Stock = Total Purchases - Total Sales This ensures the system always reflects the latest stock levels.

- **Automated Stock Alerts with IF():** The system provides clear stock status updates based on remaining inventory levels:
  - Item 1
  - Item 2
  - Item 3
- **Automated Stock Alerts with IF():** The system provides clear stock status updates based on remaining inventory levels:
  - Item 1
  - Item 2
  - Item 3
# Data Structure & Workflow
The system is structured into different tables to ensure efficient data organization:

| Table Name  | Description |
|-------------|------------|
| **Sales** | Contains all sales transactions with details like date, product, quantity, amount and customer. |
| **Purchase** | Stores all purchase transactions with supplier details and cost price. |
| **Products** | Lists product names, categories, selling prices, and cost prices. |
| **Products Categories** | Lists product categories. |
| **Customers** | Stores customer names and information (randomly generated for privacy). |
| **Vendors** | Contains supplier details (randomly generated for privacy). |
| **Inventory** | Tracks current stock levels, updated automatically based on purchases and sales. |
