# AtliQ-Grand-Hospitality-Analysis--PowerBI

Why is AtliQ Grands losing its market share and revenue? Let’s find out...

### INTRODUCTION
This document presents the analysis of hotel data for AtliQ Grands, from May 2022 — June 2022. This will enable us to gain insights into various aspects of hotel management, including, customer ratings, occupancy rates, revenue, and bookings. This analysis was performed using Power BI, a powerful data visualization and analytics tool.

### PROBLEM STATEMENT
AtliQ Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, AtliQ Grands are losing its market share revenue in the luxury/business hotels category.

### Objective: 
To provide AtliQ Grands with insights from their historical data to regain their market share and revenue.

### DATA SOURCING
The dataset used for this analysis was collected from Code Basics’ website.

### SKILLS DEMONSTRATED
This project exposed me to learning a lot using Microsoft Power BI.
· Multiple complex DAX formulas and Functions.
· Calculated columns
· Data Extraction, Cleaning, and Transformation (ETL)
· Data Modelling
· Data Visualization

### DATA MODELING : STAR SCHEMA
The data model in Power BI consists of five tables:

#### dim_date: 
Contains full date information about dates including day type (weekend or weekday), month, and week number (W19 — W32). 
#### dim_hotels: 
Stores identity number of the hotel, property name, category it belongs to (luxury/business), and the city it’s located. dim_rooms: Includes room id and room class. 
#### fact_bookings: 
Stores information about bookings including booking dates, booking platforms, number of guests, revenue, check-in, and checkout dates. 
#### fact_aggregrated_bookings: 
Includes successful bookings, hotel id, and capacity. The dimension tables (with the prefix “dim”) have a matching id in the fact tables (with the prefix “fact”). 
This modeling produces a one-to-many relationship.

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/e7d6c088-d55c-4a9e-bf75-a0225d6dd844)


## ANALYSIS/VISUALIZATION

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/b26f7e63-98e1-403f-a13d-f4952eeed49d)


From the dashboard, the key metrics are at the top.

Note: RevPar -Revenue Per Available Room, DSRN - Daily Sellable Room Nights/per night, ADR - Average Daily Rate/Amount per room, DBRN -Daily Booked Room Nights/per night, and DURN - Daily Booked Room Nights/per night, Realization% - The ratio of utilized rooms and booked rooms per night, Occupancy% - Total number of occupied rooms out of the available.


### How much did we generate in the last three months? Show other key metrics that are helpful to the business.

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/31dd74b5-6315-45b6-8d8c-e5d0e8a7eb08)

Within the period of three months, the business was able to generate a revenue of 1.71 billion. The occupancy rate across all locations is slightly above 50%,(57.9%). This means that on average, at least 50% of the rooms are utilized daily. The average selling price for a room is 12.69K while RevPar equals 7,347. Below the key metrics is the week-on-week change which shows the percentage increase or decrease compared to the latest previous week.

### Is there any significant difference in occupancy for weekends and weekdays? Does this have any impact on the pricing?

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/5eedf863-c187-445f-90f2-733a16c0378c)

The chart above shows that there are more guests/customers during weekends (62.64% occupancy) than on weekdays (55.99%). 
Meanwhile, there’s no significant difference in ADR and Realization on weekdays or weekends.

### In terms of revenue generation, how has our revenue performed across the two room categories during this period?

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/ba232edd-cf75-4c2b-aa30-dbf278ea81fb)

The above chart shows that rooms in the Luxury category are contributing the majority of the revenue (61.61%). 
Rooms in the Business category contribute less than forty percent of the total revenue (38.39%).

### Could you pull weekly trends for occupancy? We’ll like to see that concerning Revenue.

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/13cf07ab-6cdd-4faf-996e-1ab0fcb98285)

This chart shows that RevPar and Occupancy are fluctuating while ADR is constant. 
RevPar is a by-product of Occupancy, hence the reason for the fluctuation. A constant ADR shows the pricing is relatively fixed.

### What are our best and least performing properties in terms of revenue?

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/59f43856-ca3d-4baa-b25f-66066a581ab4)

Although there is little difference in the revenue for best-performing and least-performing properties (hotels), 
Atliq seasons (65M) is performing very poorly in revenue generation.

### We have several booking platforms, can we see how they are all performing?

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/1244ff4b-b88b-4cbd-92bd-dce5372cc433)

The above chart shows how ADR differs across all platforms with realization. ﻿Across all 7 booking_platform, Realization% ranged from 69.8% to 70.6% and ADR ranged from 12634 to 12791.
Not major change in Realization and ADR among all platforms but there is Other travel platforms/channels are the primary booking source.

### What about our properties in different cities, is their performance below par?

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/9aefd3cf-8ca2-4062-8e86-be69df2924a9)

The hotels in Mumbai contribute most of the revenue, followed by  Bangalore, Hyderabad and Delhi respectively.

### KEY FINDINGS/INSIGHTS

After analyzing the data, I was able to derive these insights:

* Over the period of three months (May, June, and July), AtliQ Grands were able to generate a revenue of approximately 1.7 billion. During this period, RevPar, realization and occupancy increased from the latest previous week, except for revenue which decreased by 0.82%.

* Mumbai generates the highest revenue (669 M) followed by Bangalore, Hyderabad and Delhi

* AtliQ Exotica performs better compared to all 7 type of properties with 320 Million revenue, rating 3.62, occupancy percentage 57 and cancellation rate as 24.4%.

* The overall average rating is 3.62. There is a correlation between revenue and average ratings, in that ratings with high ratings tend to generate more revenue.

* Weekends consistently exhibit higher occupancy rates than weekdays. There is no significant difference in ADR for weekdays and weekends. This shows that the hotel is using a flat pricing strategy.

* Other travel platforms/channels are the primary booking source, generating 40% of total bookings and revenue. Direct online booking contributes the least to bookings and revenue generation, with 5%.
The Average Daily(ADR) Rate is higher on direct offline (hotel premises) compared to other booking platforms.

* The Luxury room category contributes the majority of revenue and bookings. 


### RECOMMENDATIONS

* The rule of demand and supply and price elasticity is different for the travel, tourism, and hospitality industry. 
  Therefore, the hotel should leverage dynamic pricing to increase revenue generation and increase prices for peak days and weekends.

* Consider differential pricing strategies for their offline booking platforms by implementing targeted marketing campaigns/promotions to boost bookings and in turn increase revenue.

* AtliQ Grands should pay more attention to customer reviews and ratings and focus on improving customer satisfaction further by addressing critical areas identified in customer reviews.

* Explore opportunities to increase direct bookings through the hotel’s website to reduce dependence on other online platforms.

### CONCLUSION

The data analysis performed using Power BI has provided valuable insights into various aspects of hotel management for AtliQ Grands Hotel. 
The findings and recommendations can help optimize operations, enhance customer satisfaction, and drive revenue growth. 
Regular monitoring and analysis of key metrics will ensure continued success in the hotel. 









