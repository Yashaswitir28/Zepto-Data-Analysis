# Zepto-Data-Analysis

# Summary
This Power BI dashboard analyzes retail sales data, focusing on total sales, item types, outlet performance, and key metrics. I chose this dataset to explore trends in sales, outlet sizes, and customer preferences using interactive visualizations, DAX calculations, and filters for insightful business decision-making. Optimized for clarity and performance. 🚀

# DAX (Data Analysis Expressions) for Measures & Calculations
1. Avg Rating = AVERAGE('Zepto Grocery Data'[Rating])
2. Avg Sales = AVERAGE('Zepto Grocery Data'[Sales])
3. No of Items = COUNTROWS('Zepto Grocery Data')
4. Total Sales = SUM('Zepto Grocery Data'[Sales]) 


# Data Visualization & Storytelling
Used different Power BI visuals to present insights effectively:
KPI Cards: For quick stats (Total Sales, No. of Items, Avg Rating)
Line Chart: Outlet establishment trend over time
Bar Chart: Item type comparison based on sales
Pie Charts: Outlet size contribution to sales
Stacked Bars & Donut Charts: Outlet identifiers by year

# Filters & Slicers for Interactivity
Where Used?
Filter Pane on the Left: Allows users to filter by Outlet Location, Outlet Size, and Item Type.

# Advanced Insights using Conditional Formatting
Color-coded Metrics:
Different colors for various outlet sizes in the pie chart.
Conditional formatting in the matrix table for Avg Sales and Item Visibility.

Metrics = {

    ("Total Sales", NAMEOF('Zepto Grocery Data'[Total Sales]), 0),

    ("Avg Sales", NAMEOF('Zepto Grocery Data'[Avg Sales]), 1),
    
    ("No of Items", NAMEOF('Zepto Grocery Data'[No of Items]), 2),
    
    ("Avg Rating", NAMEOF('Zepto Grocery Data'[Avg Rating]), 3)

}
-----------------------------------------------------------------------------

1. What is the total sales revenue generated?
Answer: The total sales revenue is $1.20M.

2. How many items are there in the dataset?
Answer: There are 8,523 items.

3. What is the average sales value per transaction?
Answer: The average sales value is $141.

4. What is the average rating across all sales outlets?
Answer: The average rating is 3.9.

5. Which outlet type has the highest total sales?
Answer: Supermarket Type1 has the highest total sales at $787.55K.

6. Which outlet location tier has the highest total sales?
Answer: Tier 3 has the highest total sales at 472.13K.

7. What is the most common item type based on total item weight?
Answer: Fruits & Vegetables have the highest total item weight, followed by Snack Foods.

8. How has outlet establishment growth trended over the years?
Answer: The sales trend increased significantly around 2015, peaking at $205K, before slightly declining and stabilizing.

9. Which outlet size contributes the most to total sales?
Answer: Medium-sized outlets contribute the most, with $444.79K in total sales.

10. How does the fat content of products affect average sales?
Answer: There is no significant difference; Regular fat content products have an average sales value of $141, while Low Fat products have $142.


# Dashboard 
![image](https://github.com/user-attachments/assets/ba195161-5c86-4b77-8a31-03491e6d4d60)
