# Project Instructions

Write three SQL queries to answer the following questions:

- Find the number of unique individuals that use each garage’s shared charging stations. The output should contain two columns: `garage_id` and `num_unique_users`. Sort your results by the number of unique users from highest to lowest. Save the result as `unique_users_per_garage`.

- Find the top 10 most popular charging start times (by weekday and start hour) for sessions that use shared charging stations. Your result should contain three columns: `weekdays_plugin`, `start_plugin_hour`, and a column named `num_charging_sessions` containing the number of plugins on that weekday at that hour. Sort your results from the most to the least number of sessions. Save the result as `most_popular_shared_start_times`.

- Find the users whose average charging duration last longer than 10 hours when using shared charging stations. Your result should contain two columns: `user_id` and `avg_charging_duration`. Sort your result from highest to lowest average charging duration. Save the result as `long_duration_shared_users`.

Three SQL cells have been created for you in the workbook. To access the data, you will need to select data using the syntax `FROM VEHICLES.CHARGING_SESSIONS` - the schema and table names are case-sensitive, so please only use capital letters.

Note: Please also ensure that you do not change the names of the DataFrames that the three query results will be saved as - creating new cells in the workbook will rename the DataFrame (see image below). Make sure that your final solutions use the names provided: `unique_users_per_garage`, `most_popular_shared_start_times`, and `long_duration_shared_users`.

---------------------

As electronic vehicles (EVs) become more popular, there is an increasing need for access to charging stations, also known as ports. To that end, many modern apartment buildings have begun retrofitting their parking garages to include shared charging stations. A charging station is shared if it is accessible by anyone in the building.

But with increasing demand comes competition for these ports — nothing is more frustrating than coming home to find no charging stations available! In this project, you will use a dataset to help apartment building managers better understand their tenants’ EV charging habits.

The data has been loaded into an Azure Databricks database, containing a schema called vehicles and a single table named charging_sessions with the following columns:

![image](https://github.com/user-attachments/assets/8252be0b-9b2c-4f3a-b5fc-5bbbfbf0c022)

```SQL
-- unique_users_per_garage
-- Modify the code below
SELECT garage_id, COUNT(DISTINCT user_id) AS num_unique_users
FROM vehicles.charging_sessions
WHERE user_type = "Shared"
GROUP BY garage_id
ORDER BY num_unique_users DESC
```

![image](https://github.com/user-attachments/assets/8c050f0e-75c8-4b81-8f4e-a7cc383a3239)


```SQL
-- most_popular_shared_start_times
SELECT weekdays_plugin, start_plugin_hour, COUNT(*) AS num_charging_sessions
FROM vehicles.charging_sessions
WHERE user_type = "Shared"
GROUP BY weekdays_plugin, start_plugin_hour
ORDER BY num_charging_sessions DESC
LIMIT 10;
```

![image](https://github.com/user-attachments/assets/efe9cdc4-9bce-4896-a8fc-736550143906)


```SQL
-- long_duration_shared_users
SELECT user_id, AVG(duration_hours) AS avg_charging_duration
FROM vehicles.charging_sessions
WHERE user_type = "Shared"
GROUP BY user_id
HAVING AVG(duration_hours) > 10
ORDER BY avg_charging_duration DESC;
```

![image](https://github.com/user-attachments/assets/286b0040-5afd-40dc-8ffd-635e7f392896)
