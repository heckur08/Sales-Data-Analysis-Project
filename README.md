# Sales Data Analysis Project

## Overview
This project analyzes 12 months of sales data for an electronics store using Python's Pandas and Matplotlib libraries. The dataset contains hundreds of thousands of electronic store purchases with details like month, product type, cost, purchase address, and more.

## Project Structure
The analysis follows these main steps:
1. **Data Cleaning**
2. **Business Question Analysis** 
3. **Visualization**

## Data Cleaning
Before analysis, we performed several data cleaning tasks:
- Dropped NaN values from the DataFrame
- Removed invalid rows based on conditions
- Converted column types (to numeric, datetime formats)
- Merged 12 months of sales data into a single DataFrame
- Added useful columns like Sales, Month, City, and Time information

## Key Business Questions Answered

### 1. Best Month for Sales
**Analysis:** Aggregated sales by month  
**Finding:** December was the best month with $4.61 million in sales  
**Visualization:** Bar chart showing monthly sales figures

### 2. City with Most Sales
**Analysis:** Grouped sales by city  
**Finding:** San Francisco generated the most revenue at $8.26 million  
**Visualization:** Bar chart comparing sales across cities

### 3. Optimal Advertisement Time
**Analysis:** Examined order frequency by hour  
**Finding:** Peak order times are around 11am and 7pm  
**Visualization:** Line graph showing order volume throughout the day

### 4. Frequently Sold Together Products
**Analysis:** Identified product combinations in same orders  
**Finding:** iPhone and Lightning Cable are most commonly purchased together  
**Method:** Used groupby and transform to concatenate products in same orders

### 5. Best Selling Product
**Analysis:** Calculated total quantity sold by product  
**Finding:** AAA Batteries (4-pack) sold the most units (31,017)  
**Visualization:** Bar chart of product quantities sold

## Technical Methods Used
- `pd.concat()` to combine multiple CSV files
- String parsing to create new columns
- `.apply()` method for data transformations
- Groupby operations for aggregate analysis
- Various Pandas functions (`to_numeric`, `to_datetime`, `astype`)
- Matplotlib for data visualization (bar charts, line graphs)
- Proper labeling and formatting of visualizations

## How to Run
1. Clone the repository
2. Install required packages: Jupyter Notebook and Pandas
3. Open and run the `Sales_Data_Analysis.ipynb` notebook

## Dependencies
- Python 3
- Pandas
- Matplotlib
- Jupyter Notebook

This analysis provides valuable insights for business decision making, from inventory management to marketing strategy optimization.
