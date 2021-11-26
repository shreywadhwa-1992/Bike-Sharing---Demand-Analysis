# Bike-Sharing---Demand-Analysis
Importance of Simple Regression Techniques - Multiple Linear Regression

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short-term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.
 
A US bike-sharing provider has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

In such an attempt, aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all-around and stand out from other service providers and make huge profits.

They want to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:-
1. Variables, which are most significant in predicting the demand for, shared bikes.
2. How well these factors/variables describes the bike demand. 


Approach towards the problem:- 

1. Understanding Business Goal:
We are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

2. Understanding the Data:
Data comprises of "cnt" variable that is the target variable. It tells about the demand of shared bikes at a particular moment. cnt variable is subdivided into casual users and registered users.
"Registered" user’s rentals shares major percentage of Total rentals of bikes.
There are other variables such weather situation, season, workingday, holiday, temperature, humidity etc. that can be considered as factors which affects the demand on the bikes. We have extract the factors, which are contributing towards the demand of Total bike rentals.

3. Data Cleaning:
- Correcting datatypes
- Handling-missing values.
- Mapping variables to more readable form.

4. Exploratory Data Analysis:
It is said that more than half of the war is won by performing EDA only. Similarly, in this case EDA led to many insights about the variables, which can be a key contributor towards bike demands.
Following analysis were performed.
- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis

5. Data preprocessing before building a model:
- Handling categorical variables using ordinal encoding and dummy encoding.
- Handling id and date columns
- Normalizing the Numeric variables/columns.

6. Model Building – MLR
- Multiple Linear Regression model with recursive feature elimination and variance inflation factor.
- Model was trimmed down to only 9 variables making it leaner and also making the company to easily target these factors.
- Performance metric of R2_Scsore was chosen was evaluating the model’s performance.
- After building the model, Residual Analysis, Homoscedasticity of residuals was checked to evaluate the model for under fitting problem. 

7. Recommendations:
- Top 5 variables that are contributing towards the cnt were temp, weather_lightrain, yr, season_winter and windspeed. Among these variables, weather_lightrain and windspeed have negetive coffecients. It signifies that decrease in these variables will lead to increase on total rentals.
- Weather_cloudy is the least significant variable in terms of contribution towards the Total bikes Rented. So in cloudy weather conditions, company can reduce the number of bikes available. 
- Temperature have significant impact on Total Bike rentals. USA being a colder country, people prefer higher temperature for renting a bike. Targeting days with higher temperatures. Bikes should be available in abundance on these days.
- Model does not include anything about clear weather and other weather variables are negatively affecting. Therefore, removing these variables from the equation will give the equation for weather_clear. It signifies that if we remove these variables, it will positively effect the Total rentals.
- Similarly, season_winter and season_summer have high impact on the Total Rentals. Therefore, these seasons should be targeted to have positive impact on Total Rentals.
- Windspeed is a significant factor but have negative impact on Total rentals.
- mnth_september covers the fall season and it also contributing towards the Total Rentals.
