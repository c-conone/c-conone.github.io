# Business Analytics & Visual Insights Projects E-Portfolio

This repository hosts a collection of student projects and assignments focused on data-driven decision making. It showcases Python, SQL, and Power BI workflows with clear visuals, practical insights, and documentation designed for learners, professionals, and anyone interested in analytics.

In addition to collaborative coursework, this repository features a personal showcase of analytics capabilities, including custom-built dashboards, exploratory data analyses, and workflow prototypes. These projects reflect individual strengths in statistical modeling, data storytelling, and technical documentation, offering a curated view of applied business analytics in action.



# Tools and Technologies for Business Analytics Assignments

This om620_assignments repository contains assignments from the OM 620 *Tools and Technologies for Business Analytics* course at California State University San Marcos. The work emphasizes practical applications of data transformation, statistical modeling, and reproducible workflow design. Assignments progress from cleaning transactional datasets to calculating safety stock levels using service level coefficients, highlighting reproducible, well‑documented approaches for turning raw data into actionable insights in supply chain and inventory management.  


## Learning Objectives

- Application of data transformation techniques 

- Use of statistical models to support inventory decisions

- Documentation of analytical decisions

- Development of reproducible workflows for business analytics use cases


## Technologies and Tools Utilized

- **Python**: pandas, Numpy, Scipy, plotnine

- **Markdown**: documentation 

- **Jupyter Notebooks**: interactive analysis and code presentation

---

## Assignment 1: Data Preparation for Safety Stock Analysis

This assignment focuses on preapring transactional data for inventory analysis. 

### Key Tasks:

- Standardizing inconsistent data column naming conventions

- Inspecting anf correcting anomolies in numeric data features

- Filtering dataet for Make to Stock (MTS) stock keeping units (SKUs) and extracting key operational insights for unique SKUs, manufacturing sites, and division counts as well as the top and bottom transactions by order quantity with the calculated sales value. 


### Notable Findings:


Outliers were determined for both unit price and unit quantities which were handled using a combination of filtering to remove negative values for order quantities where multiple observations were found  and applying the the absolute function to unit price as few observations were found. 

Rows where SKU contained missing information were filtered out with the final filtered dataset focusing on MTS-designated finished goods, revealing: 

- 473 unique SKUs
- 15 manufacturing sites
- 66 divisions
- Order quantities ranging from 0 to 191 units
- Total sales values calculated utilizig the unit price x order quantity and the associated top and bottom 10 transactions with totals ranging from $0 to ~ $193,200. 


---


## Assignment 2: Safety Stock Calculation and Distribution Analysis

This assignment builds on the cleaned dataset to calculate safety stock levels for Make to Stock (MTS) Stock Keeping Units (SKUs) using statistical aggregation and service level coefficents. 


### Key Tasks:

- Aggregating lead time and associated SKU-level statistics: min, max, mean, medianm variance and standard deviation.

- Computing safety stock using z-scores for 75%, 90%, and 95% service levels.

- Analyzing safety stock distributions to identify SKUs with the highest and lowest safety stock requirements and average safety stock values across all SKUs.


### Notable Findings: 

Using the aggregated and transformed data,  safety stock values for each SKU were calculated for the service level coefficients of 75%, 90%, and 95%. Safety stock distribution was then determined strictly focusing on a 95% service level as follows:

- SKU with the largest safety stock at the 95th percentile: BE575720
- SKU with the smallest safety stock at the 95th percentile: 79536466
- Average safety stock at the 95th percentile: 109






