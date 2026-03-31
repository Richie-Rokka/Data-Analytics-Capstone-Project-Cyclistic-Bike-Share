# Cyclistic Bike-Share Analysis

## Introduction 
This project is part of the Google Data Analytics Professional Certificate on Coursera. In this case study, I apply the full data analysis process—Ask, Prepare, Process, Analyze, Share, and Act—to explore Cyclistic’s data, uncover meaningful insights, and develop practical, data-driven recommendations.

## Scenario
Urban mobility is undergoing a major transformation, with bike-share programs emerging as a sustainable and efficient alternative to traditional transportation. In cities like Chicago, systems such as Bike Share—operated under the Cyclistic(fictional) brand, have redefined how residents and visitors navigate dense urban environments. By integrating accessibility, convenience, and affordability, bike-share programs support reduced traffic congestion, lower carbon emissions, and healthier lifestyles.

Since its launch in 2016, Cyclistic has scaled rapidly, building a robust infrastructure of bikes and strategically located docking stations. However, as competition and operational costs increase, long-term profitability depends not just on ridership volume but on customer retention and recurring revenue. This case study explores how data-driven insights can help Cyclistic transition casual riders into loyal annual members—unlocking sustainable growth and strengthening its market position.

## Approach
• Cleaned and transformed trip data

•	Conducted exploratory data analysis 

•	Identified behavioral differences


# Phase 1 – Ask

## Business Task 
This project focuses on analyzing user behavior and ride patterns to improve annual membership by developing digital targeted marketing strategies using data-driven insights.

## Stakeholders
Director of Marketing - Leads Cyclistic’s marketing strategy, focusing on customer acquisition, membership conversion, and maximizing marketing ROI.

Marketing Analytics Team - Collects and analyzes ride data to generate actionable insights that support targeted marketing and customer segmentation.

Executive Team - Approves data-driven strategic initiatives that drive long-term growth, customer retention, and revenue sustainability.

# Phase 2 – Prepare

<a href="https://divvy-tripdata.s3.amazonaws.com/index.html">Data Source - Cyclistic Dataset</a>

This dataset used consists of 12 Months (January 2021 to December 2021) of  divvy-tripdata from Motivate International Inc under this <a href="https://www.divvybikes.com/data-license-agreement">License-Agreement</a> It provides comprehensive trip-level insights into Cyclistic’s operations, with variables supporting behavioral and trend analysis. Organized across a year generated data and excluding PII, it enables secure, aggregate-level analysis of rider patterns. The data also follows the ROCCC approach –


Reliable - The dataset includes complete and accurate ride data from divvy-tripdata used by Cyclistic’s internal systems, ensuring a high level of accuracy, consistency, and operational reliability.

Original - This is first-party data provided by Motivate International Inc. under the Divvy Bikes licensing framework, ensuring authenticity.

Comprehensive - The dataset includes all critical variables needed for analysis, such as time, location, bike type, and user segmentation, allowing for a well-rounded behavioral analysis.

Current - It captures recent 12-month period, making it suitable for identifying current trends and usage patterns.

Cited - The data is publicly available and properly documented, ensuring transparency and credibility for analysis and reporting under the <a href="https://www.divvybikes.com/data-license-agreement">License-Agreement</a>


# Phase 3 – Process

The 12 CSV files from divvy-trip data (January 2021 to December 2021) were stacked and combined into a single dataset. The DataFrame consists of 5,595,075 rows after the data consolidation.

Before analysis, the dataset was cleaned and transformed to ensure accuracy, consistency, and usability. Given that the data was collected across multiple files, part of the steps involved consolidating all datasets into a single, structured dataset for efficient analysis.

## Data Cleaning Steps-

•	Data Consolidation - Merged the 12 monthly datasets into one unified table to enable a full year trend analysis while I removed the columns for latitude and longitude.

•	Handling Missing Values - Identified and replaced records with null or incomplete fields "missing station names" with “unknown station name” to maintain data quality. 

•	Removing Duplicates - Checked for and eliminated duplicate ride entries to ensure data integrity. 

•	Standardizing Data Formats - Converted date and time fields into a consistent format and ensured uniform naming conventions across all variables. 

•	Filtering Invalid Records - Removed rides with negative or zero ride durations, less than one minute, or extended beyond twenty-four hours.

## Feature Engineering

To support deeper analysis, additional variables were created:

•	Ride Length - Calculated as the difference between end time and start time 

•	Day of Week - Extracted to analyze weekly usage patterns 

•	Month - Derived to identify seasonal trends 

•	Start of ride hour – Derived to identify rush hour rides

These new features enabled more meaningful insights into customer behavior and ride patterns.

The final dataset made available for the analysis consists of 5,504,784 rows after cleaning, validation, and 90,291 rows were removed during the cleaning process.

