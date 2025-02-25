# EuropeanFootball

archive.zip file contains all the leagues that are there in Europe

The file is in zip format so the first step is to unzip the file and save it

The next step is using ADF to extract all the files present

Combined_matches.csv holds the main data. Used League column to create partitions and stored in parquet format

Using Unity Catalogue read files from the silver container, create the league tables based on seasons and create the table

The delta table would have the following information
1. Season
2. Team
3. Goals Scored
4. Goals Against
5. Goal Difference
6. Number of matches won
7. Number of matches lost
8. Number of matches drawn
9. Points

The table would be ordered based on points

Note :- If points are equal I have taken goals scored into consideration. However in real time it depends on different factors which I have not experimented yet
