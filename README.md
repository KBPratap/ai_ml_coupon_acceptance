# Analyze Coupon Acceptance

## Overview
This project is part of the AI&ML course. It attempts to study the acceptance rate for coupon amongst different drivers and how the different criteria could affect their decisions.
This data from the UCI Machine Learning repository collected via a survey on Amazon Mechanical Turk is used in this project. 

## Analysis
### Data Cleanup
Data cleanup is the first step before one starts analysis. Steps taken during cleanup 
* drop an entire column where more than 99% of the data was null values
* drop all null value records when scope is entire dataset
* selectively drop null value records only for a subset of data when analysing a subset of coupons  


### Coupon Categories
#### "Bar"
**Goal**
Analyze the data and understand the factors that could affect the acceptance-rate for Bar coupons

**Findings**
The drivers are more likely to accept the bar coupons, if
- they visit a bar more frequently
- do not have kids as passengers
- older than 30

#### "Carry out & Take away"
**Goal**
analyze the popularity of these coupons based on income groups and driving directions.

**Findings**
the 'Carry out & Take away' coupons are popular across different income groups and uniformly distributed independent of the frequncy of the CarryAway. The coupon acceptance-rate ranges between 67% - 82% across different income groups.

When checking for driving directions, the data shows some counter-intuitive patterns:
- the acceptance-rate is higher at 76% when driving direction is opposite
- the acceptance-rate seems to be lower as 71% when driving direction is same.

A detailed analysis can be found in the [jupyter notebook](https://github.com/KBPratap/ai_ml_coupon_acceptance/blob/main/prompt.ipynb)