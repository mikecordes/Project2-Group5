## Team 5: Demi Ola, Jamie Leon, and Michael Cordes

## Summary

This repository contains a machine learning model that conducts an analysis of historical fantasy football (NFL)  data from 1970 - 2019. 

### Our Data
---
We researched historical fantasy football data and located a data set that contained fifty years of season statistics and fantasy scores saved in .csv format.  Each year saved to it's own .csv (50 csv files total!).  

The process we elected to use to process that many .csv files into one dataframe is the Glob function.  This was able to work since the .csv files were in a standardized format.  The only datapoint missing in our .csv files was the year of the corresponding data.  This was solved by using the file name, which happened to be the year.  We ran a for loop to read each .csv , add a column for the year and append it to the frame.  Once we had each .csv read, we appended all the data to one dataframe.  This resulted in a dataframe that had 2,500 rows and 29 columns.  

We elected to sperate the large dataframe into positional dataframes.  Each dataframe would contain all the players listed at the position.  The positions are quarterback (QB), running back(RB), wide receiver (WR), and tight end (TE).  This approach allowed us to ensure the model provided an accurate prediction for the positions.  


### Our Model 
---
We elected to use a Linear Regression Model to identify is there is a correlation between the age of the player and fantasy points scored.  The model should be able to tell us what age groups to avoid at each position.  

The model showed that we should target certain ages groups for certain positions:

 - QB - 28  yrs - 34 yrs
 - RB - 21 yrs  - 23 yrs 
 - WR - 26 yrs - 34 yrs
 - TE - 25 yrs - 30 yrs



### Files

Placeholder for notebook link

CSV files for each year from 1970 - 2019]

PNG file 1

PNG file 2


The files below are the resource files.

## Why Fantasy Football?
![enter image description here](http://gridironexperts.com/wp-content/uploads/2015/08/Fantasy-Football-Meme-2015.jpg)

### Resources

[Fantasy Football Data Pros (fantasyfootballdatapros.com)](https://www.fantasyfootballdatapros.com/csv_files)

[The Fantasy Footballers (fantasyfootballers.com)](https://www.thefantasyfootballers.com/articles/history-fantasy-football/)

Conlon, Rose and Uhler, Andy.  "How fantasy football became a billion-dollar industry",
MarketPlace, September 6, 2021, [How fantasy football became a billion-dollar industry - Marketplace](https://www.marketplace.org/2021/09/06/how-fantasy-football-became-a-billion-dollar-industry/) (https://www.marketplace.org/2021/09/06/how-fantasy-football-became-a-billion-dollar-industry/)


----------
