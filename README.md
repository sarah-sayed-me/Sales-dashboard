
# SalesCustomer Dashboard

## Project Overview

### Project Title: Customer Sales

### Project Description:
In this dashboard, we aim to identify the company's sales KPIs, analyze customer behavior, and understand the impact of shipping modes and geographical regions on sales.

### Business Objectives:
- Improve sales performance.
- Optimize shipping strategies.
- Identify high-potential markets to drive growth.

### Stakeholders:
- Sales Manager
- Marketing Team
- Supply Chain Managers

## Data Sources

### Data Origin:
Data for this project is sourced from the internal customer sales database, including order records, products, and customer data.

### Data Files:
- **Orders File**: Contains all data about orders and shipping modes, including:
  - `Order ID`, `Order Date`, `Ship Date`, `Ship Mode`, `Customer ID`, `Customer Name`, `Segment`, `City`, `Country`, `Region`, `State`, `Postal Code`, `Product ID`, `Category`, `Sub-Category`, `Product Name`, `Sales`, `Quantity`, `Discount`, `Profit`.
- **Customer File**: Contains data about customers, including:
  - `Customer ID`, `Customer Name`, `City`, `Country`, `Customer Status`, `Number of Orders`, `Postal Code`, `Region`, `Segment`, `State`.
- **Products File**: Contains:
  - `Product ID`, `Product Name`, `Category`, `Sub-Category`, `Number of Orders`.
- **Dates File**: Contains dates of orders, including:
  - `Month`, `Month Name`, `Order Date`, `Year`.

## Data Cleaning:
- **Remove Inconsistencies**: Address discrepancies in data entries to ensure uniformity.
- **Handle Missing Values**: Manage missing or incomplete data to maintain analysis accuracy.
- **Standardize Data Formats**: Ensure consistency in the formatting of dates, numbers, and text fields.
- **Validate Data Accuracy**: Cross-check data entries against the source to correct errors.

## Data Model

### Data Relationships:
- The data model connects `orders data`, `customer data`, `products`, and `dates data`.
- Customer ↔ Orders: `customer_id` is the primary key.
- Products ↔ Orders: `product_id` is the primary key.
- Dates ↔ Orders: `order_date` is the primary key.

### Data Integrity Checks:
- Validated that each `customer_id` has a corresponding balance entry.
- Checked for duplicates and removed any redundant entries.
- Ensured consistency in region naming conventions for accurate mapping.

