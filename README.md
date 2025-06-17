# Adidas Sales Analysis Dashboard 

## Quick Access

- [Raw Data](/adidas-dataset-raw.csv)
- [Clean Data](/adidas-dataset-clean.csv)

## Project Overview

This tutorial series is part of the Masterschool Data program, designed to help learners deepen their understanding of data visualization using an Adidas sales dataset. Through a structured sequence of lessons, it covers advanced Tableau techniques like table calculations, level of detail expressions, and time-based analysis, progressively applying these methods to explore sales performance across regions and products. Each section builds on the previous one, offering a hands-on, practical approach to mastering interactive dashboards and uncovering business-critical insights.

## Data Cleaning

The raw data contained several inconsistencies and errors that required systematic cleaning to ensure accuracy and consistency. The key data cleaning steps performed were:

- **Handling Blank Rows:** Identified and removed two significant blocks of blank rows (1226-1369 and 5114-5257)
- **Standardizing Dates:** Extracted individual date components (day, month, year) from the "Invoice Date" column and then reconstructed the dates into a uniform and consistent format, facilitating proper chronological analysis.
- **Cleaning Numerical Fields:** Removed the dollar sign ($) from the "Price per Unit", "Total Sales", and "Operating Profit" columns, to ensure fields will be recognized as numerical values rather than text strings.
- **Correcting Total Sales:** The "Total Sales" amounts were uniformly ten times larger than their actual value. This was corrected by recalculating "Total Sales" for all records as the product of "Price per Unit" and "Units Sold".
- **Correcting Operating Profit:** Similarly, the "Operating Profit" amounts were found to be inflated by a factor of ten in most instances. "Operating Profit" was recalculated for all records by multiplying the new "Total Sales" amount by the corresponding "Operating Profit" percentage, ensuring accuracy and rounding to the nearest integer.
