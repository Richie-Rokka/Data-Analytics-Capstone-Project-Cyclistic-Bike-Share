# Phase 3 – Process

The 12 CSV files from divvy- trip data (January 2021 to December 2021) were stacked and combined into a single DataFrame. The table consists of 5,595,075 rows.

Before analysis, the dataset was cleaned and transformed to ensure accuracy, consistency, and usability. Given that the data was collected across multiple files, and part of the steps involved consolidating all datasets into a single, structured dataset for efficient analysis.

## Data Cleaning Steps-

•	Data Consolidation - Merged the 12 monthly datasets into one unified table to enable a full year trend analysis while I removed the columns for latitude and longitude.

•	Handling Missing Values - Identified and replaced records with null or incomplete fields (missing station names) with “unknown station name” to maintain data quality. 

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

## Tools used

•	Excel 

•	Python (Pandas, Jupyter) 

•	Tableau 

The final dataset consists of 5,504,784 rows after cleaning, which means that 90, 291 rows were removed.
