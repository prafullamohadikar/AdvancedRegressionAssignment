# Advanced Regression - House Price Predictions
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know the following things about the prospective properties:
- Which variables are significant in predicting the price of a house.
- How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
- What is the background of your project?
- What is the business probem that your project is trying to solve?
- What is the dataset that is being used?

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Conclusion 1
    - Ridge Regression
        - Optimal value of alpha for Ridge Regression = 10
            R-Squared (Train) = 0.94
            R-Squared (Test) = 0.91
            RSS (Train) = 8.29
            RSS (Test) = 3.19
            MSE (Train) = 0.01
            MSE (Test) = 0.01
            RMSE (Train) = 0.08
            RMSE (Test) = 0.10
    - Lasso Ridge
        - Optimal value of alpha for Lasso Regression = 0.001
            R-Squared (Train) = 0.92
            R-Squared (Test) = 0.91
            RSS (Train) = 10.94
            RSS (Test) = 3.31
            MSE (Train) = 0.01
            MSE (Test) = 0.01
            RMSE (Train) = 0.10
            RMSE (Test) = 0.11

- Conclusion 2
    - The below vairables are significant in predicting the price of a house:
        Neighborhood_Crawfor, GrLivArea, OverallQual_9, OverallQual_8, Functional_Typ, YearBuilt, TotalBsmtSF Exterior1st_BrkFace, OverallCond_9, OverallQual_7, MSZoning_FV, Condition1_Norm
    - The variables affect the House prices in below manner:
        Increase of 1 square foot in GrLivArea will increase the price of house by 1.08 to 1.11 times
        Based on OverallQual_9 and OverallQual_8 the house price will increase by 1.08 to 1.14
        Neighborhood_Crawfor in nearby location will increase the price by 1.09 to 1.11
        The house price will increase by 1.06 times based on Functional_Typ
        Because of variable Exterior1st_BrkFace saying exterior brick facing will increase price by 1.05 to 1.06

- Conclusion 3
    Double the alpha for Ridge(20) and Lasso(0.002)
    - Ridge:
        R-Squared (Train) = 0.94
        R-Squared (Test) = 0.91
        RSS (Train) = 9.12
        RSS (Test) = 3.19
        MSE (Train) = 0.01
        MSE (Test) = 0.01
        RMSE (Train) = 0.09
        RMSE (Test) = 0.10
    - Lasso:
        R-Squared (Train) = 0.91
        R-Squared (Test) = 0.89
        RSS (Train) = 13.18
        RSS (Test) = 3.91
        MSE (Train) = 0.01
        MSE (Test) = 0.01
        RMSE (Train) = 0.11
        RMSE (Test) = 0.12

    - Changes in Ridge Regression metrics:
        R2 score of train set remained same at 0.94
        R2 score of test set remained same at 0.94
    - Changes in Lasso Regression metrics:
        R2 score of train set decreased from 0.92 to 0.91
        R2 score of test set decreased from 0.91 to 0.89
    
    Top predictor Variables:
        GrLivArea, OverallQual_8, OverallQual_9, Neighborhood_Crawfor, Functional_Typ, TotalBsmtSF, Exterior1st_BrkFace, YearBuilt

- Conclusion 4
    - Top 5 predictors after dropping top 5 variables:
        2ndFlrSF, 1stFlrSF, TotalBsmtSF, Exterior1st_BrkFace, Neighborhood_Somerst

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- pandas library - version 1.5.3
- numpy - version 1.24.3
- seaborn library - version 0.12.2
- matplotlib library - version 3.7.1
- plotly library - version 5.9.0
- sklearn library - version 1.2.2
- statsmodel library - version 0.13.5

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by Upgrad's Advanced Regression Assignment


## Contact
Created by Prafulla P. Mohadikar [prafulla.mohadikar@gmail.com] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->