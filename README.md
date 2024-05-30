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
5. [Advanced Analysis](#advanced-analysis)
6. [Visual Insights](#visual-insights)
7. [Conclusion](#conclusion)
8. [Appendix](#appendix)

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

*	**Loading Data from CSV**: The Adidas sales dataset is loaded into a Pandas DataFrame from a CSV file using pd.read_csv(). This method reads the CSV file and converts the structured data into a DataFrame, which is ideal for data manipulation and analysis.

**Data Cleaning and Preprocessing**: Basic preprocessing steps are carried out to ensure the data is in a suitable format for analysis.

*	**Converting Dates to DateTime Objects**: Many datasets contain date information in string format, which can be cumbersome for time-series analysis. By converting the 'Invoice Date' column to DateTime objects, we can perform more efficient date-based operations such as sorting, filtering, and aggregating data over time.

*	**Handling Categorical Data**: Transforming categorical data into a suitable format is essential for effective analysis. This involves encoding categorical variables, such as 'Gender Type' and 'Sales Method', into numerical values using techniques like one-hot encoding or label encoding. This step ensures that the data can be effectively used in various analytical and machine learning models.

These foundational steps in data handling ensure that the dataset is well-prepared for deeper analysis and visualization. By meticulously processing the data, we can perform more complex analyses that lead to actionable insights and drive strategic business decisions.
 
### Data Analysis Technique

**Descriptive Statistics:**

Descriptive statistics provide a comprehensive overview of the data through various summary metrics. These include mean, median, count, standard deviation, and more. In the context of the Adidas sales analysis, these statistics help in understanding the data distribution and key trends:
* **Mean and Median**: 
*	**Mean (Average)**: Provides an overall sense of central tendency for numerical data such as Price per Unit and Total Sales. For instance, the average price per unit can help understand the general pricing strategy, while the average total sales offer insights into revenue generation.
*	**Median:** Shows the middle value in the data distribution, helping to understand the typical sales figures and prices, especially in skewed distributions.

*	**Count:** Indicates the number of non-null entries in each column, helping to assess the completeness of the dataset and identify any columns with missing data.

*	**Standard Deviation:** Measures the variability or dispersion of a set of values. A high standard deviation in Total Sales or Units Sold indicates a wide range of sales performance, reflecting diverse customer purchasing behavior.

**Data Visualization**

Visual representations are crucial for interpreting and communicating data insights. Various plots and charts are used to visualize sales trends, customer preferences, and regional performance. Visual representations of data are used to understand trends, patterns, and outliers more intuitively. Here’s how various types of plots are employed:

*	**Bar Charts:** Used to compare the frequency or amount of different categories. For example, bar charts can illustrate the number of units sold across different product categories or the total sales in various regions. This helps in identifying the most and least popular products and regions.
*	**Pie Charts:** Effective for showing the proportional distribution of categories. Pie charts can display the percentage share of sales methods (e.g., online vs. outlet) or the distribution of sales by gender, making it easy to see dominant categories.
*	**Heatmaps:** Useful for visualizing the intensity of data and identifying patterns. Heatmaps can show the correlation between variables such as Price per Unit, Units Sold, and Total Sales, helping to uncover relationships and trends.
*	**Count Plots and Distribution Plots:** Count plots are helpful for visualizing the frequency of categorical data, such as the number of sales transactions by state or city. Distribution plots can show the distribution of numerical data like Operating Profit, highlighting common and extreme values.

These descriptive statistics and visualization techniques are fundamental for transforming raw data into actionable insights. They provide the numerical and visual tools needed to understand the data deeply, supporting strategic business decisions based on clear and comprehensible information.

### Key Findings

**User Demographics:** Analyzing the demographic data such as gender distribution across different regions provides valuable insights into customer preferences and behavior.
*	**Gender Distribution**: Understanding the distribution of sales between different genders helps tailor marketing strategies to target specific demographics more effectively. For instance, if data shows a higher proportion of sales in women's apparel in certain regions, Adidas might focus on promoting women's sportswear in those areas.
*	**Regional Preferences**: Analyzing gender-based preferences regionally can reveal cultural differences and purchasing habits that vary from one region to another, guiding localized marketing and product development efforts.

**Device Usage:** Insights into sales methods (e.g., online vs. outlet) and their popularity among different user segments.
*	**Sales Method Preferences by User Segment:** Identifying which sales methods are most preferred among different segments (e.g., online shopping among younger customers or outlet purchases among older customers) can help optimize the sales strategy for different platforms to enhance customer experience.
*	**Method-Based Purchasing Patterns:** Understanding the preferences for different sales methods can inform decisions on inventory management, customer service, and promotional activities. For example, if online sales are predominant in urban areas, efforts can be focused on enhancing the online shopping experience in these regions.


**Subscription Details:** Exploring how different product categories and price points are preferred across various user demographics.
*	**Preference for Product Categories:** Different user groups may show preferences for specific product categories (e.g., footwear vs. apparel), which can inform inventory and marketing strategies. For instance, if footwear is more popular in certain regions, Adidas might focus on expanding its footwear collection and running targeted promotions in those areas.
*	**Impact of Product Type on Sales:** Understanding how different product categories affect total sales and profit margins can help structure more appealing product offerings. For example, if higher profitability is noticed in premium footwear due to higher price points, these products could be highlighted in campaigns to boost sales.

**Regional Preferences:** Analyzing sales data across different regions provides insights into geographical market performance.
*	**High-Performing Regions:** Identifying regions with the highest sales and profit margins helps focus marketing and sales efforts on these areas to maximize revenue. For instance, if a particular state or city shows exceptional performance, Adidas might consider launching exclusive products or promotions in that region.
*	**Low-Performing Regions:** Conversely, identifying underperforming regions helps understand the challenges and devise strategies to improve sales, such as localized marketing campaigns or targeted discounts.

**Pricing and Profitability:** Understanding the relationship between price per unit, units sold, and operating profit.
*	**Optimal Pricing Strategies:** Analyzing the average price per unit and its impact on units sold and total sales helps in setting optimal prices that balance demand and profitability. For example, if reducing prices slightly leads to a significant increase in units sold and overall profit, this strategy can be adopted more widely.
*	**Profit Margin Analysis:** Understanding operating margins across different products and regions helps identify the most profitable segments, guiding future product development and marketing efforts to focus on high-margin items.

These findings provide a comprehensive view of the current sales performance and customer preferences, offering predictive insights that can help Adidas anticipate future trends and adjust its strategies accordingly. Leveraging this information effectively can lead to improved customer satisfaction, increased sales, and better financial performance through targeted marketing, optimized inventory management, and strategic pricing.

### Advanced Analysis

**Geographical Insights:** Using custom functions to categorize sales data into broader geographical regions allows for a deeper understanding of market dynamics.
*	**Categorization into Continents:** By employing custom functions to map sales data from various countries into their respective continents, the analysis can be expanded to a regional level. This categorization is essential for comparing and aggregating sales data across continents, revealing regional preferences and performance metrics. This broader view aids strategic decision-making by highlighting market penetration and customer behavior in different regions.
*	**Regional Analysis:** With continent-based categorization, Adidas can analyze regional trends such as product preferences, sales performance, and customer engagement levels. This information is instrumental in tailoring marketing campaigns, optimizing inventory, and planning strategic expansions. For example, identifying a high demand for specific products in Europe can guide localized product launches and promotional activities.

**Temporal Trends:** Analyzing sales trends over time to detect seasonal patterns in consumer behavior.
*	**Sales Trends Over Months:** Analyzing monthly sales data helps in identifying any seasonal trends or patterns in consumer purchasing behavior. For instance, sales data might show an increase during certain months, such as back-to-school seasons or holiday periods, which can be crucial for planning inventory and marketing strategies.
*	**Seasonal Patterns:** Detecting seasonal patterns in sales data helps in planning marketing strategies, promotional offers, and inventory management to maximize revenue. For example, if sales peak during summer months, Adidas might consider launching summer-specific product lines and promotions to capitalize on the increased consumer spending.

These advanced analyses leverage the dataset to understand not just the current state but also to predict and respond to future trends. By integrating geographical and temporal dimensions into the analysis, Adidas can make more informed decisions that are contextually relevant, enhancing its ability to adapt to dynamic market conditions and customer preferences effectively. This strategic approach helps in optimizing resource allocation, improving customer satisfaction, and driving overall business growth.

### Visual Insights
*	**Gender Distribution:** Count plots showing the distribution of sales by gender across different regions provide valuable insights into customer demographics.
*	**Sales Method Preference by Region:** Insights into the preferred sales methods (e.g., online vs. outlet) in different regions are crucial for strategic decision-making.
*	**Product Category Popularity:** Visualizing the popularity of different product categories among the customer base helps in understanding purchasing trends.

**Gender Distribution:**
*	**Count Plots:** These plots illustrate the distribution of sales by gender across various regions. Visualizing this distribution allows stakeholders to understand gender dynamics within the customer base, informing targeted marketing strategies and product offerings. For instance, if a region shows a predominant female customer base, promotions and product lines that appeal to women might be prioritized.
*	**Implications:** Understanding gender distribution helps tailor user experiences and promotional efforts to match the preferences and purchasing habits of different genders, potentially increasing customer engagement and satisfaction.

**Sales Method Preference by Region:**
*	**Sales Method Visualization:** Visualizing the counts or percentages of sales by method in different regions highlights regional preferences. For example, higher online sales in urban areas might indicate the need for enhanced online shopping experiences, while regions with higher outlet sales might benefit from increased store promotions.
*	**Strategic Decisions:** These insights guide decisions on where to prioritize technical support, optimize the shopping experience, and invest in partnerships with delivery services. It also influences how Adidas develops and tests new sales strategies, ensuring optimal performance in the most used sales channels.

**Product Category Popularity:**
*	**Product Category Visualization:** Bar charts or pie charts can show the distribution of sales across various product categories. This helps in understanding which categories are most attractive to customers and might reveal insights about seasonal trends or regional preferences.
*	**Business Strategy:** Knowing which product categories are popular can help in inventory management, promotional planning, and product development. For example, if footwear is particularly popular in certain areas, Adidas might focus on expanding its footwear collection and running targeted promotions to boost sales in those regions.

These visualizations not only summarize the data effectively but also serve as powerful tools for communicating findings to stakeholders. By presenting data visually, insights are made clearer and more compelling, supporting informed decision-making and strategic planning. This helps in optimizing marketing strategies, improving customer satisfaction, and driving overall business growth.

### Conclusion
This document has systematically unfolded the comprehensive analysis of Adidas sales data through various customer attributes, utilizing advanced data handling and visualization techniques to uncover key insights into consumer preferences and purchasing behaviors. By leveraging powerful Python libraries such as Pandas, Matplotlib, and Seaborn, we have transformed raw sales data into actionable intelligence that not only describes the current state of customer engagement but also forecasts future trends.

The insights derived from demographic analyses, sales method preferences, and product category popularity underscore the nuanced understanding necessary for Adidas to tailor its offerings more precisely to diverse customer needs. These findings are pivotal in shaping marketing strategies, optimizing product assortments, and enhancing overall customer experiences aimed at boosting satisfaction and retention.

Additionally, the advanced geographical and temporal analyses presented have highlighted significant patterns in sales performance that vary across different times and regions. These insights facilitate a more strategic approach to market penetration and inventory management, ensuring that Adidas products are available where and when they are most needed.

The visualization techniques employed have brought these insights to life, making them accessible and impactful for decision-makers across the organization. By presenting data visually, stakeholders can more easily understand complex trends and make informed strategic decisions.

Looking ahead, this document serves as a blueprint for continuous improvement and innovation in data-driven strategies at Adidas. It emphasizes the importance of a proactive approach to data analysis—anticipating market shifts, adapting strategies, and aligning offerings to meet the evolving demands of a global customer base. Adidas's commitment to leveraging such detailed analytics ensures that it remains at the forefront of the sportswear and fashion industry, poised for further growth and success.

In conclusion, the meticulous analysis and visualization of Adidas sales data provide invaluable insights that drive strategic decisions and foster a deeper understanding of market dynamics. By continuously refining these techniques and incorporating new data sources, Adidas can maintain its competitive edge and continue to delight customers worldwide.

### Appendix
**Code Snippet:**
<a href="Adidas.ipynb"> Adidas Sales Analysis Using Python </a>
