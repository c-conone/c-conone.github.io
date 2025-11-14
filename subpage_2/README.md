# Tools and Technologies for Business Analytics Assignments

This repository contains a series of assignments designed to apply core concepts from the OM 620 *Tools and Technologies for Business Analytics* course at California State University San Marcos.

### Learning Objectives

- Application of data transformation techniques 

- Use of statistical models to support inventory decisions

- Documentation of analytical decisions

- Development of reproducible workflows for business analytics use cases


### Technologies and Tools Utilized

- Python (pandas, Numpy, Scipy, plotnine) for data wrangling and statistical modeling

- Markdown for documentation 

- Jupyter Notebooks for interactive analysis and code presentation


### Assignment Overview



**Assignment 1:** *Data Preparation for Safety Stock Analysis*

This assignment focuses on preapring transactional data for inventory analysis. Key tasks include:

- Standardizing inconsistent data column naming conventions

- Inspecting anf correcting anomolies in numeric data features

- Filtering dataet for Make to Stock (MTS) stock keeping units (SKUs) and extracting key operational insights for unique SKUs, manufacturing sites, and division counts as well as the top and bottom transactions by order quantity with the calculated sales value. 


**Findings:** 

Outliers were determined for both unit price and unit quantities which were handled using a combination of filtering to remove negative values for order quantities where multiple observations were found  and applying the the absolute function to unit price as few observations were found. 

Rows where SKU contained missing information were filtered out with the final filtered dataset focusing on MTS-designated finished goods, revealing: 

- 473 unique SKUs
- 15 manufacturing sites
- 66 divisions
- Order quantities ranging from 0 to 191 units
- Total sales values calculated utilizig the unit price x order quantity and the associated top and bottom 10 transactions with totals ranging from $0 to ~ $193,200. 






**Assignment 2:** *Safety Stock Calculation and Distribution Analysis*

This assignment builds on the cleaned dataset to calculate safety stock levels for Make to Stock (MTS) Stock Keeping Units (SKUs) using statistical aggregation and service level coefficents. Key tasks include: 

- Aggregating lead time and associated SKU-level statistics: min, max, mean, medianm variance and standard deviation.

- Computing safety stock using z-scores for 75%, 90%, and 95% service levels.

- Analyzing safety stock distributions to identify SKUs with the highest and lowest safety stock requirements and average safety stock values across all SKUs.


**Findings:** 

Using the aggregated and transformed data,  safety stock values for each SKU were calculated for the service level coefficients of 75%, 90%, and 95%. Safety stock distribution was then determined strictly focusing on a 95% service level as follows:

- SKU with the largest safety stock at the 95th percentile: BE575720
- SKU with the smallest safety stock at the 95th percentile: 79536466
- Average safety stock at the 95th percentile: 109

