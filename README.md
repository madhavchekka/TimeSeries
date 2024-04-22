# AdEase
is an ads and marketing based company helping businesses elicit maximum clicks @ minimum cost. AdEase is an ad infrastructure to help businesses promote themselves easily, effectively, and economically. The interplay of 3 AI modules - Design, Dispense, and Decipher, come together to make it this an end-to-end 3 step process digital advertising solution for all.

## Problem Statement:
1. To understand the per page view report for different wikipedia pages for 550 days. [Dataset](https://www.kaggle.com/datasets/saimaharana/adease/data)
2. To forecast the number of views to predict and optimize the ad placement for clients
3. To provide clients (different regions) with data on how their ads will perform on pages in different languages

## Steps Performed: [Link to Code](https://github.com/madhavchekka/TimeSeries/blob/main/Project%20Ad%20Ease.ipynb)
1. Data Pre-processing
2. Exploratory Data Analysis 
3. Feature Engineering 
4. Data Aggregation by Language
5. Graphical Data Analysis including ACF & PACF plots 
6. Time Series Decomposition - Trend, Seasonality, and Residual
7. Stationarity Tests - Dickey-Fuller Test 
8. Exploring different forecasting techniques to acheive **MAPE** < 5%  
   i. Simple Exponential Smoothing  
   ii. Double Exponential Smoothing  
   iii. Triple Exponential Smoothing  
   iv. Auto Regression, Moving Average, ARIMA, SARIMA, and SARIMAX models  
   v. Facebook Prophet Library


## Inferences :
1. There are also mediawiki & commons.wikimedia pages that host media are available in the dataset
2. Of the pages from 7 different languages, English has the highest proportion, closely followed by Japanese. Rest of the languages roughly have same proportion of ~12%
3. AccessOrigin is spider for ~24% of the pages and all-agents for ~76%
4. AccessType is all-acess for about 50% of the pages. Then for desktop & mobile-web is ~25% each
5. During the months of August 2016, there is a spike in daily average views of both English & Russian pages
6. Also, a spike is observed in Nov,2016. This time for pages in Spanish, Russian, and German as well
7. English average views seem to have trend & seasonality where as other languages have seasonality mostly
8. In daily median views, Spanish language pages seem to be higher than other language pages
9. Spanish, Russian, and English median daily views had a drop.
10. In later months of 2016, english pages median daily views is on part with that of Spanish

## Recommendations:
1. English has high average daily views compared to other languages. Recommend running more ads in English pages
2. There are more than 50% of pages with all-access compared to desktop & mobile-web alone
3. Knowing the language for mediawiki & commons.wikimedia would enhance our training data further
4. Like campaign data for English pages, availability of such exogenous data would improve model predictions
5. With more time and resources, we can experiment with prophet parameters to bring better MAPE values.
