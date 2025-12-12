# Advanced Visual Analytics Assignments 
 
This repository contains a series of assignments from the OM 621 Advanced Visual Analytics course at California State University San Marcos. The project centers on developing a predictive cost estimation model for WD-40’s transportation operations, using historical shipment and invoice data to support strategic decision-making across finance, procurement, and supply chain leadership.

## Learning Objectives

- Develop context artifacts (Who, What, How, pitch, Big Idea sheets, storyboard) to frame analytics problems.
- Apply data wrangling and transformation techniques to real-world supply chain datasets.
- Create and refine visualizations that reveal trends across sites, regions, and transportation modes.
- Explore time-series patterns in invoice data to inform cost estimation and forecasting.
- Document analytical decisions and build reproducible workflows for stakeholder use.
- Translate technical findings into strategic insights for finance, procurement, and leadership teams.


## Technologies and Tools Utilized

- **Python**: pandas, plotnine, datetime  
- **Jupyter Notebooks**: interactive analysis  
- **Markdown**: documentation  
- **PNG exports**: stakeholder-ready visuals  


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







