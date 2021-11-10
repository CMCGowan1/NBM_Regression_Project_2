
# Linear Regression Project Write-up
# Predicting Movie Worldwide Total Gross in the Film Industry

## Abstract
The goal of this project was to use a linear regression model to predict what features influence box office success.  The global film market reached a record breaking $100 Billion in 2020 and film producers are interseting in understanding what features influence box office revenue.  Leveraging the use of feature engineering dummy variables to analyze the categorical variables of genre, franchise and brand.  I built a Linear Regression model to assess R^2, heteroskedasticity and to plot residuals in order to interpret data and make predictions.  

## Design
This project originates from movie producers interest in understand what features make a movie successful at the box office.  

## Data
The dataset contains 1990 movies with 10 features. The data was scraped from BoxOfficeMoJo.com using the Python requests library and the HTML was parsed using Beautiful Soup.  During the scaping process there was a large overlap in duplicates which upon cleaning reduced the data set to 884 obesrvations. Due to the large number of movies with only one brand or franchise associated with it the brand and franchise categoires were factored as either yes brand, yes franchise, or no brand, no franchise.  No brand = 625, Yes Brand = 259.  No Franchise = 490, Yes Franchise = 394.  Genre was bucketed into the top 9 genres, with the largest genre having 659 rows.  The target of the analysis is World Wide Total Gross Revenue at the box office. 

## Algorithms
Linear Regression
OLS
R^2
Feature Engineering

## Model Evaluation and Selection

The entire training dataset of 59,400 records was split into 80/20 train vs. holdout, and all scores reported below were calculated with 5-fold cross validation on the training portion only. Predictions on the 20% holdout were limited to the very end, so this split was only used and scores seen just once.

The official metric for DrivenData was classification rate (accuracy); however, class weights were included to improve performance against F1 score and provide a more useful real-world application where classification of the minority class (functional needs repair) would be essential.

Final random forest 5-fold CV scores: 99 features (7 numeric) with class weights

Accuracy 0.797
F1 0.791 micro, 0.679 macro
precision 0.792 micro, 0.722 macro
recall 0.797 micro, 0.658 macro
Holdout

Accuracy: 0.802
F1: 0.795 micro, 0.685 macro
Precision: 0.796 micro, 0.725 macro
Recall: 0.802 micro, 0.664 macro
Tools
Numpy and Pandas for data manipulation
Scikit-learn for modeling
Matplotlib and Seaborn for plotting
Tableau for interactive visualizations
Communication
In addition to the slides and visuals presented, Tanzania Waterpoints (Links to an external site.) will be embedded on my personal website and blog.

Dashboard example with sample statistics

![image](https://user-images.githubusercontent.com/18155025/141036110-9e5915c8-f74a-4363-888b-0c1d8b252cc8.png)

![image](https://user-images.githubusercontent.com/18155025/141036234-5a9a1afb-4e64-4396-ba92-31bf6949deb6.png)

![image](https://user-images.githubusercontent.com/18155025/141036156-cf2a5187-8255-4d03-acd4-638ecf19e440.png)

![image](https://user-images.githubusercontent.com/18155025/141035874-573d4259-d8e2-4517-af0d-4840444b27a4.png)

![image](https://user-images.githubusercontent.com/18155025/141036054-306601b1-bd94-4f8d-90bf-c873c0868319.png)

![image](https://user-images.githubusercontent.com/18155025/141036082-d883992a-2404-46f4-96ac-93480e7c0cac.png)

![image](https://user-images.githubusercontent.com/18155025/141036132-da122a0f-bd49-4be8-9214-ecbd68d4892e.png)




