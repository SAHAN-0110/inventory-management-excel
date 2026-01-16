# Inventory Management System (Excel)

## Overview
This project is an inventory management system built in Microsoft Excel to track stock levels, monitor product movements, and identify inventory risks.

The system is designed to work with real-world data volume and focuses on accuracy, robustness, and clear visibility of inventory status.

---

## Problem Statement
Manual inventory tracking often leads to:
- Stock shortages
- Overstocking
- Data inconsistencies
- Delayed decision-making

This project addresses these issues by providing a structured and automated Excel-based solution.

---

## Sheets Description

### 1. Inventory_Data
Contains master data for products, including:
- Product ID
- Product Name
- Category
- Supplier
- Reorder Level
- Unit Price

This sheet acts as the reference table for the entire system.

---

### 2. Stock_Movements
Records all stock transactions with:
- Date
- Product ID
- Movement Type (IN / OUT)
- Quantity

This sheet represents real operational activity and drives stock calculations.

---

### 3. Inventory_Status
Calculates current stock levels using Excel formulas and displays inventory health:
- Current Stock
- Reorder Level
- Stock Status

Stock Status logic:
- **DATA ISSUE** → More stock-out than stock-in (data inconsistency)
- **LOW STOCK** → Stock below reorder level
- **OK** → Healthy stock level

Conditional formatting is used for quick visual alerts.

---

### 4. Dashboard
Provides a summary view of inventory health, including:
- Total number of products
- Count of data issues
- Low stock items
- Inventory distribution insights

The dashboard updates dynamically as stock movement data changes.

---

## Key Insights
- The system highlights data inconsistencies instead of hiding them.
- Low-stock items are identified early to support timely reordering.
- Inventory status updates automatically based on transaction data.
- The design supports scalability with larger datasets.

---

## Tools Used
- Microsoft Excel
- Pivot Tables
- Conditional Formatting
- SUMIFS, COUNTIF, IF logic

---

## Conclusion
This project demonstrates how Excel can be used to build a practical inventory management system with real-world logic, error handling, and decision-support features.
