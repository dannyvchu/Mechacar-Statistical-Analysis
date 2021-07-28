# MechaCar Statistical Analysis

## Project Purpose
The company AutosRUs wants to improve their decision making process on improving their MechaCar by implementing data driven analysis and statistics. Using old data provided by the company, we will perform retrospective analysis, analytical verification and validation of current automotive specifications, and study design of future product testing.

## Resources
- Software: 
	- R
	- RStudio
	- tidyverse
	- ggplot2
	
## Results

### Linear Regression to Predict MPG

![lin_reg](images/lin_reg.png)

- Both the Vehicle Length (p-value = 2.60x10^-12) and Ground Clearance (p-value = 5.21x10^-08) variables have the most significant impact on the MPG of MechaCar. The intercept (-104.0) is also significant, implying other important variables that impact MPG not included in the given dataset.
- The slope of the linear model is not considered to be zero because the coefficients of the significant variables are non-negligible. Assuming a confidence level of α=0.05, we can see that the calculated p-value of 5.35x10^-11 is much lower than α, therefore their is an extremely high probability that the relationships between our variables and the MPG is not just random chance.
- This linear model predicts the miles per gallon of mechacar fairly effectively. Our r-squared value of 0.7149 implies a 71.5% accurate representation of the data.

### Summary Statistics on Suspension Coils

![tot_sum](images/tot_sum.png)
![lot_sum](images/lot_sum.png)

The design specifications of the MechaCar dictate that the variance of the suspension coils can not exceed 100 lbs/in^2 . The variance for the combined lots is below the specified threshold sitting at 62.29, therefore meeting the design specifications. However, the variance for Lot 3 is 170.29, which far exceeds the appropriate design.



### T-Tests on Suspension Coils

Looking at the heat map on the top right, we can see that the majority of rentals are done by subscribers, compared to one time users. New startups should definitely consider a subscription plan for local renters who may use bikes as a way to commute to and from work.


## Summary

There are many trends and insights that can be deduced looking at the visualizations above that would be extremely useful for any bike rental company.

### Trends
- Most bikes are rented for under 30 minutes.
- Males are the majority of users for bike rentals.
- Bikes are rented most commonly at the start and end of work hours.
- Subscribers rent more often than one-time-users.

### Insights
- The target demographic for any ad campaigns should target males at first, and then switch to females when the male market is saturated.
- Bike maintenance should be performed during the slowest times of the day in the very early AMs.
- Creating a subscription service will help incentivize local commuters to joining.

### Further Analysis
For more information, I would like to create a heatmap over a map of the area, to help understand which types of neighborhoods have the most rentals. This would give us an insight on how to distribute the total supply of bikes to each given neighborhood. Another visualization I would like to make in the future is a map of each bike and the location of the end points vs start points to gain an insight of how to redistribute bikes from areas of low rental traffic to high rental traffic.

## Link to my Tableau Public page: [CitiBike Data Analysis Dashboard](https://public.tableau.com/views/CitiBikeDataAnalysis_16268649968870/CitiBikeDataAnalysis?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)