# 🚲 Cyclistic Bike-Share Analysis

## 🚀 Executive Summary
This project analyzes Cyclistic’s bike-share data to understand how **casual riders and annual members use the service differently**. The findings show that casual riders are primarily **leisure-driven**, while members are **commute-focused**, creating a clear opportunity to increase revenue by converting high-frequency casual users into annual members through targeted, data-driven marketing strategies.

---

## 📌 Business Problem
Cyclistic aims to grow its business by increasing the number of **annual memberships**, which provide more stable and predictable revenue.  

The key question:
**How can Cyclistic convert casual riders into annual members?**

---

## 🎯 Objectives
- Analyze **user behavior and ride patterns**
- Identify differences between **casual riders and members**
- Generate **actionable insights**
- Recommend **data-driven marketing strategies**

##    Stakeholders
- Director of Marketing - Leads Cyclistic’s marketing strategy, focusing on customer acquisition, membership conversion, and maximizing marketing ROI.
- Marketing Analytics Team - Collects and analyzes ride data to generate actionable insights that support targeted marketing and customer segmentation.
- Executive Team - Approves data-driven strategic initiatives that drive long-term growth, customer retention, and revenue sustainability.

---

## 🧠 Approach
This project follows the **Google Data Analytics framework**:

**Ask → Prepare → Process → Analyze → Share → Act**

## 📊 Dataset
- 12 months of **trip-level ride data**
- Dataset link - <a href="https://divvy-tripdata.s3.amazonaws.com/index.html">Cyclistic Dataset</a>
- divvy-tripdata from Motivate International Inc under this <a href="https://www.divvybikes.com/data-license-agreement">License-Agreement</a> 
- Key features:
  - Ride unique id
  - Ride timestamps  
  - Start & end stations  
  - Bike types  
  - User type (casual vs member)  
- No **personally identifiable information (PII)** included  
- Enables **aggregate behavioral analysis**

## 🧹 Data Cleaning & Preparation
- Merged 12 monthly datasets into one  
- Removed missing and duplicate records  
- Standardized date/time formats
- Invalid records (negative/zero/Outliers)  
- Created new features:
  - Ride duration  
  - Day of week  
  - Month  
  - Start ride hour


---

## 📊 Key Insights (Quick View)

- Casual riders → **longer rides** (29.96 mins vs 13.57 mins)  
- Members → **commute-focused** (peak at 8 AM & 5 PM)  
- Casual riders → **weekend & leisure usage**  
- Members → **weekday, routine usage**  
- Strong **seasonal trends** (summer peaks, winter lows)


---


