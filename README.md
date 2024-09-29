![MasterHead](https://github.com/user-attachments/assets/df01824d-2b3a-4d40-b330-dc34ff53b698)


# Uber Data Science - Exploration and Insight

This work contains the code and results of a data science take home assignment performed on an Uber dataset. The aim is to extract insights from the data by answering specific problem statements related to user activity, driver supply and demand analysis.

# Overview

This work involves exploratory data analysis (EDA) of a dataset provided by Uber which captures the interaction between users and drivers over a given period. The data was used to address multiple problem statements related to:

- User behavior (requests, completed trips)
  
- Driver availability and supply-demand analysis
  
- Calculation of useful metrics (e.g., busiest times, most requests)
  
The data exploration was carried out using Python libraries such as Pandas, Matplotlib, and Seaborn. The project provides valuable insights into the supply-demand patterns during the observed time frame and suggests potential improvements.

# Setup

Visual Studio Code

# Dataset Description

The dataset contains 336 rows and 7 columns. Each row represents one hour of data for a particular day. Here’s a breakdown of the columns:

| Column            | Description                                                            |
|-------------------|------------------------------------------------------------------------|
| `Date`            | The date when the data was recorded.                                   |
| `Time (Local)`    | The hour of the day in local time (0-23).                              |
| `Eyeballs`        | Number of users who opened the Uber app during this hour.              |
| `Zeroes`          | Number of users who opened the app but did not see any available cars. |
| `Completed Trips` | Number of successfully completed trips during this hour.               |
| `Requests`        | Number of trip requests made during this hour.                         |
| `Unique Drivers`  | Number of drivers available during this hour.                          |

The dataset reflects user activity, requests made, trips completed and drivers logged in during different hours of the day over a span of days in September 2012.

[Access the dataset](https://github.com/BIKASH1002/Uber-Data-Science/blob/c8af5820b24d80ff28876e5f1ba79b47ddde008c/uber_dataset.csv)

# Problem Statements

**1)** Which date had the most completed trips during the two week period?
   
**2)** What was the highest number of completed trips within a 24 hour period?

**3)** Which hour of the day had the most requests during the two week period?

**4)** What percentages of all zeroes during the two week period occurred on weekend (Friday at 5 pm to Sunday at 3 am)? 

**5)** What is the weighted average ratio of completed trips per driver during the two week period? 

**6)** In drafting a driver schedule in terms of 8 hours shifts, when are the busiest 8 consecutive hours over the two week period in terms of unique requests? A new shift starts in every 8 hours. Assume that a driver will work same shift each day.

**7)** True or False: Driver supply always increases when demand increases during the two week period.

**8)** In which 72 hour period is the ratio of Zeroes to Eyeballs the highest?

**9)** If you could add 5 drivers to any single hour of every day during the two week period, which hour should you add them to? 

**10)** True or False: There is exactly two weeks of data in this analysis.

**11)** Looking at the data from all two weeks, which time might make the most sense to consider a true "end day" instead of midnight? (i.e when are supply and demand at both their natural minimums).

# Visualizations

The following visualizations were generated to support the analysis:

**1) Supply vs. Demand Graph:** This plot shows the correlation between the number of users opening the app (Eyeballs) and the number of drivers logged in (Unique Drivers).

![1](https://github.com/user-attachments/assets/5653a861-5d4c-4d9d-bce4-a2404ea8ea7a)

**2) Trips Over Time:** This graph displays the number of completed trips over the two-week period.

![2](https://github.com/user-attachments/assets/35389e55-c0fc-42a2-9fca-ccc770eb4aed)

# Conclusion

This work provides a clear picture of how user demand fluctuated during the day and how well the supply of drivers met the demand. It identifies key issues such as periods of unmet demand and suggests times when driver availability should be increased.

# Credits

Everyday Data Science from Youtube
