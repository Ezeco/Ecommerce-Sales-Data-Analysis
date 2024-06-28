# E-commerce Sales Data Analysis
---
## Project Title - *Comprehensive E-commerce Sales Data Analysis*
## Project Overview
This project focuses on analyzing e-commerce sales data to identify purchasing trends, preferences by gender, and other key insights. 
The analysis highlights the most: 
- Purchased item categories
- Frequency of purchases
- Preferred payment methods
- Review ratings and common shipping types.

The primary item categories analyzed include
- Clothing
- Accessories
- Footwear
- Outerwear.

## Data Source
The data was sourced from a CSV file containing e-commerce sales records.

## Tools Used
- Power BI for data visualization and reporting
- Power Query for data cleaning and transformation
- SQL for data manipulation

## Screen shots of Data Visualization
![Screenshot (42)](https://github.com/Ezeco/Ecommerce-Sales-Data-Analysis/assets/125317057/8dc41ca2-75d7-42f1-a730-6013d97f4d50)
![Screenshot (45)](https://github.com/Ezeco/Ecommerce-Sales-Data-Analysis/assets/125317057/389c983c-40e5-4de0-80fb-3977524ce0ac)

## Data Cleaning
Data cleaning was performed using Power Query in Power BI. 
The process included:
- Renaming columns for clarity and consistency
- Standardizing the datetime format
- Dropping irrelevant or redundant columns
- Replacing empty rows with appropriate values etc.

## Explorative Data Analysis (EDA)
During EDA, several trends and insights were identified:
- Item Category Trends: Jewelry had the highest frequency of purchases, while jeans had the lowest.
- Seasonal Trends: The analysis revealed seasonal variations in the frequency and total amount of goods purchased.
- Price Impact: The relationship between prices and sales frequency was explored, showing how pricing strategies affect purchase behavior.
- Payment Methods: The highest used payment methods were identified.
- Review Ratings: Analysis of customer reviews provided insights into product satisfaction.
- Shipping Preferences: The most common shipping types were evaluated, including free shipping, standard shipping, store pickup, next day by air, express, and 2-day shipping.

## Result and Findings
- Item Categories: Jewelry emerged as the most frequently purchased category, while jeans had the least frequency
- Purchasing Trends: Seasonal trends showed peaks in purchases during holiday seasons.
- Pricing Strategy: Higher prices were generally associated with lower purchase frequency.
- Payment Methods: Credit cards were the most frequently used payment method.
- Review Ratings: Products with higher average ratings saw more frequent purchases.
- Shipping Preferences: Free shipping was the most preferred shipping option, followed by standard shipping.

## Recommendations
- Sales Performance: Focus marketing efforts on promoting jewelry and other high-frequency categories.
- Pricing Strategy: Consider dynamic pricing strategies to optimize sales across different seasons.
- Payment Options: Enhance and promote convenient payment methods to improve customer experience.
- Customer Feedback: Use review ratings to identify and address product quality issues, boosting overall customer satisfaction.
- Shipping Options: Expand free shipping and optimize other shipping methods to meet customer preferences.

## Limitations
#### Data Quality: The analysis is dependent on the accuracy and completeness of the provided data.
#### Temporal Scope: Seasonal trends might vary year by year; a longer time frame would provide more robust insights.
#### External Factors: Factors such as market trends, economic conditions, and competitor actions were not considered.

## References
Power BI Documentation: [https://docs.microsoft.com/en-us/power-bi/]

SQL Documentation: [https://www.w3schools.com/sql/]

## E-commerce Data Analysis Articles:

"Understanding E-commerce Sales Data" - Journal of Data Analysis

"The Impact of Pricing Strategies on E-commerce Sales" - E-commerce Analytics Review

# Ecommerce Sales Data Analysis Power BI Dashboard
Click on this link to view the Ecommerce Sales Data Analysis Dashboard https://app.powerbi.com/view?r=eyJrIjoiYThjYzMwYzEtMTVjYS00MTA3LWI3NmMtNTRiZjA5Y2JhZmY1IiwidCI6ImY2NWQxY2U4LTYwOTEtNDk4Ny04ZmI4LWJjM2E0MTA5MDY3NSIsImMiOjl9

### This project provides a detailed analysis of e-commerce sales data, offering actionable insights to improve sales performance, marketing strategies, and customer satisfaction.

## Data Analysis Source Code:
Below is an example of SQL queries used to derive key insights from the data:
### Sql code
-- Query to find the most purchased item categories by gender

``` SELECT gender, category, COUNT(*) AS purchase_count
FROM sales_data
GROUP BY gender, category
ORDER BY purchase_count DESC;

-- Query to find the frequency of each payment method used

SELECT payment_method, COUNT(*) AS usage_count
FROM sales_data
GROUP BY payment_method
ORDER BY usage_count DESC;

-- Query to find the review ratings

SELECT product_id, AVG(review_rating) AS average_rating
FROM sales_data
GROUP BY product_id
ORDER BY average_rating DESC;

-- Query to find the most common shipping types

SELECT shipping_type, COUNT(*) AS shipping_count
FROM sales_data
GROUP BY shipping_type
ORDER BY shipping_count DESC; ```
