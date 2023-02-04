# Expected Goals Esrimator (Football): Project Overview

* Created a tool that estimates the number of goals that will be scored throughout the season to help football scouts with the recruitment of 
prosepect palyers.
* Scraped around 3000 players statistics playing in the top 5 leagues from FBref.com using Pandas.
* Engineered features to give more edge for players playing in top teams and in leagues that usually concedes more goals.
* Optimized Linear, Lasso Regressions, and Random Forest Regressors using GridsearchCV to discern the best model.
* Built a client facing API using Flask

# Code and Resources Used

**Python Version:** 3.7\
**Packages:** Pandas, numpy, sklearn, matplotlib, seaborn, flask, json, pickle

# Web Scrapping

Utilized `pandas.read_html` 

# Model Performance 

* **Linear Regression:** MAE = 0.027
* **Lasso Regression:** MAE = 0.027
* **Random Forest:** MAE = 0.063