## Visualization & Reporting:
![Screenshot 2024-10-10 184903](https://github.com/user-attachments/assets/86acc2e8-c26b-4908-8b31-3d47c98f1d94)

1. **Order Count**
   - **Visualization Type**: KPI Card
   - **Description**: Displays the total number of orders placed, which is 2,323.
   - **Purpose**: Provides a quick overview of total order volume, indicating the level of sales activity.

2. **Active Customers**
   - **Visualization Type**: KPI Card
   - **Description**: Shows the number of active customers, which is 26.
   - **Purpose**: Helps to identify the customer base contributing to sales, allowing for an understanding of engagement and retention levels.

3. **Sum of Sales**
   - **Visualization Type**: KPI Card
   - **Description**: Displays the total sales amount, which is 501.24K.
   - **Purpose**: Provides a snapshot of overall revenue, useful for assessing financial performance.

4. **Average of Sales by Category**
   - **Visualization Type**: Bar Chart
   - **Description**: Shows the average sales across different product categories like Technology, Furniture, and Office Supplies.
   - **Purpose**: Helps to identify which product categories perform better in terms of sales, assisting in product focus and marketing efforts.

5. **Sum of Quantity by Category**
   - **Visualization Type**: Donut Chart
   - **Description**: Represents the distribution of sales quantities across product categories, with Technology leading at 61.61%.
   - **Purpose**: Provides insights into the demand for different product categories, guiding inventory management and supply chain strategies.

6. **Sales Distribution by Country**
   - **Visualization Type**: Map Visualization
   - **Description**: Highlights the geographical regions where sales are occurring, with a focus on North America.
   - **Purpose**: Helps to understand the geographical distribution of sales, useful for regional marketing strategies and resource allocation.

7. **Average of Profit by Category**
   - **Visualization Type**: Bar Chart
   - **Description**: Shows the average profit across different product categories, with Technology having the highest average profit.
   - **Purpose**: Assists in identifying the most profitable product lines, aiding in pricing strategies and product development.
![Screenshot 2024-10-10 185446](https://github.com/user-attachments/assets/10960ed0-ba62-4ce9-b8cf-d8a5cab9112f)

8. **Key Influencers**
   - **Visualization Type**: Key Influencer Chart
   - **Description**: Analyzes factors that influence the increase in discounts, such as sales thresholds.
   - **Purpose**: To identify the key drivers behind changes in discount levels, which can help refine discount strategies to maximize profitability.

9. **Top Segments Suggestions**
   - **Visualization Type**: Suggestion Panel
   - **Description**: Provides options for quick analysis, like identifying top order states by order count or active customer cities.
   - **Purpose**: To guide users in exploring the data efficiently, offering insights into customer distribution and order trends by various segments.

10. **Count of Customer ID by State**
   - **Visualization Type**: Line Chart
   - **Description**: Displays the number of unique customers in different states, with Texas having the highest count.
   - **Purpose**: Helps to understand the distribution of customers geographically, guiding targeted marketing efforts in regions with higher customer density.

11. **Sum of Discount by Customer Status**
   - **Visualization Type**: Bar Chart
   - **Description**: Shows the total discounts given to active versus non-active customers, with non-active customers receiving a higher sum.
   - **Purpose**: Provides insights into how discounts are allocated across different customer groups, helping to optimize discount strategies for reactivation or retention.

12. **Order Count by State**
   - **Visualization Type**: Line Chart
   - **Description**: Displays the number of orders by state, highlighting states with the highest order counts such as Texas.
   - **Purpose**: Helps to identify key markets and regional order patterns, assisting in logistics planning and sales strategies.

13. **Month Name Selector**
   - **Visualization Type**: Slicer
   - **Description**: A month-by-month filter allowing users to narrow down the data view to specific months of the year.
   - **Purpose**: Enables time-based analysis of sales trends, customer behavior, and discount patterns, aiding in seasonal planning and forecasting.
![Screenshot 2024-10-10 202720](https://github.com/user-attachments/assets/8e52916c-1401-49e9-ab6c-a15557ee1e1a)

14. **Order Count by Segment**
   - **Visualization Type**: Donut Chart
   - **Description**: Represents the distribution of order counts across segments, such as Consumer, Corporate, and Home Office, with Consumer being the largest segment.
   - **Purpose**: Helps to understand which customer segments contribute the most to the order volume, guiding targeted sales efforts.

15. **Sum of Sales by Segment**
   - **Visualization Type**: Donut Chart
   - **Description**: Shows the total sales value by segment, with Consumer contributing to over 50% of sales.
   - **Purpose**: Provides insights into revenue distribution across different segments, aiding in identifying high-value customer groups.

16. **Sum of Discount by Segment**
   - **Visualization Type**: Donut Chart
   - **Description**: Displays the total discounts given to each segment, with Corporate receiving the highest discounts.
   - **Purpose**: Assists in analyzing discount allocation across segments, which is useful for adjusting discount strategies to improve margins.

17. **Key Influencers**
   - **Visualization Type**: Key Influencer Chart
   - **Description**: Examines factors influencing the selection of "First Class" shipping mode, highlighting that it was more likely during the years 2015-2016.
   - **Purpose**: Identifies variables that impact shipping mode preferences, helping in logistics planning and understanding customer shipping choices.

18. **Average of Profit by Category**
   - **Visualization Type**: Bar Chart
   - **Description**: Displays the average profit generated by each product category, showing Technology as the most profitable and Furniture as less profitable.
   - **Purpose**: Helps to identify the profitability of different product categories, informing decisions about product focus and pricing.

19. **Sum of Profit by State**
   - **Visualization Type**: Line Chart
   - **Description**: Shows total profit distribution across states, with Michigan having the highest profit and Texas showing a negative trend.
   - **Purpose**: Aids in understanding regional profitability, helping to adjust strategies in underperforming regions.
![Screenshot 2024-10-10 205824](https://github.com/user-attachments/assets/0b5e9a03-e8a5-4a8a-a8ab-75367ed667ee)

20. **Sum of Sales by State**
   - **Visualization Type**: Bar Chart
   - **Description**: Displays the total sales for each state.
   - **Purpose**: To identify which states contribute the most to overall sales and to compare sales performance across different regions.

21. **Sum of Sales by Sub-Category**
   - **Visualization Type**: Bar Chart
   - **Description**: Shows the total sales for each sub-category within the dataset.
   - **Purpose**: To determine which product sub-categories are driving the most revenue and to identify potential areas for growth or optimization.

22. **Sum of Discount and Sum of Profit by Category**
   - **Visualization Type**: Combined Bar Chart and Line Graph
   - **Description**: Compares the total discount and profit amounts for each product category.
   - **Purpose**: To assess the profitability of different categories, considering both revenue and discounts provided.

23

. **Sum of Quantity by Product Category**
   - **Visualization Type**: Bar Chart
   - **Description**: Displays the total quantity sold for each product category.
   - **Purpose**: To understand which categories have the highest volume of sales, which can inform stocking and sales focus.

## Key Insights and Findings

### Customer Segmentation and Sales Performance:
- **Customer Segments**: The "Consumer" segment is the most active and profitable, contributing significantly to both order volume and sales.
- **Segment-Specific Strategies**: Tailor marketing and sales efforts to cater to the unique needs and preferences of each segment.

### Shipping Mode Analysis:
- **Shipping Mode Influence**: The "First Class" shipping mode was more popular in 2015-2016, likely due to factors like pricing or delivery times.
- **Shipping Optimization**: Evaluate the impact of shipping modes on customer satisfaction and costs to optimize shipping strategies.

### Regional Sales Patterns:
- **State-Level Analysis**: Texas and California are key states in terms of both sales and order volume.
- **Regional Focus**: Prioritize marketing efforts and resource allocation in these regions to drive further growth.

### Product Performance:
- **High Performing Categories**: Technology consistently ranks as the highest-performing category in terms of sales and profitability.
- **Discount Patterns**: Non-active customers receive a higher proportion of discounts, suggesting opportunities for reactivation through targeted discount offers.

## Conclusion

### Overall Findings:
The comprehensive analysis of customer sales data has yielded valuable insights into various aspects of the business. Key findings include:
- **Customer Segmentation**: The "Consumer" segment is the most profitable, driving significant revenue.
- **Product Profitability**: Technology products consistently outperform Furniture and Office Supplies in terms of profit margins.
- **Regional Sales**: Texas and California are key markets with high sales and order volume.
- **Shipping Mode Preferences**: The "First Class" shipping mode was more popular in previous years, indicating a preference for faster delivery options.
- **Discount Strategies**: Non-active customers receive a higher proportion of discounts, suggesting opportunities for optimization.

### Impact on the Business:
The insights derived from this analysis can have a significant impact on the business by:
- **Targeted Marketing**: Enabling the development of tailored marketing campaigns for different customer segments.
- **Product Focus**: Guiding product development and investment towards high-margin product categories.
- **Regional Expansion**: Identifying high-potential regions for expansion.
- **Shipping Optimization**: Refining shipping strategies to meet customer preferences.
- **Discount Optimization**: Developing more effective discount strategies.

### Recommendations:
- **Customer Relationship Management**: Implement a robust CRM system to track customer interactions.
- **Data-Driven Decision Making**: Foster a data-driven culture within the organization.
- **Continuous Improvement**: Regularly review and update the dashboard to incorporate new data and insights.
