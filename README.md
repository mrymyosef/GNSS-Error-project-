# GNSS-Error-project-
Time Series and Statistical Analysis

# Challenge #1: Preparing the Data for Analysis Before performing any analysis.

I needed to ensure the dataset was reliable. I started by: Checking for missing values Validating data types Converting the date column into a proper datetime format Creating new features such as Month and Season Although the dataset was already clean, creating these additional features made it possible to perform meaningful temporal and seasonal analyses.

# Challenge #2: Identifying Extreme Positioning Errors One of the first questions I asked was: 

"Are there any abnormal positioning errors?" Using boxplots, I discovered that the vertical positioning error (dUp) contained the largest number of outliers. More importantly, the WAGN station showed much larger vertical deviations than ADCN, indicating that positioning performance varied significantly between the two stations. 

# Challenge #3: Understanding Error Behavior Over Time Instead of analyzing thousands of observations individually.

I aggregated the data into: Daily trends Weekly summaries Monthly summaries Seasonal comparisons This approach revealed periods where GNSS errors consistently increased, making it easier to identify long-term patterns rather than isolated events. 

# Challenge #4: Measuring Positioning Accuracy To evaluate the performance of each station.

I calculated several statistical metrics, including: Mean Standard Deviation Root Mean Square (RMS) Mean Absolute Error (MAE) Root Mean Square Error (RMSE) These metrics provided a comprehensive picture of positioning accuracy and variability across both monitoring stations.

# Challenge #5: Going Beyond Individual Error Components Rather than analyzing North, East, and Vertical errors separately.

I calculated: 2D Position Error 3D Position Error These engineering metrics provide a much better representation of overall positioning accuracy and made it possible to compare station performance more effectively. 

# Challenge #6: Investigating Relationships Between Error Components I wanted to determine whether an increase in one positioning error would influence the others.

Using Pearson Correlation Analysis, I found that the relationships between horizontal and vertical error components were generally very weak. This suggests that each component behaves largely independently and should be analyzed separately when developing correction models. 


# Key Insights 

📌 WAGN exhibited significantly larger vertical positioning errors than ADCN. 
📌 Vertical errors contributed the most to total 3D positioning error. 
📌 GNSS positioning accuracy varied across seasons. 
📌 Daily, weekly, and monthly analyses revealed recurring periods of increased positioning errors. 
📌 Horizontal and vertical positioning errors showed very weak correlations, suggesting independent behavior. create presentation in canva
