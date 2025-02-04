# Maximize Revenue for Taxi Drivers through Payment Type Analysis
Statistics Hypothesis Testing Project - Mode of Payment Analysis


### Introduction
In the taxi industry, the method of payment (cash, card, mobile wallets) can impact the revenue generation of drivers. However, many taxi drivers fail to optimize their payment options because they do not fully understand customer preferences regarding payment types. This analysis explores whether certain payment methods (cash vs. card) correlate with higher revenue and whether identifying such patterns can help drivers improve their earnings.

### Objective
The main objective of this project is to analyze customer preferences for cash vs. card payments and identify which payment method generates higher revenue for taxi drivers. This analysis aims to uncover patterns that will guide drivers in selecting the optimal payment methods, potentially boosting their earnings.

### Data Cleaning
The dataset is first examined for issues like missing values, incorrect data types, duplicates, and irrelevant or zero values in the columns:

Data Types: Columns like tpep_pickup_datetime and tpep_dropoff_datetime were converted to the datetime format.
Duration Calculation: A new column duration was created to represent the trip duration in minutes by calculating the difference between tpep_dropoff_datetime and tpep_pickup_datetime.
Duplicates: Duplicate records were identified and removed to ensure accuracy in the analysis.
Irrelevant Data: Non-relevant data like entries with zero passengers, fare amounts, or trip distances were filtered out.
Outliers: Outliers in trip duration, distance, and fare amounts were identified using boxplots and removed using the Interquartile Range (IQR) method to avoid skewed results.

### Data Analysis
#### Exploratory Data Analysis (EDA):

Visualizations like histograms and box plots were used to understand the distribution of fare amounts and trip distances for both payment types (cash vs. card).
A pie chart was created to show the proportion of cash vs. card payments, highlighting customer preferences.
Stacked bar charts were used to show how payment preferences vary with passenger count.

#### Insights:

A noticeable variation in payment types based on passenger count and trip characteristics (distance, fare) was identified.
A significant proportion of passengers prefer using card payments, but cash payments are still prominent among certain trip distances and fare amounts.
Hypothesis Testing

#### Objective: 
To test whether there is a significant difference in the average fare amounts between customers paying by card and those paying by cash.

#### Null Hypothesis: 
There is no difference in the average fare amounts for card and cash payments.

#### Alternative Hypothesis: 
There is a significant difference in the average fare amounts for card and cash payments.

#### Test Used: 
Since the data does not follow a normal distribution, a T-test was applied to compare the means of two independent samples (cash vs. card payments).

### Results: 
The p-value from the T-test was significantly lower than 0.05, leading to the rejection of the null hypothesis. This suggests that there is a significant difference in fare amounts between cash and card payments.

### Conclusion
The analysis shows that there is a significant difference in fare amounts between customers paying by cash and those paying by card.
Drivers should consider leveraging data-driven insights into customer preferences for payment types to maximize their revenue.
Future work can include additional segmentation of the data based on location, time of day, or seasonality to provide more specific recommendations for taxi drivers.







