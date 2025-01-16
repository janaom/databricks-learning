# Project Instructions

Write three SQL queries to answer the following questions:

- What are the most popular transport types, measured by the total number of journeys? The output should contain two columns, 1) `journey_type` and 2) `total_journeys_millions`, and be sorted by the second column in descending order. Save the query as `most_popular_transport_types`.

- Which five months and years were the most popular for the Emirates Airline? Return an output containing `month`, `year`, and `journeys_millions`, with the latter rounded to two decimal places and aliased as `rounded_journeys_millions`. Exclude null values and save the result as `emirates_airline_popularity`. Note - in Databricks SQL, aliased column names cannot be used in a `WHERE` clause, you will need to use original column names.

    Find the five years with the lowest volume of `Underground & DLR journeys`, saving as `least_popular_years_tube`. The results should contain the columns `year`, `journey_type`, and `total_journeys_millions`. 

Three SQL cells have been created for you in the workbook. To access the Databricks database, you will need to select data using the syntax FROM `tfl.journeys` (selecting from `journeys` without referring to the `tfl` schema first will result in an error).

Note: Please also ensure that you do not change the names of the DataFrames that the three query results will be saved as - creating new cells in the workbook will rename the DataFrame (see image below). Make sure that your final solutions use the names provided: `most_popular_transport_types`, `emirates_airline_popularity`, and `least_popular_years_tube`.

-------------------------

London, or as the Romans called it "Londonium"! As of 2021, Greater London is home to over 8.5 million residents who speak over 300 languages. While the City of London is a little over one square mile (hence its nickname "The Square Mile"), Greater London has grown to encompass 32 boroughs spanning a total area of 606 square miles!

Given the city's roads were originally designed for horse and cart, this area and population growth have required the development of an efficient public transport system! Since the year 2000, this has been through the local government body called Transport for London, or TfL, which is managed by the London Mayor's office. Their remit covers the London Underground, Overground, Docklands Light Railway (DLR), buses, trams, river services (clipper and Emirates Airline cable car), roads, and even taxis.

The Mayor of London's office makes their data available to the public here

. In this project, you will work with a slightly modified version of a dataset containing information about public transport journey volume by transport type.

The data has been loaded into a Databricks database containing a schema called `tfl` with a single table called `journeys`. The table, which you will use for the project, includes the following data:

![image](https://github.com/user-attachments/assets/d950229e-16fd-4fdd-953b-7233a09d1750)

```SQL
-- most_popular_transport_types
-- modify the query below as required
SELECT journey_type, 
	SUM(journeys_millions) as total_journeys_millions
FROM tfl.journeys
GROUP BY journey_type
ORDER BY total_journeys_millions DESC;
```

![image](https://github.com/user-attachments/assets/803d1ea4-2303-479a-9f58-1f80a6f6b960)


```SQL
-- emirates_airline_popularity
SELECT month, 
	year, 
	ROUND(journeys_millions,2) AS rounded_journeys_millions
FROM tfl.journeys
WHERE journey_type = 'Emirates Airline' AND journeys_millions IS NOT NULL
ORDER BY rounded_journeys_millions DESC
LIMIT 5;
```

![image](https://github.com/user-attachments/assets/5e59b817-3de7-4162-ad04-73ffe3955a6a)

```SQL
-- least_popular_years_tube
SELECT year,
	journey_type,
	SUM(journeys_millions) as total_journeys_millions
FROM tfl.journeys
WHERE journey_type LIKE '%Underground%'
GROUP BY year, journey_type
ORDER BY total_journeys_millions
LIMIT 5;
```

![image](https://github.com/user-attachments/assets/3ed0249a-47e2-4662-826e-5cb631660e1c)
