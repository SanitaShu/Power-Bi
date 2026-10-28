# Travel Insurance Claims & Sales Analysis | Power BI

## Project Overview

This project focuses on analysing travel insurance data and developing an interactive Power BI dashboard to explore sales performance, insurance claims, customer demographics and distribution channels.

The project covers the complete data analysis process, from data cleaning and preprocessing to feature development, KPI calculations and interactive data visualisation.

The dashboard is designed to provide business insights and support data-driven decision-making.

## Tools & Technologies

- **Power BI** – interactive dashboard development and data visualisation
- **Power Query** – data cleaning and transformation
- **DAX** – calculated columns, measures and data categorisation
- **Statistical analysis** – Interquartile Range (IQR) method and Chi-square test

## Dataset

The original dataset contained **63,326 records and 11 variables**, including:

- Agency and Agency Type
- Distribution Channel
- Product Name
- Claim Status
- Travel Duration
- Destination
- Net Sales
- Commission
- Gender and Age

**Data source:** [Travel Insurance Dataset](https://raw.githubusercontent.com/juschan/ml_travelclaims/master/travel%20insurance.csv)

## Data Cleaning & Preprocessing

Exploratory data analysis identified several data quality issues:

| Data Quality Issue | Findings |
|---|---|
| Duplicate records | 12,412 |
| Missing gender values | Approximately 69% |
| Invalid travel durations | 50 records |
| Extreme outliers | Duration, Age, Net Sales and Commission |
| Class imbalance | Approximately 1.28% claims vs 98.72% non-claims |

### Data Preparation Approach

- Identified and removed duplicate records.
- Detected invalid travel durations.
- Applied the **IQR method** to identify and remove extreme outliers.
- Investigated missing gender values using a **Chi-square test**.
- Created a separate "Missing" category for gender to preserve records with incomplete information.
- Considered class imbalance when interpreting insurance claim patterns.

## Feature Engineering & DAX

Additional calculated fields and measures were developed to improve analytical capabilities.

**Calculated Fields:**
- Geographic regions based on destination countries
- Travel duration categories: 1–7, 8–14, 15–30 and 30+ days
- Customer age groups: 18–24, 25–34, 35–44, 45–59 and 60+
- Aggregated sales by agency and agency type

**Calculated Measures:**
- Total Policies
- Total Net Sales
- Total Claims
- Claim Rate (%)

DAX expressions, including `SWITCH`, were used for regional classification and calculated fields.

## Dashboard Features

The interactive Power BI dashboard includes:

**Key Performance Indicators**
- Total Policies
- Total Net Sales
- Total Claims
- Claim Rate (%)

**Interactive Visualisations**
- Geographic distribution of net sales
- Net sales by agency type
- Claim rates by region
- Claims and claim rates by age group
- Policy distribution and net sales by travel duration
- Product-level sales and claims analysis

**Interactive Filters**

Users can filter the dashboard by product, region, country, agency type, agency and gender.

## Dashboard Overview

The final dashboard displays the following key metrics:

| KPI | Value |
|---|---:|
| Total Policies | Approximately 40,000 |
| Total Net Sales | 1.18M |
| Total Claims | 514 |
| Claim Rate | 1.3% |

*These values represent the processed dataset displayed in the dashboard.*

## Business Questions Addressed

The dashboard was developed to help explore the following questions:

1. Which regions generate the highest net sales?
2. Which distribution channels perform best?
3. How does travel duration relate to sales performance?
4. How do insurance claim rates vary across age groups and regions?
5. Which insurance products generate the most sales and claims?
6. What are the geographic patterns of travel insurance sales?

## Key Challenges & Learning Outcomes

This project provided practical experience in:

- Cleaning and transforming datasets with missing values, duplicates and outliers.
- Applying statistical techniques to support data preparation decisions.
- Developing calculated columns and measures using DAX.
- Working with imbalanced datasets and interpreting claim rates appropriately.
- Selecting appropriate visualisations for different business questions.
- Improving dashboard usability through iterative design and stakeholder-focused reporting.

The dashboard underwent several design iterations to improve layout consistency, readability and user experience.

## How to Use

1. Download the `.pbix` file from this repository.
2. Open it using **Microsoft Power BI Desktop**.
3. Explore the dashboard using the interactive filters and visualisations.

## Project Scope

This is a data analytics portfolio project demonstrating practical skills in data preparation, exploratory analysis, feature engineering and business intelligence reporting.
