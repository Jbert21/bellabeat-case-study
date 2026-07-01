# Bellabeat Case Study – Google Data Analytics Capstone

## Overview

This case study is part of the Google Data Analytics Professional Certificate capstone project.

The objective is to analyze smart device usage data from Fitbit users in order to identify behavioural trends in how consumers use wearable fitness devices. These insights are then applied to a Bellabeat product to provide recommendations that support marketing strategy and future business growth.

Bellabeat is a wellness technology company that creates health-focused smart products designed primarily for women. Understanding user behaviour in similar fitness tracking devices helps inform product development and marketing decisions.

---

## Business Task Summary

Analyze smart device usage data from non-Bellabeat users to identify trends in how consumers use wearable fitness devices. Apply these insights to one Bellabeat product and provide recommendations that can help inform Bellabeat's marketing strategy and support future business growth.

---

## Stakeholders

- **Urška Sršen** – Bellabeat co-founder and Chief Creative Officer  
- **Sando Mur** – Bellabeat co-founder and key member of the executive team  
- **Bellabeat Marketing Analytics Team** – Responsible for collecting, analyzing, and reporting data to guide marketing strategy  

---

## Key Questions

- What trends can be identified in smart device usage among consumers?
- How can these trends be applied to Bellabeat customers and products?
- How can these insights be used to influence Bellabeat's marketing strategy and drive future growth?

---

## Data Source

The dataset used is the **FitBit Fitness Tracker Data (CC0: Public Domain)**, made available through Mobius on Kaggle.

It contains personal fitness tracker data from 30 Fitbit users who consented to the submission of their data. The dataset includes minute-level and daily-level information on physical activity, heart rate, and sleep monitoring.

### Dataset Overview

- **Source:** Kaggle (Fitbit Fitness Tracker Data)
- **Users:** 30 Fitbit users
- **Timeframe:** 31 days
- **Granularity:** Daily-level activity data
- **Records:** 940 daily activity entries

The dataset was imported into **Google BigQuery** for cleaning and analysis.

---

## Data Schema (Daily Activity Table)

- **Id** – Unique identifier for each user  
- **ActivityDate** – Date of recorded activity  
- **TotalSteps** – Total steps taken per day  
- **TotalDistance** – Total distance travelled per day  
- **TrackerDistance** – Distance tracked by Fitbit device  
- **LoggedActivitiesDistance** – Manually logged activity distance  
- **VeryActiveDistance** – Distance from very active activity  
- **ModeratelyActiveDistance** – Distance from moderate activity  
- **LightActiveDistance** – Distance from light activity  
- **SedentaryActiveDistance** – Distance recorded during sedentary activity  
- **VeryActiveMinutes** – Minutes spent very active  
- **FairlyActiveMinutes** – Minutes spent moderately active  
- **LightlyActiveMinutes** – Minutes spent lightly active  
- **SedentaryMinutes** – Minutes spent sedentary  
- **Calories** – Estimated daily calories burned  

This dataset enables analysis of physical intensity, movement behaviour, and daily energy expenditure.

---

## Data Cleaning & Preparation

The dataset was imported into Google BigQuery and validated before analysis.

### Duplicate Check
No duplicate records were found.

### Missing Values
No NULL values were detected.

### Time Range Validation
The dataset was confirmed to span a 31-day period as expected.

### User Participation Consistency
User activity tracking varied significantly:
- Most users logged close to 30–31 days
- Some users logged as few as 4 days
- Overall engagement declined toward the end of the study period

### Data Filtering
No data was removed or filtered during analysis.

---

## Analysis

The analysis focused on three key aspects of smart device usage relevant to Bellabeat’s business objectives:
1. Activity intensity distribution  
2. Differences in user activity levels  
3. User engagement over time  

---

### 1. Activity Intensity Distribution

The analysis measured the average proportion of time users spent in different activity states:
- Sedentary
- Lightly active
- Very active

**Findings:**
- Users spend approximately **81% of their time sedentary**
- Around **17% of time is lightly active**
- Less than **2% of time is very active**

This indicates that most users have highly sedentary daily behaviour, with very limited time spent in high-intensity activity.

---

### 2. User Activity Segmentation

Users were segmented based on daily step count:
- Low activity (<5,000 steps/day)
- Moderate activity (5,000–10,000 steps/day)
- High activity (≥10,000 steps/day)

**Findings:**
- 54.55% of users are **moderately active**
- 24.24% are **low activity**
- 21.21% are **high activity**

This shows that most users fall into the moderate-to-low activity range, with relatively few consistently highly active users.

---

### 3. User Engagement Trends

User engagement was measured by tracking daily participation over the study period.

**Findings:**
- Daily active users decreased from **33 at the start** to **21 at the end**
- This represents a **36.36% decline in engagement over 31 days**

This suggests that user engagement decreases over time, indicating potential retention challenges.

---

## Recommendations

### 1. Personal Coaching & Behavioural Support

Since users are largely sedentary, Bellabeat should introduce features that encourage consistent movement through behavioural nudges.

A potential solution is a **personal coach or avatar system** that:
- Sends reminders and motivational messages
- Provides personalised recommendations
- Encourages consistent daily activity

This would improve accountability and increase user engagement.

---

### 2. Focus on Step Count as a Core Metric

Step count is a simple and accessible metric that works well for beginners.

Since ~79% of users are low-to-moderately active:
- Step tracking should be positioned as the **primary entry point**
- Users should be guided with personalised daily step goals
- Progress tracking should be highly visible and motivating

This reduces friction for new users starting their fitness journey.

---

### 3. Improve Long-Term Engagement & Retention

Engagement declines over time, suggesting a need for stronger retention strategies.

Potential improvements:
- Monthly or yearly personalised summaries (similar to Spotify Wrapped)
- Shareable progress reports for social media
- Multi-metric insights (sleep, hydration, cycle tracking, etc.)

This increases long-term engagement and strengthens brand visibility.

---

## Conclusion

This analysis identified three key trends in Fitbit smart device usage:

- Users spend most of their time sedentary  
- Activity levels vary significantly across users  
- Engagement declines over time  

These insights suggest that Bellabeat should focus on:
- Simple, accessible metrics like step count  
- Behavioural coaching and personalised guidance  
- Long-term engagement features that encourage retention and sharing  

By implementing these strategies, Bellabeat can better support users at the beginning of their fitness journey, improve retention, and increase brand growth through engagement and organic sharing.

---

## Author

Jason Bertschinger  
Google Data Analytics Capstone Project
