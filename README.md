Bellabeat Case Study
Capstone Project for Google Data Analytics Professional Certificate

1. Project Overview
Title: Bellabeat: How Can A Wellness Technology Company Play It Smart?
Author: Mario Ariel Galarza Mancedo
Date: January 19, 2024

1.1 Background
Bellabeat is a high-tech wellness company specializing in smart products for women. This case study analyzes FitBit Fitness Tracker Data (publicly available on Kaggle) to uncover trends in consumer behavior and provide insights for Bellabeat’s marketing strategy.

1.2 Business Task
Analyze FitBit usage data to:

Identify trends in user activity.

Determine how these trends apply to Bellabeat customers.

Provide data-driven recommendations for Bellabeat’s marketing strategy.

1.3 Key Questions
What are the trends in FitBit usage?

How do these trends relate to Bellabeat’s customers?

How can Bellabeat leverage these insights for marketing?

2. Data Preparation
2.1 Data Source
Dataset: FitBit Fitness Tracker Data (Kaggle)

Collection Period: March 12, 2016 – May 12, 2016

Sample Size: 30 FitBit users (33 unique IDs in data)

Data Includes:

Daily activity (steps, distance)

Heart rate

Sleep monitoring

Calories burned

2.2 Data Limitations
Small sample size (30 users) → Not representative of the female population.

Outdated (2016 data) → User habits may have changed.

Third-party collection (Amazon Mechanical Turk) → Potential integrity issues.

2.3 Data Quality (ROCCC Assessment)
Criteria	Rating	Reason
Reliable	❌ Low	Only 30 respondents
Original	❌ Low	Collected via third party
Comprehensive	⚠️ Medium	Matches Bellabeat’s parameters
Current	❌ Low	5+ years old
Cited	❌ Low	Unknown original source
Conclusion: Data is low quality; insights should be taken cautiously.

3. Data Processing (Python)
3.1 Tools Used
Python Libraries:

pandas (data manipulation)

numpy (numerical analysis)

matplotlib (visualizations)

3.2 Key Data Cleaning Steps
Handled Missing Values: No null values detected.

Converted Data Types:

Changed ActivityDate from object to datetime64.

Added New Columns:

day_of_the_week (extracted from date)

total_mins (sum of all activity minutes)

total_hours (converted minutes to hours)

3.3 Data Transformation
Renamed columns for clarity (e.g., TotalSteps → total_steps).

Calculated median and mean values for analysis.

4. Analysis & Key Findings
4.1 Statistical Summary
Metric	Average	CDC Recommendation*
Daily Steps	7,637	≥10,000
Distance (km)	5.4	≥8.0
Sedentary Time	20 hrs	< 8 hrs
Calories Burned	2,303	Varies by individual
Source: CDC & Medical News Today

4.2 Visualizations & Insights
A. Activity Frequency by Day
📊 Observation:

Highest usage: Midweek (Tue-Fri)

Lowest usage: Weekends & Monday
💡 Insight: Users track activity more on weekdays (possibly due to work routines).

B. Steps vs. Calories Burned
📈 Observation:

Positive correlation (more steps = more calories burned).

Outliers: Some users logged 0 steps or >35,000 steps with low calories.
💡 Insight: Encouraging consistent moderate activity is key.

C. Sedentary vs. Active Time
🛋️ Observation:

81.3% of logged time was sedentary (sitting/inactive).

Only 1.7% was "very active" (exercise).
💡 Insight: Most users do not use FitBit for fitness tracking—Bellabeat can fill this gap.

5. Recommendations for Bellabeat
5.1 Marketing Strategies
✅ Educate Users:

Push notifications on health benefits of 10,000 steps.

Share simple weekday workouts (10-min exercises).

✅ Weekend Engagement:

Send weekend fitness challenges (e.g., "Saturday Stretch Goal").

✅ Gamification:

Reward users for consistent activity (badges, discounts).

5.2 Product Improvements
📱 App Features:

Sleep & stress tracking (women-focused wellness).

Personalized calorie goals based on activity.

6. Conclusion
FitBit data shows low physical activity and high sedentary behavior.

Bellabeat can differentiate itself by promoting fitness engagement and women-centric health tracking.

Next Steps: Validate findings with larger, recent datasets and conduct user surveys.

🔗 Files Included:

dailyActivity_merged.csv (processed dataset)

Python script (bellabeat_analysis.ipynb)

Visualizations (PNG/JPEG)
