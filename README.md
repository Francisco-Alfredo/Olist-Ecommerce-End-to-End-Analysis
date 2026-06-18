# Olist E-commerce Data Analysis

This notebook performs an end-to-end analysis of the Olist e-commerce public dataset. The goal is to understand various aspects of the business, including customer behavior, order fulfillment, payment trends, and product performance.

## Table of Contents

1.  **Project Description**
2.  **Data Loading**
3.  **Data Cleaning and Preprocessing**
4.  **Key Performance Indicators (KPIs) Analysis**
    *   1.1 Average review score by product category
    *   1.2 Payment type and Review score distribution
    *   1.3 Monthly Revenue Trend Analysis
    *   1.4(a) On-Time Delivery Rate
    *   1.4(b) Monthly On-Time Delivery
    *   1.5 Order Cancellation Rate
    *   1.6 Monthly cancellation trend
    *   Distribution of City Delay

## 1. Project Description

This project analyzes the Olist E-commerce dataset, focusing on various operational and customer-centric metrics. The analysis aims to provide insights into sales trends, delivery performance, customer satisfaction, and areas for potential improvement.

## 2. Data Loading

The notebook begins by loading multiple CSV files from the Olist dataset into pandas DataFrames. These files include information about customers, geolocation, orders, order items, payments, products, sellers, and product categories.

## 3. Data Cleaning and Preprocessing

*   **Date Column Conversion**: Several date-related columns in the `df_orders` DataFrame are converted to datetime objects for proper temporal analysis.
*   **Missing Values**: An audit of null values is performed to understand the completeness of the data. Specific attention is given to null values in delivery dates, which are often indicative of different order statuses (e.g., canceled, shipped).
*   **Data Merging**: All relevant DataFrames are merged into a single comprehensive DataFrame (`df`) to facilitate integrated analysis.
*   **Feature Engineering**: New features such as `delivery_days`, `delivery_delay`, `Total_price_value`, `order_month`, and `order_year` are created to support KPI calculations.

## 4. Key Performance Indicators (KPIs) Analysis

### 1.1 Average review score by product category

This section calculates and displays the average review score for each product category, providing insights into customer satisfaction per product type.

### 1.2 Payment type and Review score distribution

Visualizations are generated to show the distribution of payment types used by customers and the overall distribution of review scores.

### 1.3 Monthly Revenue Trend Analysis

This analysis tracks the total revenue generated each month, highlighting trends, peaks, and troughs in sales over time.

### 1.4(a) On-Time Delivery Rate

Calculates the percentage of orders delivered on time and the average delay for late orders.

### 1.4(b) Monthly On-Time Delivery

Visualizes the on-time delivery rate on a monthly basis, showing trends in delivery performance over time.

### 1.5 Order Cancellation Rate

Determines the overall cancellation rate of orders and provides a breakdown of all order statuses.

### 1.6 Monthly cancellation trend

Illustrates the monthly cancellation rate, helping to identify periods with higher cancellation frequencies.

### Distribution of City Delay

Analyzes the total delivery days accumulated by customer city, identifying cities with significantly higher or lower delivery times.
