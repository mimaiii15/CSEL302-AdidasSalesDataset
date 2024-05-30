# CSEL 302 Final Project: Data Analysis and Visualization
*  **Coladilla, Jandrei V.**
*  **Vargas, Mairene Rose B.**
*  **BSCS-2A**

##  TOPIC: Adidas Sales Analysis
## Table of Contents

1. [Project Overview](#project-overview)
2. [Libraries and Data Handling](#libraries-and-data-handling)
3. [Data Analysis Technique](#data-analysis-technique)
4. [Key Findings](#key-findings)
5. [Advance Analysis](#advance-analysis)
6. [Visual Insights](#visual-insights)
7. [Conclusion](#conclusion)

### Project Overview
The analysis aims to explore key sales attributes such as Retailer, Region, Gender Type, Product Category, Price per Unit, Units Sold, Total Sales, Operating Profit, and Sales Method. The goal is to derive insights into sales performance, customer preferences, and market trends.

The analysis of Adidas sales data leverages several key attributes to uncover patterns and preferences among the customer base. This approach aims to understand user behavior and market trends, informing strategic business decisions. Here's how each attribute contributes to understanding user behavior:

1.	**Retailer**: Analyzing the performance of different retailers helps identify which ones drive the most sales and profit. Understanding retailer performance can inform partnerships and distribution strategies.
2.	**Region**: By examining sales data across various regions, we can tailor marketing and inventory strategies to specific geographical areas. Regional analysis can reveal which areas have the highest demand for certain products.
3.	**Gender Type**: Understanding gender-based preferences allows for targeted marketing and product recommendations. Identifying which products are more popular among men or women can guide future product development and promotional campaigns.
4.	**Product Category**: Analyzing the popularity and sales of different product categories helps in understanding customer preferences. This insight can guide product stocking decisions and highlight which categories to invest in further.
5.	**Price per Unit**: Examining how different price points affect sales can provide insights into pricing strategies. Understanding the relationship between price and demand helps in setting optimal prices to maximize revenue.
6.	**Units Sold**: Tracking the number of units sold for various products helps in identifying best-sellers and understanding overall market demand. This data is crucial for inventory management and forecasting future sales.
7.	**Total Sales**: Analyzing total sales figures gives a comprehensive view of revenue generation and financial health. It helps in evaluating the effectiveness of sales strategies and identifying high-revenue products.
8.	**Operating Profit and Margin**: Understanding operating profit and margin helps in assessing the profitability of different products and sales strategies. This analysis can highlight areas where cost management can improve profitability.
9.	**Sales Method**: Evaluating different sales methods (e.g., online, outlet) provides insights into which channels are most effective. This can guide future investments in sales infrastructure and marketing efforts.

By analyzing these attributes, we can tailor business strategies to better meet market demands, optimize inventory management, and improve marketing efforts. This detailed analysis supports strategic business decisions and enhances customer satisfaction by aligning offerings more closely with user preferences and market trends.

### Libraries and Data Handling

**Libraries Used**: Pandas for data manipulation, Matplotlib and Seaborn for data visualization.

1.	**Pandas**: Pandas is essential for data manipulation and analysis. It provides data structures such as DataFrames that allow for efficient manipulation of large datasets. In this project, Pandas is used to handle, clean, and preprocess the Adidas sales data.
2.	**Matplotlib**: Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. It is used here to generate a variety of plots and charts that help in visualizing sales trends and patterns.
3.	**Seaborn**: Seaborn is built on top of Matplotlib and provides a high-level interface for drawing attractive and informative statistical graphics. It is particularly useful for creating complex visualizations that enhance the understanding of data distributions and relationships.

**Data Loading**: Data is loaded from a CSV file into a Data Frame.

•	**Loading Data from CSV**: The Adidas sales dataset is loaded into a Pandas DataFrame from a CSV file using pd.read_csv(). This method reads the CSV file and converts the structured data into a DataFrame, which is ideal for data manipulation and analysis.

**Data Cleaning and Preprocessing**: Basic preprocessing steps are carried out to ensure the data is in a suitable format for analysis.

•	**Converting Dates to DateTime Objects**: Many datasets contain date information in string format, which can be cumbersome for time-series analysis. By converting the 'Invoice Date' column to DateTime objects, we can perform more efficient date-based operations such as sorting, filtering, and aggregating data over time.

•	**Handling Categorical Data**: Transforming categorical data into a suitable format is essential for effective analysis. This involves encoding categorical variables, such as 'Gender Type' and 'Sales Method', into numerical values using techniques like one-hot encoding or label encoding. This step ensures that the data can be effectively used in various analytical and machine learning models.

These foundational steps in data handling ensure that the dataset is well-prepared for deeper analysis and visualization. By meticulously processing the data, we can perform more complex analyses that lead to actionable insights and drive strategic business decisions.
 

