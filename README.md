# ETL

The purpopse of this project was to see if there was any correlation between the best selling games and the highest reviewed games.

# Data Source
https://www.kaggle.com/gregorut/videogamesales
https://www.kaggle.com/juttugarakesh/video-game-data
We used 2 different CSV files for this. One that contained all video game reviews and another that contained all video game sales.

# Data Transformation
We filtered out user_score with the "tbd" acronym on them.
We did not filter out the games with 'NA' on the review section of the tables because we found that some of the highest selling games of all time came out many moons ago and it would be unfair and inaccurate to filter out some of the best selling games of all time only because they were not reviewed then.
We joined the 2 tables together by 'name', 'year of release', and 'platform'.
We used the example of the platform Wii because it had the highest selling game of all time. We aggregated the global sales by year of release and found that the longer the system was out the trend in sales would decrease. Nevertheless Wii Sports on the Wii had more than double the sales of the 2nd best selling game of all time. 
We loaded the CSV files in a MySQL database.

# Conclusion
We chose these databases because we wanted to see if the highly reviewed games would affect the trend in sales.
We found that there is little correlation between higher critically acclaimed games and sales and even less correlation between higher user reviewed games and sales. If we had more time we would look for a database with marketing money spent on the highest selling games and see if there is a correlation there.  
