# DemoPandas

This is a demonstrative example of Data analysis using Python Pandas library

## DataSet
- streams.csv - one row per date, country, region, gender
- n_of_streams - total number of spotify streams for the artist, that is how many times song of that artist were listened to (the entrire dataset relates to one artist only)


## What is shown in the example code
1. *General information*
    - dataset shape
    - min, max date available
    - number of countries, regions, genders
    - number of missing values for country, region, gender, streams

2. *Descriptive tables*
    1. per country
        - number of regions
        - total number of streams
        - average number of streams 
        - standard deviation  
        - percentage of total number of streams
    2. per gender
        - number of streams
        - percentage of streams
        - number of distinct regions

3. *Outlier detection*
    - Create  "_outlier" variable of boolean type
    - Assign a value **True** if the row is considered an outlier, and **False** if not
    - A row is considered an outlier if the value of n_of_streams is out of +-1.5*IQR for country, region, gender group

4. *Spike*
 a spike is defined as an occasion when the moving average for the number of streams forprevious 3 days (MA3) proceeds the moving average for the number of streams for previous 10 days (MA10) by 10 percent.

## BONUS
Visualization with *matplotlib*


