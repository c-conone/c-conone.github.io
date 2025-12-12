# Advanced Visual Analytics Assignments 
 
This repository contains a series of assignments from the OM 621 Advanced Visual Analytics course at California State University San Marcos. The project centers on developing a predictive cost estimation model for WD-40’s transportation operations, using historical shipment and invoice data to support strategic decision-making across finance, procurement, and supply chain leadership.

## Learning Objectives

- Develop context artifacts (Who, What, How, pitch, Big Idea sheets, storyboard) to frame analytics problems.
- Apply data wrangling and transformation techniques to real-world supply chain datasets.
- Create and refine visualizations that reveal trends across sites, regions, and transportation modes.
- Explore time-series patterns in invoice data to inform cost estimation and forecasting.
- Document analytical decisions and build reproducible workflows for stakeholder use.
- Translate technical findings into strategic insights for finance, procurement, and leadership teams.
- Apply end‑to‑end analytics workflows by integrating Python preprocessing with Power BI visualization and reporting
- Develop interactive dashboards that transform raw aviation data into structured insights for decision‑making



## Technologies and Tools Utilized

- **Python**: pandas, plotnine, datetime  
- **Jupyter Notebooks**: interactive analysis  
- **Markdown**: documentation  
- **PNG exports**: stakeholder-ready visuals  
- **Power BI (Power Query, DAX)**: for data modeling, interactive dashboards, multi‑page reports, and custom slicers/tooltips



## Assignment 1: Context Artifacts and Problem Framing

### Case Background  
WD-40, a prominent San Diego-based company, faces recurring challenges in budgeting and forecasting transportation costs. Shipments—whether internal transfers or customer orders—are handled by third-party logistics providers across multiple modes (air, truck, container). However, invoice delays of weeks or months prevent timely cost visibility, creating ripple effects across finance, procurement, and executive planning.

### Who, What, and How  
- **Who**: Director of Supply Chain at WD-40  
- **What**: Transportation cost estimation and forecasting across divisions, vendors, and modes  
- **How**: Develop a predictive model using historical shipment and invoice data, integrated into planning workflows

### Audience Understanding  

To better understand the director of supply chain and their priorities:

1. Conduct stakeholder interviews to uncover pain points and decision timelines  
2. Review internal budgeting and procurement workflows to identify data bottlenecks  
3. Analyze historical shipment and invoice data to surface patterns and anomalies

### Data Needs  

To support this business problem, the following features are required:

- Shipment-level details: site, region, destination, shipping date, transportation mode  
- Invoice-level details: invoice date, invoice amount (USD-adjusted)  
- Derived features: delay (invoice date − shipping date), cost breakdowns by division, vendor, and mode

### 3-Minute Story  

> *What was the costliest shipment WD-40 made last quarter? If you had to pause and think—or wait for an invoice to tell you—you’re not alone. Your company is flying blind when it comes to transportation costs. This isn’t due to negligence, but because the data arrives too late to act on.*  
>  
> *Multiple departments are impacted: finance can’t forecast, procurement can’t negotiate, and leadership lacks visibility. Our consulting team is building a predictive cost estimation model that delivers actionable insights within days of shipment initiation. It’s not just a rough guess—it’s a tailored breakdown by division, vendor, and mode, built on your historical data and designed to integrate into your planning workflows.*  
>  
> *This solution empowers WD-40 to allocate costs before invoices arrive, maintain transparency across divisions, and make smarter decisions in real time.*

### Storyboard  

The dashboard development process follows a structured seven-step workflow:

1. Hold Initial Stakeholder Meeting & Define Project Scope  
2. Data Collection & Analysis  
3. Create Model / Develop Dashboard  
4. Demo Dashboard to Stakeholders  
5. Collect / Implement Dashboard Feedback  
6. Final Dashboard Delivery, Implementation, and Training  
7. Evaluate Dashboard Performance  

### Success Criteria  

A successful solution will:
- Provide cost visibility within days of shipment initiation  
- Enable breakdowns by division, vendor, and mode  
- Support proactive budgeting and negotiation  
- Integrate seamlessly into WD-40’s planning workflows

---

## Assignment 2: Delay Feature Engineering and Exploratory Analysis  

This phase introduced a stakeholder-provided dataset containing shipment and invoice details across sites, regions, and transportation modes.

### Key Tasks:

- **Expectation Review**: Compare dataset to initial assumptions and identify mitigation strategies  

- **Exploratory Analysis**: Assess data completeness and summarize invoice amounts  

- **Visual Insights**:  
  - Transportation volume by site and region  
  - Mode utilization trends  

- **Delay Feature Creation**:  
  - Derived from shipping and invoice dates  
  - Explored across regions, sites, and invoice amounts  

- **Mode-Based Delay Analysis**:  

  - Distribution of delays by transportation mode

### Notable Findings:

- Delay patterns vary significantly by region and mode  
- Invoice amounts show moderate correlation with delay  
- Data cleaning included date parsing, null filtering, and categorical refinement

---

## Assignment 3: Delay-by-Mode and Invoice Time Series Forecasting  
Building on the delay analysis, this assignment focused on visualizing delay distributions and uncovering time-series patterns in invoice data.

### Key Tasks:

- **Delay Distribution by Mode**:  

  - Ordered boxplots with refined themes and axis labels  
  - Exported visuals for stakeholder review  

- **Invoice Time Series Analysis**:  

  - Explored seasonality and trends using small multiples  
  - Refined final visual and exported to plots folder  

- **Forecasting Insights**:  

  - Evaluated cost estimation potential based on observed patterns  
  - Compared trends across transportation modes

### Notable Findings:

- Air modes exhibit distinct delay profiles compared to ground and container modes  
- Invoice time series reveal seasonal fluctuations and regional nuances  
- Final visuals support cost forecasting and strategic planning


## Power BI Dashboard Project: Aviation Accident Trends in California (2019)

This project analyzes aviation accident trends in California during 2019 to identify contributing factors across aircraft, environmental, and human dimensions. Using Python for data preparation and Power BI for interactive visualization, the work demonstrates a full analytics workflow from raw data to actionable insights.

- Data Cleaning & Transformation: Combined non-incident and accident flight records, standardized columns, removed duplicates/NaN values, and merged datasets.

- Visualizations (plotnine): Bar charts showing monthly accident counts and findings categorized by aircraft features, personnel, and environmental issues.

- One-Pager Report: Summarizes project scope, workflow, and key visualizations in a concise two-column format.
Power BI Dashboard

- Data Prep & Modeling: Imported cleaned Python outputs into Power Query; built relationships across fact and dimension tables (Accident, Aircraft, Engines, Events, Findings).

- Interactive Pages: Multi-page dashboard with slicers, definitions page, and edited visuals for clarity.

### Key Insights:

- ~0.006% of 1.96M flights in 2019 had accidents in California, with August as the peak month.
- Cessna 172 aircraft with Lycoming O-320 engines showed the highest accident frequency.
- Environmental conditions (dew point near 0°F and 55°F) correlated with accident peaks.
- Human factors, especially operator task performance, were the most significant contributors.




