---
layout: post
title: Predicting Agriculture Yield with Weather
---
![_config.yml]({{ https://media1.britannica.com/eb-media/90/94190-004-D8BC0070.jpg}}/images/weather_agriculture/wheat_image.jpg)


$\LaTeX$

## Background:
The global human population has been growing consistently and is expected to reach 9 billion by 2050. The average American consumes about 2000 pounds of food per year. Assuming these numbers hold true through 2050, there will be a significant increase in demand for food in the next few decades. Scientists have claimed that environmental degradation and variable weather conditions caused by climate change can potentially threaten the global food supply. In order to understand this relationship, the effect of different weather variables on crop yield is studied. California agriculture data from USDA National Agricultural Statistics Service is studied in order to understand the crop yield of corn and wheat in the nation's largest agriculture industry. Weather data on Fresno, California is collected from Weather Underground in order to specify the county with the highest crop yield in the state. Using these two data sources, an appropriate study can be done to predict the effect of weather on crop yield for the rest of the US.

## Approach:
The dependent variable is crop yield measured in BU/acre. The independent variables of interest are weather variables, such as maximum temperature, mean temperature, minimum temperature, heating days, cooling days, growing days, dew point, precipitation, wind, and sea level pressure, as well as population and year. This study was done on two different field crops: corn and wheat.

The relationship between the independent and dependent variables were modeled using linear regression techniques. The initial model contains all independent variables with the results analyzed using `statsmodels`. Variables with p-values greater than 0.05 were removed in order to focus the model on only statistically significant variables. A new model with fewer variables was analyzed to observe the changes in significance of variables. A heat map of the correlation between the variables helped remove variables that had strong correlation and did not improve the model. Each linear regression model was cross validated with 5-folds to test its capability to accurately predict crop yield based on new inputs.

Once the optimal variables had been identified, regularization with an alpha value that minimized mean squared error was applied to build a model with minimal overfitting. Three different techniques of regularization were applied: Ridge, Lasso, and Elastic Net. The regularization technique with the highest R-squared value from cross validation was chosen as the final model.

## Analysis:

### Corn Yield



### Wheat Yield


## Next Steps:
