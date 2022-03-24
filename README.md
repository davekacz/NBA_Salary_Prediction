# NBA Salary Prediction

Georgia Tech ISyE 7406 DMSL Final Project

## Questions to answer after training models

* Who are the highest value players?  Players the model thinks should be paid more than they actually are.  What teams has the most value, the least.  

Once we come up with best performing model, can grab the best estimator from all the training.

Train the model on all previous season data.  Apply a scaling factor where appropriate on current season data, then predict on it.  

Inaccuracies aren't exactly *wrong*.  We can consider the results what a player is actually worth.  Doing some testing on the simple models, Steph Curry in 2019 was worst prediction.  Something like 30M difference.  But that season he was hurt and only played 5 games.  So maybe he wasn't worth his 40M contract?  

Anyway we can see what our model thinks a player is worth, highlight some highs and lows.  Then do a groupby on teams and do the same.  


* Regular Stats vs Advanced Stats.  Does including advanced stats in the model make them perform significantly more accurately?  Not sure if I feel like adding this...  

## Data Clean Up Notes

* Data scraped, cleaned, organized. -- Done

* Traded players combined.  Some columns averaged, some added.  This may not be perfect depending on games played splits for averages.  -- Done

* ~~Position has been one hot encoded.  Earlier data lists PF, PG, SG, etc...  later data is G, F, C we may want to just make 3 dummy variables?  Transfer PF to F, PG to G...~~

* Some salary data missing.  Some noticible players, but very few.  These rows dropped. -- Done

* About ~1800 ORTG and DRTG values missing.  Otherwise all data is there.  These columns have been dropped -- Done

## Explore Data

* Covariance Plots, Violin/Histogram plots

* Data is right skewed, see histogram plot of salary. Box-Cox transformation helps this.  Also gets rid of need to transform salaries based on year/salary cap.  See data explore notebook -- Done

## Model to do

* Normalize, standardize data? -- Done

* Variable Selection -- Done

### Regression Methods - Possible Models to use

https://scikit-learn.org/stable/supervised_learning.html

* Linear Regression: OLS, Ridge, Lasso, Elastic Net -- Done
* Support Vector Machines -- Done
* Nearest Neighbors -- Done
* Tree models (random forest) -- Done
* Ensemble Methods: Bagging, aDaBoost

### Scoring

* When we cross validate should we drop the same players through all years?

* Will need to transform results from models with inverse box cox transformation to come up with meaningful analysis.


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

