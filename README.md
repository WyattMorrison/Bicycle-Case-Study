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

##Distribution of riders in year 2022
<img src="images/Total%20Trips%20By%20Member.png" />
There are 4.1 million trips in total in 2022. There were 2,505,317 member riders which constitutes 60.8% of all riders and 1,615,551 casual riders which constitutes 39.2% of all riders.
<img src="images/Total%20Trips%20Dash.png" /> 
Classic bikes are the most common among riders and electric is the second most common. Meanwhile, docked bikes are far less popular for riders. Member riders primarily use classic bikes, but even though they only use electric bikes half as much, there are still a large amount of member riders that use electric bikes. For casual riders it is almost an even split between classic and electric bikes. For docked bikes, no members use them and only a smaill percentage of casual riders use this type of bike.

##Number of Trips 
<img src="images/Trips%20By%20Month%20Dash.png" />
<img src="images/Trips%20By%20Day%20Dash.png" />
<img src="images/Trips%20By%20Hour%20Dash.png" />
<img src="images/Duration%20By%20Month%20Dash.png" />
<img src="images/Duration%20By%20Day%20Dash.png" />
<img src="images/Duration%20By%20Hour%20Dash.png" />
<img src="images/Distance%20By%20Month%20Dash.png" />
<img src="images/Distance%20By%20Day%20Dash.png" />
<img src="images/Distance%20By%20Hour%20Dash.png" />
<img src="images/Distance%20By%20Bike%20Dash.png" />
<img src="images/Start%20Location%20Dash.png" />
<img src="images/End%20Location%20Dash.png" />

