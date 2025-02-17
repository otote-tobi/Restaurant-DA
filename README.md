# Restaurant Business Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sourcing](#data-sourcing)
- [Tools](#tools)
- [Methodology](#methodology)
  - [Data Cleaning & Preprocessing](#data-cleaning--preprocessing)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Data Visualization](#data-visualization)
  - [Statistical Analysis](#statistical-analysis)
- [Results and Findings](#results-and-findings)
- [Recommendations](#recommendations)

## Project Overview
Data for a 3-month period, between Jan. 1st and March 31st was collected and analyzed. 
This project aims to analyze restaurant sales and order patterns to uncover insights that can help 
business owners make data-driven decisions. 

## Data Sourcing
The data was sourced from two relatable databases: `menu_items.csv` and `order_detail.csv`, 
which were later merged into a single CSV file called `restr_df.csv`. This new dataframe contained
12,097 rows and 8 columns.

## Tools
- Pandas
- Matplotlib
- Numpy
- Jupyter Lab
- Excel

## Methodology
### Data Cleaning & Preprocessing
Handling missing values, converting date/time formats, and ensuring data consistency.

### Exploratory Data Analysis (EDA)
Using Pandas and Matplotlib to visualize sales trends, order distributions, and revenue patterns. 
The following questions were answered:

#### **Sales Performance & Revenue**
1. What are the top 10 best-selling items? 
2. What are the least popular items? 
3. Which category generates the highest revenue? 
4. How do sales vary over time (daily, weekly, and monthly)? 
5. What are the peak ordering hours? 
6. What is the average order value? 
7. How many unique items are sold per order on average? 
8. How does the price distribution of menu items look? 
9. What is the relationship between item price and order frequency? 

#### **Customer Behavior & Trends**
10. Are there seasonal trends in sales? 
11. Which days of the week have the highest sales? 
12. How does item popularity vary by time of day?
13. How often do customers order high-priced vs. low-priced items? 
14. Do specific food categories sell better at certain times of the day? 

#### **Operational Efficiency**
15. Are there any patterns in order volume that could help optimize staffing? 
16. How many orders are placed per day, and what are the busiest hours? 
17. Are there menu items that rarely get ordered and should be reconsidered? 

#### **Profitability & Pricing Strategy**
18. Are higher-priced items selling well, or do lower-priced items dominate sales? 
19. What is the total revenue contribution of each menu category? 

### Data Visualization
Implementing bar charts, line graphs, pie charts, histograms, and scatter plots for better insights.

### Statistical Analysis
Identifying correlations between price, order frequency, and time-based sales variations. 

## Results and Findings
The results are summarized as follows:
- The top three most selling items are **Korean Beef Bowl, Spaghetti & Meatballs, and Tofu Pad Thai** 
  while the least three selling items are **Chicken Tacos, Potstickers, and Cheese Lasagna**, by order volume.
  ![Top 10 best selling items](https://github.com/user-attachments/assets/d9a6f62f-6582-4761-9760-1418b5787387)

  ![Ten least popular items](https://github.com/user-attachments/assets/3b08073f-d1dc-4a4b-a3a0-89d94b0509b8)

- **Italian and Asian** food categories generate over 50% of the total revenue while **American** food generates the least revenue.
  ![Highest revenue by category](https://github.com/user-attachments/assets/689e75b1-93aa-4d3d-9684-17cf16d9d0bd)

- The days, weeks, and months with the highest sales were either in **January or March**.
  **February** experienced lower sales numbers compared to the other two months.
- **Peak ordering hours** are between **12 PM and 5 PM** daily. 
- **Monday, Friday, and Sunday** have the highest order volumes, with **Wednesday and Saturday** being the lowest.
  ![Daily_Weekly_Monthly sales trend](https://github.com/user-attachments/assets/e8875a24-f01e-48b6-a338-b9cb61cbd83b)
![HDM patterns in order volume](https://github.com/user-attachments/assets/2dc20191-1573-43d0-9d60-77ebc1c754fd)

- The **average value** of a single item on the menu is **$13.16**.
  ![price distribution of menu items](https://github.com/user-attachments/assets/6037d9c6-9ccc-4d0b-870f-91008acdd439)

- As price increases, order frequency **slightly decreases**, but the effect is very weak.
  ![Price vs Order frequency correlation](https://github.com/user-attachments/assets/2157049a-c2e5-44fd-9c37-47269f09e654)

- Customers order more **mid-range priced** items than any other price category.
- Mid-priced items are more likely to sell best between **12 noon and 5 PM**. The trend is also similar for 
  low and high-priced items, but the number of items ordered is generally less than mid-priced items.
  ![Order Trends by Price Category Over Time](https://github.com/user-attachments/assets/21cd2729-6d17-4484-b964-157da6cc2511)

- Specific food categories do not sell differently from other food categories at different times of the day. 
  However, **Asian food is most ordered all day**, while **American food is least ordered**.
  ![Order trend by category over time](https://github.com/user-attachments/assets/025f3128-1f2e-43ca-95e6-59152088ebea)
- However, one three out of the eight food items in the Asian category are priced between $5-$12
![Price Distribution of Top Ordered Asian Dishes](https://github.com/user-attachments/assets/977a95b8-c969-453d-b916-961eaa694efd)

- The three most ordered items by time of day are **Edamame, Tofu Pad Thai, and Cheeseburger** between **12 and 1 PM**.

## Recommendations
- More of the top three selling items should be stocked in high volumes, 
  while more advertisements are necessary for the three least selling items.
- More items in the leading food categories need to be added to the menu to 
  cater to customers and add excitement to the menu.
- If yet unknown, **investigations need to be carried out into the cause of poor sales in February**.
- More staff should be on duty during **daily peak order periods**.
- If yet unknown, **investigations need to be carried out into the cause of
  low order volumes on Wednesday and Saturday**.
- More items priced between **$12 and $16** should be included on the menu.
- Between **90 to 100 servings** of **Edamame, Tofu Pad Thai, and Cheeseburger** should be ready for serving before noon.

