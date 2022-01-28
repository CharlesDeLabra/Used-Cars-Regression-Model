# Used-Cars-Regression-Model
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/cars4u.png?raw=true" alt="Logo" width=72 height=72>
  <h3 align="center">Used Cars Regression Model</h3>
  <p align="center">
    This project solved a prediction problem for Cars4U to predict price of used cars based on their features. It was trained different models for finding a better solution for solving the problem.
    <br>
  </p>
</p>

## Table of contents

- [Context](#context)
- [Problem Statement](#problem-statement)
- [Code](#code)
- [Status](#status)
- [Analysis](#analysis)
- [Conclusions](#conclusions)
- [Recomendations](#recomendations)

## Context

There is a huge demand for used cars in the Indian Market today. As sales of new cars have slowed down in the recent past, the pre-owned car market has continued to grow over the past few years and is now larger than the new car market. Cars4U is a budding tech start-up that aims to find footholes in this market. Unlike new cars, where price and supply are fairly deterministic and managed by OEMs (Original Equipment Manufacturer / except for dealership level discounts which come into play only in the last stage of the customer journey), the used car market is a very different beast, with large uncertainties in both pricing and supply. Several factors, including mileage, brand, model, year, etc. can influence the actual worth of a car. From the perspective of a seller, it is not an easy task to set the correct price of a used car. Keeping this in mind, the pricing scheme of these used cars becomes important in order to grow in the market. 


## Problem Statement

It is needed to develop a price prediction model in order to be able to predict used cars prices based on the features of each cars. It is provided a dataset with features of each cars such as; Mileage, Brand, Mode, Power, Engine, Type of Owner, etc. The task is to analize the data and come with different regresion solution in order to find which model fits best to data and that will mean that is a better predictor.


## Code

The program was written on Jupyter Notebooks in Python Language. You can access to the code [here](https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/Regression_Code.ipynb)

## Status

The code is finished and have been evaluated, the goal was partially completed since the models were good enough to predict non-luxury cars but they lack data in order to predict luxury brands.

## Analysis


First it is needed to understand the dataset, so this summary was presented:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data.JPG" alt="Data" width=1000 height=353> 
</p>
<br>
Here we can notice that dataset contains lots of features of cars and numerical or categorical variables. Also there are missing values so this will need to be treated.

After processing data and handling missing values a new dataset can be showed which will be used for training models. The next dataset is:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data2.JPG" alt="Data1" width=1000 height=353> 
</p>
<br>

Then it was trained different models for the separate dataset and the best result were the decision tree and the random forest. The Results for the decision tree for non-luxury cars were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data3.JPG" alt="Data2" width=500 height=350> 
</p>
<br>
The Results for the decision tree for luxury cars were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data4.JPG" alt="Data3" width=500 height=350> 
</p>
<br>

The Results for the Random Forest for non-luxury cars were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data5.JPG" alt="Data4" width=500 height=350> 
</p>
<br>
The Results for the Random Forest for luxury cars were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data6.JPG" alt="Data5" width=500 height=350> 
</p>
<br>

After seeing this results it was decided to train a model for complete dataset and see how it improve the results for decision tree it obtained the next results;
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data7.JPG" alt="Data" width=500 height=350> 
</p>
<br>
For Random Forest it was obtained the next ones:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data8.JPG" alt="Data6" width=500 height=350z>
</p>
<br>
It was decided that Random Forest was the best ones so it was decided to test for both of the type of cars and the results for non-luxury cars were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data9.JPG" alt="Data7" width=500 height=350> 
</p>
<br>
The results for luxury cars were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data10.JPG" alt="Data8" width=500 height=350> 
</p>
<br>
At the end it was decided to use Lasso Model for luxury cars and Random Forest for non-luxury cars. Finally it was plotted the differences in percentage between real and predicted, For Random Forest the positive difference were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data11.JPG" alt="Data9" width=600 height=650> 
</p>
<br>
And the negative differences were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data12.JPG" alt="Data10" width=600 height=650> 
</p>
<br>
For Lasso Regression the positive difference were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data13.JPG" alt="Data11" width=600 height=650> 
</p>
<br>
And the negative differences were:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Used-Cars-Regression-Model/blob/main/imagen/data14.JPG" alt="Data12" width=600 height=650> 
</p>
<br>

## Conclusions

- The training made with the complete dataset were good on non-luxury brands since the dataset contains more of this data
- Simpler models were good with luxury cars
- Random forest were the best model with complete dataset
- All of the three simple model were equally good
- Power, Mileage, Brands, Owner and Kilometers were the most important features
- Tuning improved our results, specially RMSE
- It was needed to fill some missing data in order to have better features
- Skew data were removed with natural logaritm

## Recomendations

- It is needed to obtain more data about luxury cars
- Use the model for luxury cars only as a guide since the results could be better
- Since model of non-luxury cars had more than 90% of R-squared it is good to predict prices 
- Use Lasso model for luxury cars and Random Forest for non-luxury cars



