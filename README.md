# Hotel_DashBoard
Develop a database to analyze and visualize 
![](hotel_image.jpg)


This project is aimed at giving business insights of an hotel so as to aid the management to make/take progressive decisions. 
A dashboard will be created to present to stakeholders.

## Problem Statement 
1. is our hotel revenue growing yearly?
2. should we increase our parking lot size?
3. what trends can we see in the data?

## Data Analysis project pipeline
 ----
* Build a Database
* Develop the SQL Query
* connect Power Bi to the Database
* Visualize
* Summarize findings

## Skills used in the project
 MySQL server management studio, Powerbi 

## Data Transformation
   we will be performing exploratory analysis on the data set in this project so as to help answer the business questions required. The flat file is in csv which was uploaded into SQL server management studio where most data wrangling  was carried out before connecting the database to Powerbi using power Query.

## Creating a Database
A new database was created with the name Historical Hotel.
The excel was upload with aid of the import & export wizard.
Next was to choose a data source, in this case our data source will be from Microsoft excel, The file path will be the excel file we want to work with and lastly I pick the 2007-2010 version of Excel from the drop down. 
NB: This might not be the same for everyone. I tried choosing the recent version but kept getting errors. I was frustrated for a sec(emoji) but I tried every version in the drop down till I got no error prompt.
Data Enriching
Querying the 2018,2019 & 2020 tables to have a detailed look at the fields was quite difficult studying each table in different windows. The tables were appended making use of " union" operator to have a unified data set. 
A table function(common table expression) was created encapsulating the query into one table and rename as "Hotels".
Image

# Exploratory Analysis & Developing SQL Query
First, the revenue column was created using the adr, stay in week nights & stay in weekend nights.
The "group by “aggregate operator was used to on the year & hotel type column to see if there is a trend in the revenue. 

The market segment & meal ticket table were merged with the hotels table making use of the left join clause. 

# Connect Power Bi to the Database 
 
Import the SQL query through the get data button on Power Bi. 
Measures were created and used to replace calculated columns for better visualizations. 

# Visualization 
	image
# Summary Findings

Based on the exploratory analysis, it was discovered that the hotel revenue has been growing steadily from 2018 to 2020. Also, there was a significant increase in revenue from the second quarter of each year. This could be an indication of a high demand for hotel services during this period, which could inform the hotel management to increase their marketing and promotional activities during this period.

It was also discovered that the parking lot size may not need to be increased as the hotel's revenue does not seem to be significantly affected by the availability of parking spaces.

Furthermore, trends in the data show that the majority of the hotel's revenue is generated from guests who book through online travel agencies and those who book directly with the hotel. This information could help the hotel management focus their marketing efforts towards these channels.

In summary, this data analysis project has provided valuable insights to aid the hotel management in making progressive decisions that could enhance their revenue and overall business performance.

