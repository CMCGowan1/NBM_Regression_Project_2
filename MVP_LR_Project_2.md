# Analysis of Box Office Revenue for the Worldwide Film Industry

The goal of this project is to better understand which features affect box office revenue.  Features in this data set include: 
- movie title
- domestic gross
- international gross
- budget
- runtime in minutes
- genre
- brand
- franchise
- earliest release date

The Target is:
- worldwide gross

The data was cleaned of duplicates and NaN values.

To start exploring this goal, I used a pair plot to view a subset of the features that have numeric values: domestic gross, international gross, budget and runtime.  The pair plot will be used to look for colinearity or multicolinearity.  

![image](https://github.com/CMCGowan1/NBM_Regression_Project_2/blob/main/Screen%20Shot%202021-09-28%20at%201.45.38%20PM.png)

This subset of data was fitted and scored using a linear regression model with data segmented into train/validation split 80/20.

Validation R^2 score on four numeric value features is: 0.9891240911033221

Feature coefficient results: 
  - domestic_total_gross : 1.00
  - international_total_gross : 0.99
  - runtime_(mins) : 15500.42
  - budget : 0.07

The R^2 score for the models numerical values is extreamly high suggesting colinearity.  

The next step will be to split the data into train, validation and test segments.  Feature engineering will then be done on genre, brand and franchise through the use of dummies. Features with multicolinearity or colinearity will be dropped.  Earliest release date may also factor into the model to assess the effects of seasonality on the model depending on time.  

The model will be fit, validated and finalized.  Then the steps will be repeated on the test data and a final score will be computed to see how well the model predictions are. 

Note:  Additional scraping in progress to see if star ranking and cast can be added as features.
