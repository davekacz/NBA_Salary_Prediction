## Data Clean Up Notes

* Data scraped, cleaned, organized. 

* Traded players combined.  Some columns averaged, some added.  This may not be perfect depending on games played splits for averages.  Added a traded field

* Some salary data missing.  Some noticible players, but very few.


## Questions to Answer after training models

* Who are the highest value players?  Players the model thinks should be paid more than they actually are.  What teams has the most value, the least.  

* Regular Stats vs Advanced Stats.  Does including advanced stats in the model make them perform significantly more accurately?  

## Explore Data

* Covariance Plots, Violin/Histogram plots

## Model to do

* Normalize, standardize data?
* Variable Selection

### Regression Methods

https://scikit-learn.org/stable/supervised_learning.html

* Linear Regression: OLS, Ridge, Lasso, Elastic Net
* Support Vector Machines
* Nearest Neighbors
* Tree models (random forest)
* Ensemble Methods: Bagging, aDaBoost