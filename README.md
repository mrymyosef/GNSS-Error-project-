🛰️ GNSS Error Project
Time Series & Statistical Analysis of GNSS Positioning Errors (2022–2024)

# 📌 Challenge #1: Preparing the Data for Analysis

Objective: Ensure the dataset was reliable before analysis.

Tasks Performed

✔ Checked for missing values

✔ Validated data types

✔ Converted the Date column to datetime

✔ Created new features:

Month
Season

Outcome

Dataset was already clean.
Feature engineering enabled meaningful temporal and seasonal analysis.

# 📌 Challenge #2: Identifying Extreme Positioning Errors

Question

Are there any abnormal positioning errors?

Method

Used boxplots to detect outliers.

Findings

Vertical positioning error (dUp) contained the highest number of outliers.
WAGN exhibited significantly larger vertical deviations than ADCN.
Positioning performance differed noticeably between the two stations.

# 📌 Challenge #3: Understanding Error Behavior Over Time

Approach
Instead of analyzing individual observations, the data was aggregated into:

Daily trends
Weekly summaries
Monthly summaries
Seasonal comparisons

Findings

Identified recurring periods of increased GNSS errors.
Revealed long-term trends instead of isolated events.

# 📌 Challenge #4: Measuring Positioning Accuracy

Statistical Metrics Calculated

Mean
Standard Deviation
Root Mean Square (RMS)
Mean Absolute Error (MAE)
Root Mean Square Error (RMSE)

Outcome

Evaluated positioning accuracy.
Measured variability for both monitoring stations.

📌 Challenge #5: Going Beyond Individual Error Components

Instead of analyzing North, East, and Vertical errors separately, I calculated:

2D Position Error
3D Position Error

Outcome

Better representation of overall positioning accuracy.
Easier comparison between ADCN and WAGN.

# 📌 Challenge #6: Investigating Relationships Between Error Components

Objective
Determine whether one positioning error influences another.

Method

Pearson Correlation Analysis

Findings

Very weak correlations between horizontal and vertical error components.
Each component behaves largely independently.
Correction models should analyze each component separately.

# 📊 Key Takeaways

📌 WAGN exhibited significantly larger vertical positioning errors than ADCN.

📌 Vertical errors contributed the most to total 3D positioning error.

📌 GNSS positioning accuracy varied across seasons.

📌 Daily, weekly, and monthly analyses revealed recurring periods of increased positioning errors.

📌 Horizontal and vertical positioning errors showed very weak correlations, indicating largely independent behavior.







