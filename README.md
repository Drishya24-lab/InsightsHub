# InsightsHub
A collection of data-driven projects exploring trends ,patterns and insights cross various domains
# Budget Sales Analysis Project

## Overview
This project analyzes sales data from the AdventureWorks database and a budget dataset. The primary goal is to derive insights from sales trends over different time periods and product categories.

## Datasets
1. **AdventureWorks_Database.xlsx**: Contains historical sales data, including timestamps and product details.
2. **Budget.xlsx**: Contains budgeted sales data across different categories and months.

## File Structure
/content ├── Budget Sales data.zip ├── cleaned_budget_data.csv ├── adventure_data.csv ├── reshaped_budget.csv

## Data Preparation
- The **Budget.xlsx** file is read while skipping the first three rows to avoid metadata.
- The column names are manually set based on the fourth row to ensure accurate data representation.
- Missing values are filled with appropriate placeholders:
  - Subcategory: 'Unknown'
  - ProductName: 'Unknown'
  - ProductKey: 0 (assumed numeric)

## Data Exploration
### Sales Analysis
- **Total Sales per Category**: A bar plot visualizing total sales for each category.
- **Monthly Sales Trends**: A line plot showing sales trends across months.
- **Total Sales per Subcategory**: A bar plot visualizing total sales for each subcategory.

### Statistical Summary
- Monthly totals and averages are calculated and printed for insights into sales performance.
- Top known products by total sales are identified.

### Temporal Analysis
- Yearly, quarterly, monthly, and weekday/weekend distributions are visualized using count plots.
- The most frequent time periods in terms of sales transactions are highlighted.

## Data Export
- Cleaned and reshaped datasets are exported as CSV files for further analysis or visualization in tools like Tableau.

## Libraries Used
- `pandas`: For data manipulation and analysis.
- `matplotlib` and `seaborn`: For data visualization.

## Instructions to Run
1. Ensure you have the necessary datasets.
2. Load the datasets using the provided Python code snippets.
3. Execute the data cleaning and analysis steps.
4. Visualize the results as specified.

## Future Improvements
- Explore additional insights by integrating external datasets (e.g., marketing data).
- Implement predictive modeling to forecast future sales trends.

## Author
[Drishya]
