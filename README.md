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


# Phase 4 – Analyze

## Data Analysis

- Total Rides & Average Ride Length Patterns in  year 2021

<img width="1500" height="1200" alt="Total Ride Stats" src="https://github.com/user-attachments/assets/c0453833-8c1b-4684-894e-13871f36fb52" />

• Casual riders tend to have significantly longer ride durations, averaging 29.96 minutes compared to 13.57 minutes for members, indicating a stronger preference for leisure and exploratory use rather than routine commuting.

• Annual members typically take shorter, more frequent trips, indicating routine usage such as commuting. The annual members accounted for 55% of the total ride.

- Hourly Ride Trends

<img width="708" height="319" alt="Hourly Stats" src="https://github.com/user-attachments/assets/bb5a014e-d78a-4522-a6c6-9d1e213b90b5" />

•	Casual riders show a steady increase in activity throughout the day, peaking in the late afternoon around 5 PM, reflecting flexible, leisure-driven usage patterns.

• In contrast, members exhibit distinct peak hours at around 8 AM and 5 PM, aligning with typical commute times to and from work, which highlights more structured, routine usage behavior.

- Daily Ride Trends
  
<img width="1500" height="1200" alt="Daily Stats" src="https://github.com/user-attachments/assets/2df0f24a-97d3-48cb-9492-78d2f32a63b0" />

• Members demonstrate consistent and frequent usage patterns, typically riding on a daily or weekly basis, with peak activity during weekday mornings and evenings—clear indicators of commuting behavior. Notably, Wednesdays record the highest ride volume (469,431 rides), while average ride duration peaks on Sundays (15.53 minutes), suggesting occasional leisure use alongside routine trips.

• In contrast, casual riders exhibit more irregular and leisure-driven usage, with activity concentrated around weekends and special occasions. Saturdays show the highest ride volume (549,630 rides), and average ride duration is longest on Sundays (35.19 minutes), reinforcing the pattern of extended, recreational rides.
  
- Monthly Ride Trends
  
<img width="1500" height="1200" alt="Monthly Stats" src="https://github.com/user-attachments/assets/64c892c1-552f-4173-b919-50b7cb32a3ff" />

•Cyclistic usage exhibits clear seasonal trends across both user groups, with ridership at its lowest in February 2021, where members recorded 38,522 rides and casual riders 9,901 rides, reflecting reduced demand during winter months.

• Activity peaks during the summer, with members reaching their highest usage in September 2021 (385,779 rides), while casual riders peak earlier in July 2021 (435,779 rides). This pattern suggests that casual riders are more influenced by seasonal and recreational factors, whereas members maintain relatively consistent, routine-driven usage throughout the year.

# Phase 5 – Share

<img width="1200" height="1200" alt="Riders&#39; Analysis" src="https://github.com/user-attachments/assets/05911bdb-02ae-44e8-b310-db4a1cef538d" />

## Key Insights

From the analysis, several actionable insights emerge:

•	Behavioral Gap: Casual riders and members use the service for fundamentally different purposes (leisure vs. utility). 

•	Conversion Opportunity: Casual riders already see value but lack a strong incentive to commit. 

•	Timing Matters: Marketing efforts should align with weekend and leisure usage patterns. 

•	High-Intent Segment: Frequent casual riders are the most likely candidates for conversion. 

•	Experience vs. Cost Trade-off: Casual users may perceive memberships as unnecessary for occasional us.

