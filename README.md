# InsightsHub
A collection of data-driven projects exploring trends ,patterns and insights cross various domains
# Budget Sales Analysis

## Overview
This project involves analyzing sales data from the AdventureWorks and Budget datasets. The data covers various sales categories, subcategories, monthly trends, and yearly distributions, allowing insights into sales performance across multiple dimensions. This analysis includes data cleaning, exploratory data analysis (EDA), visualization, and exporting for further analysis in tools like Tableau.

## Dataset Information

### 1. **AdventureWorks_Database.xlsx**
   - Contains data related to sales transactions.
   - Fields include:
     - **Date**: Specific transaction dates.
     - **Year, Quarter, Month**: Temporal data indicating the year, quarter, and month.
     - **Fiscal Year, Fiscal Quarter, Fiscal Month**: Financial periods.
     - **Weekday/Weekend**: Indicates whether the transaction took place on a weekday or weekend.

### 2. **Budget.xlsx**
   - Includes monthly sales budgets for various categories and subcategories of products.
   - Fields include:
     - **Category**: Main product category.
     - **Subcategory**: Specific subcategories within each category.
     - **Product Name and Product Key**: Identifiers for each product.
     - **Monthly Columns (Jan 2016 - Dec 2016)**: Budgeted sales amounts by month.
     - **Grand Total**: Total budgeted sales amount for the year.

## Project Structure

├── Budget Sales Analysis.ipynb        
├── cleaned_budget_data.csv             
├── adventure_data.csv                  
├── reshaped_budget.csv                
                          

## Project Steps

### 1. Data Loading
   - Mounted Google Drive in Google Colab to access datasets.
   - Extracted the zipped data folder.
   - Loaded both `AdventureWorks_Database.xlsx` and `Budget.xlsx` files using Pandas.

### 2. Data Cleaning and Preprocessing
   - **Budget Dataset**:
     - Skipped the first 3 rows to access the actual data.
     - Manually assigned column names based on header row content.
     - Filled missing values in `Subcategory`, `ProductName`, and `ProductKey`.
   - **AdventureWorks Dataset**:
     - Examined and exported the data for consistency and formatting.
     - Provided frequency counts by year, month, quarter, weekday, and weekend.

### 3. Exploratory Data Analysis (EDA)
   - **Category and Subcategory Sales**:
     - Calculated total sales for each product category and subcategory.
     - Visualized these totals using bar plots.
   - **Monthly Sales Trends**:
     - Summed monthly sales for each month and plotted trends.
   - **Yearly and Quarterly Distributions**:
     - Analyzed the frequency of data by year and quarter.
     - Identified peak periods for sales transactions.
   - **Temporal Trends**:
     - Analyzed sales frequency by fiscal periods such as fiscal year, fiscal quarter, and fiscal month.
   - **Weekday vs Weekend**:
     - Compared transaction frequencies between weekdays and weekends.

### 4. Visualizations
   - **Matplotlib and Seaborn** were used to create visualizations:
     - Bar plots of total sales per category and subcategory.
     - Line plots of monthly sales trends.
     - Count plots for yearly, monthly, weekday/weekend distributions.
   - Insights from these visualizations helped identify top-performing categories, peak months, and important trends in sales.

### 5. Exporting Data
   - Saved cleaned data to CSV files:
     - `cleaned_budget_data.csv`: Contains cleaned and processed budget data.
     - `adventure_data.csv`: Contains processed AdventureWorks data.
     - `reshaped_budget.csv`: Reshaped data for use in visualization tools like Tableau.

## Analysis Summary

- **Total Sales by Category**: Identified high-performing categories and subcategories for budgeted sales.
- **Monthly Sales Trends**: Observed seasonal patterns and peak sales periods.
- **Yearly Analysis**: Determined the most active years and quarters.
- **Weekday vs Weekend Sales**: Analyzed transaction patterns based on day type.
- **Fiscal Trends**: Aligned data to fiscal periods to support business insights.

## Key Findings

1. **Category Analysis**: Certain categories consistently outperform others in budgeted sales.
2. **Monthly Sales Patterns**: Notable seasonal fluctuations, with peak months identified.
3. **Transaction Distribution**: Higher transaction volumes noted in specific quarters and months.
4. **Fiscal Year Analysis**: Insights based on fiscal years and quarters to support budget alignment.

## Usage

1. **Run the Notebook**:
   - Open `Budget Sales Analysis.ipynb` in Google Colab.
   - Ensure that the dataset is available on Google Drive or within the local environment.
2. **Explore Visualizations**:
   - Adjust plot parameters to explore different views of the data.
   - Run visualizations for quick insights into sales performance.
3. **Tableau Import**:
   - Use `reshaped_budget.csv` in Tableau for interactive visualizations.

## Future Enhancements

- **Predictive Modeling**: Apply machine learning to predict future sales.
- **Advanced Visualization**: Use dynamic dashboards in Tableau for real-time insights.
- **Deep Dive into Product-Level Analysis**: Explore patterns at the individual product level.

## Technologies Used

- **Python**: Data manipulation and analysis with Pandas.
- **Google Colab**: Environment for coding and visualizations.
- **Tableau**: For creating interactive visualizations (future step).
- **Libraries**: Matplotlib, Seaborn for data visualization.
