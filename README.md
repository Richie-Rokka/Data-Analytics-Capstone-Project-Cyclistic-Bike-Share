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


---

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

- Total Rides & Average Ride Length Patterns in  year 2021

<img width="1500" height="1200" alt="Total Ride Stats" src="https://github.com/user-attachments/assets/c0453833-8c1b-4684-894e-13871f36fb52" />


---


## 🔍 Detailed Insights

### ⏱️ Ride Duration
Casual riders take significantly longer rides, indicating **leisure and exploration**, while members prioritize **short, efficient trips**.

---

### ⏰ Time of Use
- Members peak at **8 AM and 5 PM** → commuting behavior  
- Casual riders show a **steady increase throughout the day**, peaking in the afternoon  


---
- Hourly Ride Trends

<img width="708" height="319" alt="Hourly Stats" src="https://github.com/user-attachments/assets/bb5a014e-d78a-4522-a6c6-9d1e213b90b5" />

---


### 📅 Weekly Patterns
- Members: consistent weekday usage (highest on Wednesdays)  
- Casual riders: peak on weekends (highest on Saturdays)  

<img width="1500" height="1200" alt="Daily Stats" src="https://github.com/user-attachments/assets/2df0f24a-97d3-48cb-9492-78d2f32a63b0" />

---

### 🌦️ Seasonal Trends
- Lowest usage in winter (February)  
- Peak usage in summer:
  - Casual riders peak in July  
  - Members peak in September  

<img width="1500" height="1200" alt="Monthly Stats" src="https://github.com/user-attachments/assets/64c892c1-552f-4173-b919-50b7cb32a3ff" />


---

### 🚴 Bike Preference
Both groups prefer **classic bikes**, while docked bikes are mainly used by casual riders.

---

## 💡 Recommendations

- Target **high-frequency casual riders**  
- Introduce **trial membership offers**  
- Focus marketing on **weekends and high-traffic locations**  
- Highlight **cost savings of membership**  
- Use **personalized usage insights** to drive conversion  

---

## 📈 Business Impact

- Increased **membership conversion rates**  
- Improved **customer lifetime value (CLV)**  
- More **predictable recurring revenue**  
- Better **marketing ROI through targeted campaigns**  

---

## 🔑 Why This Matters
Understanding the difference between **leisure and commuter behavior** allows Cyclistic to shift from broad marketing to **precision targeting**, improving both efficiency and profitability.

---

## 🛠️ Tools & Technologies

- **SQL** – Data cleaning and transformation  
- **Excel** – Data analysis  
- **Tableau** – Data visualization  

---

