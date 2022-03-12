# NBA Salary Prediction

Georgia Tech ISyE 7406 DMSL Final Project

## Questions to answer after training models

* Who are the highest value players?  Players the model thinks should be paid more than they actually are.  What teams has the most value, the least.  

* Regular Stats vs Advanced Stats.  Does including advanced stats in the model make them perform significantly more accurately?  

## Data Clean Up Notes

* Data scraped, cleaned, organized. 

* Traded players combined.  Some columns averaged, some added.  This may not be perfect depending on games played splits for averages.  

* Traded column not working correctly.  Can revisit or just drop.  

* Position has been one hot encoded.  Earlier data lists PF, PG, SG, etc...  later data is G, F, C we may want to just make 3 dummy variables?  Transfer PF to F, PG to G...

* Some salary data missing.  Some noticible players, but very few.  These rows dropped. 

* About ~1800 ORTG and DRTG values missing.  Otherwise all data is there.  

## Explore Data

* Covariance Plots, Violin/Histogram plots

## Model to do

* Normalize, standardize data?
* Variable Selection

### Regression Methods - Possible Models to use

https://scikit-learn.org/stable/supervised_learning.html

* Linear Regression: OLS, Ridge, Lasso, Elastic Net
* Support Vector Machines
* Nearest Neighbors
* Tree models (random forest)
* Ensemble Methods: Bagging, aDaBoost

## Other thoughts

How to handle 2020 covid season

How to handle current partial season data.  

### Sources

Players Stats:
https://www.nbastuffer.com/2020-2021-nba-player-stats/

Salary Cap:
https://www.spotrac.com/nba/cba/

Player Salaries:
https://hoopshype.com/salaries/players/2020-2021/

