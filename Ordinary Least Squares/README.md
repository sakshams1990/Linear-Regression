# Car Price Prediction

**Problem Statement**
A Chinese automobile company Geely Auto aspires to enter the US market by setting up their manufacturing unit there and producing cars locally to give competition to their US and European counterparts.

They have contracted an automobile consulting company to understand the factors on which the pricing of cars depends. Specifically, they want to understand the factors affecting the pricing of cars in the American market, since those may be very different from the Chinese market. The company wants to know:

1. Which variables are significant in predicting the price of a car
2. How well those variables describe the price of a car

**Business Problem**
You are required to model the price of cars with the available independent variables. It will be used by the management to understand how exactly the prices vary with the independent variables. They can accordingly manipulate the design of the cars, the business strategy etc. to meet certain price levels. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

**Dataset** can be found from the link below - 

https://www.kaggle.com/sakshams1990/carprice

**Data Cleaning**

There were a few car names that were misplelt and were rectified with correct car names.

**Data Visualisation**

Using Matplotlib and Seaborn , each of the numerical independent variable was plotted as scatter plot vs Price field.

Based on the scatter plot, we could identify the columns that have correlation with the Price column.

**Feature Engineering**

The categorical variables were converted into numerical using get_dummies.

**Model Building**

1. The  model was developed using Ordinary Least Squares (OLS).

2. Recursive Feature Elimination was used to identify the top 10 features.

3. From the top 10 features, the features were dropped having p-value greater than 0.05 and VIF greater than 5.

**Inference**
1. R2 score for Actual vs Prediction is 85%.

2. The features horsepower, four,rwd,dohcv,rotor & Luxury determined the car price.

3. The final equation is **price = 0.3857horsepower - 0.1060four + 0.1285rwd - 0.2791dohcv -0.1567rotor + 0.3434Luxury**
