# Linear Regression on Bike Share 

> Linear Regression model applied using RFE and manually adjusted variables

## Table of Contents

- [Linear Regression on Bike Share Scenerio](#linear-regression-on-bike-share-scenerio)
  - [Table of Contents](#table-of-contents)
  - [General Information](#general-information)
    - [Business Problem](#business-problem)
    - [Goal of the Project](#goal-of-the-project)
  - [Conclusions(Business Recomendation)](#conclusionsbusiness-recomendation)
  - [Result](#result)
  - [Technologies Used](#technologies-used)


<!-- You can include any other section that is pertinent to your problem -->

## General Information

### Business Problem

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

### Goal of the Project

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands


## Conclusions

1. Model Fit:

R-squared: 0.833 – This model explains about 83.3% of the variance in bike rentals, which is very strong. Adjusted R-squared: 0.830 – After adjusting for the number of predictors, the model still explains 83% of the variance, indicating a good fit. F-statistic: 249.2 (p-value: 7.37e-187) – The model is highly significant, and the predictors as a group are meaningful.

2. Coefficients (Impact of Predictors):

const: 0.1910 – The intercept term is the baseline value when all independent variables are zero. yr (year): 0.2341 – The number of bike rentals increases by approximately 0.2341 units for each year increase. holiday: -0.0969 – Bike rentals are lower on holidays by 0.097 units on average, a statistically significant result. temp (temperature): 0.4782 – For each increase of 1 degree in temperature, the number of rentals increases by 0.478, showing a strong positive relationship. windspeed: -0.1482 – For each unit increase in windspeed, the number of rentals decreases by 0.148, which is statistically significant. season_spring: -0.0551 – Spring season reduces rentals by about 0.055 compared to other seasons. season_summer: 0.0610 – Summer season increases rentals by 0.061, which is significant at p < 0.0001. season_winter: 0.0959 – Winter season increases rentals by 0.096, statistically significant. mnth_Sep (September): 0.0909 – Bike rentals in September are higher by 0.091, a statistically significant increase. weathersit_Cloudy: -0.0801 – Cloudy weather results in a decrease in rentals by 0.0801. weathersit_Rainy: -0.2860 – Rainy weather has a substantial negative effect on bike rentals, reducing them by 0.286, which is highly significant.

3. Statistical Significance:

Most predictors are statistically significant with p-values well below 0.05, suggesting that the relationships between these variables and bike rentals are not due to random chance. Holiday, windspeed, season, weather conditions, and temperature all have strong and meaningful effects on bike rentals.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Result

We achieved the following results:


- Adj. R-squared: 0.830
- Durbin-Watson value : 2.076

## Technologies Used

numpy version: 1.26.4
pandas version: 2.2.3
seaborn version: 0.13.2
statsmodels version: 0.14.4
scikit-learn version: 1.6.1
matplotlib version: 3.10.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


<!-- Optional -->

## License

This project is open source and available without restrictions.

<!-- You don't have to include all sections - just the one's relevant to your project -->
