# NBA Salary Prediction

The National Basketball Association (NBA) is a professional basketball league in the United States. With 210.2 million followers across all social media platforms, it is one of the most popular sport games in the world. Fans in the United States spend hundreds of dollars watching NBA games in the stadiums which creates revenue for the teams to pay the salary to obtain existing players or trade potential players from other teams. Thus, the salaries of the players is one of the hottest topics on social media and the news. 

In this final project, we will use past and current players’ demographic and regular season performance data to analyze the parameters and come up with models that can best predict the salaries of the players. The data set will be split into training and testing data sets and utilize K-Fold cross validation. We will be building multiple linear regression, Support Vector Machine (SVM), K Nearest Neighbors (KNN), random forest, and ensemble methods such as AdaBoosting models based on the training data set. The testing data set will be used to examine the accuracy or testing error of the models.  

We have concluded that the random forest is the best performing model and the SVM is the worst performing model. In addition, we identified the overpaid and underpaid players and explained the difference between predictions and their salaries by the actual trading situations. 

### File Overview

#### Folders
* Data includes the datasets we created from the following sources:  
* 
Player statistics and performance analytics: https://www.nbastuffer.com/2020-2021-nba-player-stats/ 

Season Salary Caps:  https://www.spotrac.com/nba/cba/ 

Player Salaries: https://hoopshype.com/salaries/players/2020-2021/ 


* Images includes some of the images we utilized for the report
* Results includes the output of SKLearns Grid Search CV on all our models
* Tableau Files includes the files we built in tableau for visualizations.

#### Files
* 2021_predictions.csv - The output of our analysis applied to the 2021 season.  Shows players and their predicted and true salaries in 2021.
* README_notes.md - Our readme while we working on the project to jot notes down on.
* data_explore.ipynb - Our initial file to explore the data.  Includes lots of plots.
* data_prep.ipynb - The file we used to scrape and build the dataset to be input into the model.  Includes all the data cleaning operations.  
* model_results.csv - Includes all the results from the training of the models.  
* model_explore.ipynb - Includes our first attempt at training some models to get an idea of what would work well.  
* models_final.ipynb - The file that trains all of our models to the find the best performing model.  
* review_results.ipynb - The file to review the models as well as the file used for our analysis on the 2021 season.
