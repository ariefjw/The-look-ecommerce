# 📊 The Look Ecommerce - Tableau Dashboard

[![Tableau](https://img.shields.io/badge/Tableau-2023.1+-blue.svg)](https://www.tableau.com/)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()

## 📋 Table of Contents
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Data Sources](#data-sources)
- [Setup Instructions](#setup-instructions)
- [Troubleshooting](#troubleshooting)
- [Contact](#contact)

## 🔍 Overview
This repository contains a Tableau dashboard for monitoring The Look Ecommerce's operational performance. The dashboard focuses on shipping performance and inventory management metrics.

## 💻 Prerequisites
- Tableau Desktop 2023.1 or later
- Access to CSV data files
- Minimum 8GB RAM recommended
- Stable internet connection for live data updates

## 📁 Data Sources Setup

### Required Files
1. Primary Data:
   - `order.csv` - Main order information
   - `order_items.csv` - Order details
   - `products.csv` - Product catalog

2. Inventory Data:
   - `inventory_items.csv` - Main inventory tracking
   - `dc.csv` - Distribution center information

3. Stock Analysis:
   - `stock_turnover.csv` - Stock performance metrics
   - `stock_aging.csv1` - Age of stock items
   - `safety_stock.csv` - Safety stock levels
   - `oldest_stock.csv` - Oldest inventory items

### File Placement
1. Create a dedicated data folder:
```bash
📁 The_Look_Ecommerce
 ┣ 📁 Data
 ┃ ┣ 📄 order.csv
 ┃ ┣ 📄 order_items.csv
 ┃ ┣ 📄 products.csv
 ┃ ┣ 📄 inventory_items.csv
 ┃ ┣ 📄 dc.csv
 ┃ ┣ 📄 stock_turnover.csv
 ┃ ┣ 📄 stock_aging.csv1
 ┃ ┣ 📄 safety_stock.csv
 ┃ ┗ 📄 oldest_stock.csv
 ┗ 📄 Thelook_Ecommerce.twb
```

## 🛠️ Setup Instructions

### 1. Initial Setup
1. Download and install Tableau Desktop
2. Create the folder structure as shown above
3. Place all CSV files in the Data folder
4. Open `Thelook_Ecommerce.twb`

### 2. Data Connection Setup
1. In Tableau Desktop, go to "Data Source" tab
2. For each CSV file:
   ```
   a. Click "Add Connection" > "Text file"
   b. Navigate to the Data folder
   c. Select the CSV file
   d. Verify data types for each column
   ```

### 3. Establishing Relationships
Connect the tables in this order:
```
order.csv ─── order_items.csv ─── products.csv ─┬─ dc.csv
                                               │
                                               ├─ inventory_items.csv ─┬─ oldest_stock.csv
                                                                     ├─ safety_stock.csv
                                                                     ├─ stock_aging.csv1
                                                                     └─ stock_turnover.csv
```

Key steps:
1. Start with `order.csv` as your primary table
2. Join `order_items.csv` using Order ID
3. Connect `products.csv` using Product ID
4. Link remaining tables following the relationship diagram

### 4. Data Refresh Settings
1. For Live Connections (Real-time data):
   - `order.csv` and `order_items.csv`
   - Set refresh rate: Every 15 minutes

2. For Extract Connections (Daily updates):
   - All other CSV files
   - Schedule daily refresh during off-peak hours

## 🔧 Troubleshooting

### Common Connection Issues
1. **File Not Found Errors**
   ```
   Solution:
   - Verify file paths
   - Check file names (case-sensitive)
   - Ensure CSV files are not open in other programs
   ```

2. **Data Type Mismatches**
   ```
   Solution:
   - Review CSV column data types
   - Use "Data Interpreter" in Tableau
   - Fix date formats if necessary
   ```

3. **Performance Issues**
   ```
   Solution:
   - Use extracts for large CSV files
   - Index frequently filtered fields
   - Optimize relationships
   ```

### Data Refresh Problems
1. Check file permissions
2. Verify CSV file encoding (use UTF-8)
3. Monitor available disk space
4. Review Tableau logs for errors

## 📧 Contact
For technical support and queries:
- Email: ariefjkwicakson@gmail.com
- LinkedIn: [Arief Joko Wicasksono](https://www.linkedin.com/in/arief-joko-wicaksono-80a519141)
- GitHub: [ariefjw](https://github.com/ariefjw)

---

<div align="center">
  <sub>Built by Arief Joko Wicaksono</sub>
</div> 