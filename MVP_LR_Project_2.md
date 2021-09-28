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

To start exploring this goal, I used a pair plot to view a subset of the features that have numeric values: domestic gross, international gross, budget and runtime.  The pair plot will be used to look for colinearity or multicolinearity.  

![image](https://github.com/CMCGowan1/NBM_Regression_Project_2/blob/main/Screen%20Shot%202021-09-28%20at%201.45.38%20PM.png)

This subset of data was fitted and scored using a linear regression model with data segmented into train/validation split 80/20.

Validation R^2 score on four numeric value features is: 0.9891240911033221

Feature coefficient results: 
  - domestic_total_gross : 1.00
  - international_total_gross : 0.99
  - runtime_(mins) : 15500.42
  - budget : 0.07

The R^2 score for the model is extreamly high suggesting colinearity.  Additional feature engineering will be done on genre, brand and franchise through the use of dummies.  Earliest releasea date may also factor into the model to assess the effects of seasonality on the model.  

This initial analysis suggests that budget may have a significant positive impact on a film's revenue. However, the magnitude of the model's residuals makes it clear that budget is not the only important factor in determining the success of a film.
