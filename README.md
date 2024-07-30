# Bike Sharing 
> Bike Sharing Project details: BoomBikes, a US bike-sharing provider, is struggling with reduced revenues due to the COVID-19 pandemic and >seeks to develop a business plan to boost revenue post-pandemic. To prepare for a surge in demand once the lockdown ends, BoomBikes wants >to analyze factors influencing bike demand in the American market. They have hired a consulting company to determine:

> * Significant variables predicting bike demand.
> * How well these variables explain bike demand.

>The company has collected a large dataset on daily bike usage, incorporating various factors from meteorological surveys and consumer >behaviors. This analysis aims to optimize BoomBikes' strategy and stand out in the competitive market once the economy recovers.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Project Information
- This project is a data science project. It uses Bike data set to predict whether a user will register for bike sharing or not.
### Project Background
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 

<img width="452" alt="image" src="https://github.com/user-attachments/assets/9560d424-9482-4eb7-8ceb-fd2171e14cd2">
<img width="452" alt="image" src="https://github.com/user-attachments/assets/32d1bf00-8bd3-4f41-8c7e-4cfd91c17dfd">

### Business Problem to solve
-  To model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 
  
### Project dataset
- The dataset is a csv file with name: day.csv. It is added in the repo.


## Conclusions
- By using the above scatter plot and the table , We can see that the equation of our best fitted line is:

  cnt = 0.488858 × temp + 0.237253 × yr + 0.121488 × season_Winter + 0.107894 x mnth_Sep + 0.098906 × weathersit_Mixed clouds + 0.097239 ×     season_Summer + 0.061845 × weekday_Sutarday + 0.055781 x mnth_Aug + 0.051308 × workingday - 0.017070 - 0.037014 x mnth_Jan − 0.180140 ×      windspeed

- All the positive coefficients like temp,season_Summer indicate that an increase in these values will lead to an increase in the value of cnt. All the negative coefficients indicate that an increase in these values will lead to a decrease in the value of cnt.
- From R-Sqaured and adj R-Sqaured value of both train and test dataset we could conclude that the above variables can well explain more than 0.78% of bike demand.
- Coeffiencients of the variables explains the factors effecting the bike demand
- Based on final model top three features contributing significantly towards explaining the demand are:
* Temperature (0.488858)
* windspeed : (-0.180140)
* year (0.237253)

- Hence, it can be clearly concluded that the variables temperature , windspeed and month are significant in predicting the demand for shared bikes .

<img width="340" alt="image" src="https://github.com/user-attachments/assets/82a30430-3f76-4126-ae52-91f3531669dd">
<img width="377" alt="image" src="https://github.com/user-attachments/assets/b5edcdf4-6f49-4edc-bb09-2e5e9238af29">

### Driving factors which can be used to predict about chances of loan default are:
- temp
- yr
- season_Winter
- mnth_Sep
- weathersit_Mixed clouds
- season_Summer
- weekday_Sutarday
- mnth_Aug
- workingday
- mnth_Jan
- windspeed
  
## Technologies Used
- Numpy - version '1.23.5'
- Pandas - version '1.5.3'
- Seaborn - version '0.12.2'
- Matplotlib - version '3.7.1'
- sklearn - '1.3.0'
- statsmodels - '0.14.0'

## Acknowledgements
- This project was inspired by UpGrad(IIITB) in AI/ML Executive Post Graduate course as a case study
- This project was based on linear regression: ([https://learn.upgrad.com/course/5800/segment/50366/308501/935805/4670514](https://learn.upgrad.com/course/5800/segment/52631/312288/946785/4724968)).

## Contact
Created by [@RavishankarDuMCA10] - feel free to contact me!
