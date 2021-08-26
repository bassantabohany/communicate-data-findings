# Ford GoBike Data Visualiztaion 
## by Bassant Hany

This data set includes information about individual rides made
in a bike-sharing system covering the greater San Francisco
Bay area for the month February, 2019 

## The dataset includes:

* an ID number for each bicycle
* how long it was rented for, in seconds
* the beginning and end staton ID, latitude, longitude and station name
* the start and end time
* the year the user was born
* the gender of the user
* the user type

## Cleaning Steps:

* dropped records with NaN values
* droped all columns related to beginning and end station except for their names columns
* droppd the bike_share_for_all_trip column
* changed the type of start_time, end_time to datetime
* changed the type of user_type, member_gender to categorical
* changed birth_year to intger
* changed bike_id to string
* added a new column for the trip day of week extracted from start_time
* added a new columns for both trip start and end hour extracted from start_time and end_time respectivley 
* added a new column for member age by substracting birth_year from 2019
* added a new column to show trips duration in minutes by dividing duration_sec by 60

## Main Features 
* User_type
* Start_Hour

## Summary of Findings
* Found out that 90.5% of users are subscribers 
* found out that'Market St at 10th St' and 'San francisco caltrain station 2' are the most popular stations at both starting and ending trips
* The most popular hours were 8:00 AM and 5:00 PM, which are one hour before work starts and the hour work ends, which conclude that people tend to rent bikes right before going to work or right after finishing work
* found out that most users are aged between 30 - 40 years old
* Trip durations are mostly the same during the week except for friday is slightly lower than the rest 
* Monday is the day with the highest usage for both subscribers and customers
* customers have higher usage percentage during the weekend 
* Most trips last for about 120 minutes
* customers tend to use their bikes more during rush hours
* Male users are much much higher than other genders

## Key Insights for Presentaion:
* First i want to show the percentage of each user type and how most users are subscribers,and i want to show what hours of the day are most popular to start your trip by using histogram and i want to show the what days are most popular for trips among both types of users and i wanted to show the relation between member age and trip duration, finally i wanted to show the relation between both user types and trip ending hour and days of the week to gain some new insights 

## Resources
* https://github.com/dirkkadijk/Ford-GoBike-Data-Exploration-and-Communication-of-insights
* https://github.com/mnalmelihi/udacity-dand-communicate-data-findings-ford-GoBike
