# Athletic Sales Analysis

## Overview
The athletic sales analysis looks at 2020 and 2021 sales data to analyze and understand top sales by region, retailer, and a focus on women's athletic footwear.

## Description
This code will analyze sales data to gain insights into which cities in the U.S. have sold the most athletic wear over two years and determine which retailers had the greatest total sales for athletic wear, and which retailers sold the most women's athletic footwear. Finally, the code determines which day and week had the highest sales for women's athletic footwear.

## 1. Combine and Clean Data
In order to analyze the sales information, first two csv files are read in - one for 2020 and another for 2021.  The two files are then reviewed as well as the data types.  Since both files have the same columns and data types they are combined into a single DataFrame.  The invoice_date column is updated to a datetime data type to enable the analysis needed. 

## 2. Determine which Region Sold the Most Products
Two approaches are utilized to determine which region sold the most products - groupby and pivot table.  Both approaches show that New York City in the Northeast sold the most products.

## 3. Determine which Region Had the Most Sales
The two approaches are also utilized to show which region had the most sales.  New York City also had the most sales. 

## 4. Determine which Retailer Had the Most Sales
Both the groupby and pivot table approaches show that West Gear out of San Francisco was the retailer with the most sales.

## 5. Determine which Retailer Sold the Most Women's Athletic Footwear
To determine which retailer sold the most women's athletic footwear, the base DataFrame is filtered for women's athletic footwear. Both groupby and pivot table approaches show West Gear out of San Francisco was the retailer with the most women's athletic footwear.

## 6. Determine the Day with the Most Women's Athletic Footwear
To determine the day with the most women's athletic footwear, a pivot table is created that compiles sales by invoice date. The result is sorted by value to determine that 7/16/2021 had the highest sales.

## 7. Determine the Week with the Most Women's Atheletic Footwear
The daily data is then resampled by week to determine the week of 12/19/2021 had the most women's athletic footwear sales.