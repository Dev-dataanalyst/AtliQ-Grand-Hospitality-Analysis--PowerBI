# AtliQ-Grand-Hospitality-Analysis--PowerBI

Why is AtliQ Grands losing its market share and revenue? Let’s find out...

# INTRODUCTION
This document presents the analysis of hotel data for AtliQ Grands, from May 2022 — June 2022. This will enable us to gain insights into various aspects of hotel management, including, customer ratings, occupancy rates, revenue, and bookings. This analysis was performed using Power BI, a powerful data visualization and analytics tool.

# PROBLEM STATEMENT
AtliQ Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, AtliQ Grands are losing its market share revenue in the luxury/business hotels category.

# Objective: 
To provide AtliQ Grands with insights from their historical data to regain their market share and revenue.

# DATA SOURCING
The dataset used for this analysis was collected from Code Basics’ website.

# SKILLS DEMONSTRATED
This project exposed me to learning a lot using Microsoft Power BI.
· Multiple complex DAX formulas and Functions.
· Calculated columns
· Data Extraction, Cleaning, and Transformation (ETL)
· Data Modelling
· Data Visualization

# DATA MODELING
The data model in Power BI consists of five tables:

# dim_date: 
Contains full date information about dates including day type (weekend or weekday), month, and week number (W19 — W32). 
# dim_hotels: Stores identity number of the hotel, property name, category it belongs to (luxury/business), and the city it’s located. dim_rooms: Includes room id and room class. 
# fact_bookings: Stores information about bookings including booking dates, booking platforms, number of guests, revenue, check-in, and checkout dates. 
# fact_aggregrated_bookings: Includes successful bookings, hotel id, and capacity. The dimension tables (with the prefix “dim”) have a matching id in the fact tables (with the prefix “fact”). 
This modeling produces a one-to-many relationship.

![image](https://github.com/Dev-dataanalyst/AtliQ-Grand-Hospitality-Analysis--PowerBI/assets/143479964/e7d6c088-d55c-4a9e-bf75-a0225d6dd844)






