# Amazon Products Ratings and Review Analysis

## Project Overview

This repository contains information and resources related to the analysis carried out on a dataset cointaining over 1,000 Amazon products ratings and reviews as per their deatils listed on the official website of Amazon.
Working on this project allowed for the following to be carried out on the dataset:

- Dataset Walkthrough
- Understanding Dataset Hierarchy
- Data Preprocessing
- Exploratory Data Analysis
- Data Visualization

The project was carried out using **Power Query** for data transformation and **Power BI** for visualizing insights.  
It also involved the use of **DAX** for calculations and logical measures.

---

## Tools Used

- **Power Query** — data transformation and cleaning  
- **Power BI** — dashboard creation and visualization  
- **DAX** — calculated measures and analytics  

---

## Project Goal

The primary goal of this project is to analyss the data within the dataset, derive various insight in the process and visualize insights through an **interactive Power BI dashboard**.

The final interactive dashboard will 

1. Top Performing Products by Rating
Description: Identify the products with the highest average ratings.
2. Price vs. Rating Analysis
Description: Compare the relationship between actual price, discounted price, and product rating.
3. Category Performance
Description: Determine which product categories have the highest average rating and the highest number of reviews.
4. Product Popularity by User Engagement
Description: Identify the most popular products based on the number of unique users who have reviewed them.
5. Generate all the following necessary KPIs:

- Total products
- Total category
- Total reviews
- Average rating
- Maximum average rating
- Minimum average rating
- Number of prducts with 5 star rating
- Average actual price
- Average discounted price
- Average discount percentage
- Price of most expensive product
- Price of cheapest product
- Highest amount saved on a product
- Number of products without discounts

---

## Features

- Three-page **interactive Power BI dashboard**
- Slicers for:
  - Rating
- Toggle buttons for **Review count distribution across category / Average customer rating by product category**
- Page navigation buttons
- Separate file containing all **DAX formulas**

---

## Data

### Raw Dataset

Amazon product ratings and reviews Dataset:  
https://github.com/ifioklee/Amazon-Products-Rating-and-Review-Analysis./tree/main/Data

### Power BI Dashboard

Interactive Power BI file:  
https://github.com/ifioklee/Amazon-Products-Rating-and-Review-Analysis./blob/main/Amazon%20Products%20Ratings%20%26%20Reviews%20Analysis.pbix

### Amazon Sales – DAX Measures

File cotaining all DAX formulas: 
https://github.com/ifioklee/Amazon-Products-Rating-and-Review-Analysis./blob/main/Amazon%20Sales%20%E2%80%93%20DAX%20Measures

---

## Technical Details

### Data Preparation & Transformation (Power Query)

#### Amazon sales Table

Transformations applied:
- Import CSV file into Power Query
- Split category column by delimitter using the left most delimitter
- Rename category.1 to category
- Create new discounted price column by example to have price column without the currency symbol
- Rename new column to discounted price and delete previous discounted price column and change data type to fixed whole number
- Repeat the last two steps for the "actual_Price" column
- Remove errors from rating column
- remove empty rows from rating_count column
- Remove the following columns: about_product, user_name, review_title, review_content, img_link, product_link
- create a column named column with the custom column feature
- close and apply

---

## Visualizations in Power BI

### Page 1
#### KPI cards:
- Total products
- Total category
- Total reviews
- Average rating
- Maximum average rating
- Minimum average rating
- Number of prducts with 5 star rating
  #### Stacked bar chart:
  - Average rating by product category
  - Review count distribution across categories
  - Products with average ratings
  #### Slicers:
  - Rating
- Navigation buttons to Pages 2 & 3

---

### Page 2
#### KPI cards:
- Average actual price
- Average discounted price
- Average discount percentage
- Price of most expensive product
- Price of cheapest product
- Highest amount saved on a product
- Number of products without discounts
  #### Line and Clustered charts:
  - Price VS Ratings 
  #### Slicers:
  - Rating
  - Navigation buttons to Pages 1 & 3

---

### Page 3
#### Clustered bar chart:
- Most popular products by unique reviewers
### Stacked Column Chart
- Average saving by category
- Slicers:
  - Rating
- Navigation buttons to Pages 1 & 2

---

## Results & Insights



---


