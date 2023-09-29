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











