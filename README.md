# Bicycle-Case-Study

## Introduction
Cyclistic is a bike-share program that features more than 5,800 bicycles and 600
docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand
tricycles, and cargo bikes, making bike-share more inclusive to people with
disabilities and riders who can’t use a standard two-wheeled bike. The majority of
riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic
users are more likely to ride for leisure, but about 30% use them to commute to
work each day.

Until now, Cyclistic’s marketing strategy relied on
building general awareness and appealing to broad consumer segments. One approach that
helped make these things possible was the flexibility of its pricing plans: single-ride passes,
full-day passes, and annual memberships. Customers who purchase single-ride or full-day
passes are referred to as casual riders. Customers who purchase annual memberships are
Cyclistic members.

Cyclistic’s finance analysts have concluded that annual members are
much more profitable than casual riders. Although the pricing flexibility helps Cyclistic
attract more customers, executives believe that maximizing the number of annual members
will be key to future growth. Rather than creating a marketing campaign that targets all new customers, executives believe there is a very good chance to convert casual riders into
members. She notes that casual riders are already aware of the Cyclistic program and have
chosen Cyclistic for their mobility needs.
## Ask
Three questions will guide the futture marketing program:
1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclisttic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?
## Data Source & Credibility
**Source:** The data used is from https://divvy-tripdata.s3.amazonaws.com/index.html. It was located in zip files according to month and    year.

**Reliability:** The data is very reliable with over 5 million records. That is enough to dampen the effects that outliers may have within  the analysis.

**Comprehensiveness:** The data provides comprehensible attributes to perfrom a thorough analysis. Some of the atttributes observed include: rider id, bike type, member type, start time, end time, start location, and end location.
##Process
With there being over 5 million rows of data, SQL was used to clean and analyze the data.

#### Data Cleaning & Manipulation
1. The tables were first renamed to make it easier to read. For example I changed "202201-divvy-tripdata.csv" to "Jan_2022.csv."
2. The 12 datasets (1 for each month) were then imported into SQL and merged into one table named "Bike_Trips_2022." The table has a total of 5,667,717 rows.

<img src="images/Union%20Code.PNG" />

3. The following code was used to clean and manipulate the data.

<img src="images/Cleaned%20Table%20Code%20pt1.PNG" />
<img src="images/Cleaned%20Table%20Code%20pt2.PNG" />
<img src="images/Cleaned%20Table%20Results.png" />

After running the code, there was 4,120,868 rows remaining.

## Distribution of riders in year 2022
<img src="images/Total%20Trips%20By%20Member.png" />

There are 4.1 million trips in total in 2022. There were 2,505,317 member riders which constitutes 60.8% of all riders and 1,615,551 casual riders which constitutes 39.2% of all riders.

<img src="images/Total%20Trips%20Dash.png" /> 

Classic bikes are the most common among riders and electric is the second most common. Meanwhile, docked bikes are far less popular for riders. Member riders primarily use classic bikes, but even though they only use electric bikes half as much, there are still a large amount of member riders that use electric bikes. For casual riders it is almost an even split between classic and electric bikes. For docked bikes, no members use them and only a smaill percentage of casual riders use this type of bike.

## Number of Trips 
<img src="images/Trips%20By%20Month%20Dash.png" />

The trend shows that the number of trips increases to July where the peak is around 600k trips and then the number of trips starts to decrease through December. This shows that Q2 and Q3 are the most popular riding times for riders and any advertising or business plans should take this trend into account.

<img src="images/Trips%20By%20Day%20Dash.png" />

The member riders do more trips during the weekdays with Tuesday, Wednesday, and Thursday being the most popular. The casual riders do more trips during the weekends, especially on Saturday and combined, Saturday is the busiest overall day for riders.

<img src="images/Trips%20By%20Hour%20Dash.png" />

The casual riders see their number of trips increase until it peaks at 5:00 PM and then begins to decrease. Member riders see a surge in usage during morning and evening rush hours.

## Duration of Trips
<img src="images/Duration%20By%20Month%20Dash.png" />

The average ride duration for members was consistent throughout the year. For casual riders, the months of March, April, and May had longer ride durations in comparison to other months.

<img src="images/Duration%20By%20Day%20Dash.png" />

For ride duration by day, members are consistent during the week with a slight increase on the weekends. Casual riders have some fluctuations during the week and see a large increase during the weekends.

<img src="images/Duration%20By%20Hour%20Dash.png" />

Member riders' ride duration is reletively consistent throughout the day. Casual riders' ride duration fluctuates throughout the day, with the longest ride durations being between 10:00 AM and 2:00 PM.

Overall, casual riders' ride duration is about 2-2.5 times longer than member riders throughout the year,week, and day. While casual riders have longer ride duration in comparison to member riders, they ride less frequently.

## Distance of Trips
<img src="images/Distance%20By%20Month%20Dash.png" />

During December, January, and February both casual and member riders have the smalled amount of distance travelled mainly due to weather. For casual riders, April, May and June are the peak months for distance travelled. Meanwhile, member riders' peak months are June, July, and August. Overall, casual members have slighly longer ride distances for most months compared to member riders.

<img src="images/Distance%20By%20Day%20Dash.png" />

For distance travelled by day both casual and member riders follow the same pattern throughout the week. There is a slight increase in distance on Wednesday's compared to the other weekday's and then the distance travelled peaks during the weekends. The only difference is that casual riders have a travel distance that is slightly longer than members. 

<img src="images/Distance%20By%20Hour%20Dash.png" />

On average, casual riders have a longer travel distance of 2.30 kilometers compared to 2.15 kilometers for members. Members' peak riding hours are between 4:00 AM and 7:00 AM while casual riders' peak riding hours are between 10:00 AM and 5:00 PM.

<img src="images/Distance%20By%20Bike%20Dash.png" />

For bike types, the ride distance varies. Classic bikes have a big difference in distance travelled between the ttwo rider types, with casual riders having a distance of 2.3 kilometers and members having a distance of 2.05 kilometers. Docked bikes have the longest distance travelled with casual riders travelling on average 2.65 kilometers (members did not have any data for docked bikes). Lastly, electric bikes are similar with casual riders having a average distance travelled of 2.34 kilometers compared to 2.35 kilometers for members.

<img src="images/Start%20Location%20Dash.png" />
<img src="images/End%20Location%20Dash.png" />

