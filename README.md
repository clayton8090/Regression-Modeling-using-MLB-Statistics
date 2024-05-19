
Executive summary:

In this study, we conducted exploratory data analysis and built multiple regression models to investigate the relationship between various offensive statistics and the number of runs scored in baseball. We evaluated the models using metrics such as mean squared error and Bayesian information criterion and found that a Poisson regression model with total hits, plate appearances, singles, doubles, triples, and walks as predictor variables performed the best.
We analyzed the coefficients of the model to determine the relative importance of each offensive statistic in predicting the number of runs scored. Some variables, such as singles and walks, had unexpected signs, suggesting complex relationships between these variables and the response variable in a team sport like baseball.
Our findings indicate that certain offensive statistics are more important than others in predicting the number of runs scored, and that a Poisson regression model can be an effective tool for this type of analysis. However, further research is needed to fully understand the complex factors that can affect the relationships between these variables.


Problem: 

The data set we choose for this project is 2020-2022 offensive baseball statistics. Our source of the data is Baseball Savant,  a major league baseball affiliated data repository for everything professional baseball. The goal of the report is to make a model using limited offensive stats to predict runs. Runs are a good measure of offensive performance as they are the points scored by players. In baseball the primary goal is to have more runs at the end of the game than the opposing team. 

The family of regression analysis we are using is poisson. The baseball regular season is 162 games every year for each team ( even if games are canceled they are made up eventually before the season starts). Poisson distribution is a statistical distribution that models the probability of rare events occurring in a fixed interval of time or space, given the average rate at which these events occur. This is consistent with how baseball is played and the data collected for it and is more optimal than a general linear model. This is due to baseball data being non-negative. Linear models have the potential to give negative numbers which are not in the feasible region for prediction. 
