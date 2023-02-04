# Expected Goals Estimator (Football): Project Overview

* Created a tool that estimates the number of goals that will be scored throughout the season to help football scouts with the recruitment of 
prospect palyers.
* Scraped around 3000 players statistics playing in the top 5 leagues from FBref.com using Pandas.
* Engineered features to give more edge for players playing in top teams and in leagues that usually concedes more goals.
* Optimized Linear, Lasso Regressions, and Random Forest Regressors using GridsearchCV to discern the best model.
* Built a client facing API using Flask

# Code and Resources Used

**Python Version:** 3.7\
**Packages:** Pandas, numpy, sklearn, matplotlib, seaborn, flask, json, pickle

# Web Scrapping

Utilized `pandas.read_html` to scrap around 3000 player stats in 2021/2022 season from FBref.com; each player got the following:

* Player
* Nation
* Position
* Squad
* Competition
* Age
* Shot Creating chances
* Completed passes that lead to shots
* Goal creating Actions
* Completed passes that lead to a goal
* Successful dribbles that lead to goal
* shots that lead to a goal scoring shots
* Assists

# Data Cleaning

After scrapping the data, I needed to clean it up to make it more usable to the model. I did the following actions:

* Removed rows with missing records
* Removed irrelevant features such as: Born Year
* Removed expected goals and assists which was calculated with respect to last season's stats
* Made a new column denoting wether a player is playing for a top team or not
* Made a new column denoting wether a player is very involved in the offensive animation

# Data Exploratory Analysis

I looked at the distribution and value counts for different variables. Below are a few highlights of the conducted analysis.

# Model Performance 

* **Linear Regression:** MAE = 0.027
* **Lasso Regression:** MAE = 0.027
* **Random Forest:** MAE = 0.063



