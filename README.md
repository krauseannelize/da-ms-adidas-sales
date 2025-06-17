# Adidas Sales Analysis Dashboard 

## Tools & Skills Used

![Tableau](https://img.shields.io/badge/Tableau-Dashboard-%235778a4)
![Tableau](https://img.shields.io/badge/Tableau-Data%20Analysis-%235778a4)
![Tableau](https://img.shields.io/badge/Tableau-Interactive%20Filtering-%235778a4)  

## Quick Access

- [Raw Data](/adidas-dataset-raw.csv)
- [Clean Data](/adidas-dataset-clean.csv)
- [Tableau Workbook]()
- [Tableau Public Dashboard]()

## Project Overview

This project is a self-initiated deep dive to practically apply advanced Tableau data visualization techniques. Leveraging the core concepts and the Adidas sales dataset provided through the Masterschool Data program, my goal is to comprehensively incorporate principles learned from the "Data Modeling with Parameters, Groups and Sets" section.

Key Tableau concepts that was explored:

- Data Type Management
- Table Calculations
- Level of Detail (LOD) Expressions
- Date & Time Analysis
- Parameters
- Groups
- Sets

The Tableau Public Dashboard can be [viewed online here]() and the workbook can be downloaded [here]().

## Data Cleaning

The raw data contained several inconsistencies and errors that required systematic cleaning to ensure accuracy and consistency. The key data cleaning steps performed were:

- **Handling Blank Rows:** Identified and removed two significant blocks of blank rows (1226-1369 and 5114-5257)
- **Standardizing Dates:** Extracted individual date components (day, month, year) from the "Invoice Date" column and then reconstructed the dates into a uniform and consistent format, facilitating proper chronological analysis.
- **Cleaning Numerical Fields:** Removed the dollar sign ($) from the "Price per Unit", "Total Sales", and "Operating Profit" columns, to ensure fields will be recognized as numerical values rather than text strings.
- **Correcting Total Sales:** The "Total Sales" amounts were uniformly ten times larger than their actual value. This was corrected by recalculating "Total Sales" for all records as the product of "Price per Unit" and "Units Sold".
- **Correcting Operating Profit:** Similarly, the "Operating Profit" amounts were found to be inflated by a factor of ten in most instances. "Operating Profit" was recalculated for all records by multiplying the new "Total Sales" amount by the corresponding "Operating Profit" percentage, ensuring accuracy and rounding to the nearest integer.
