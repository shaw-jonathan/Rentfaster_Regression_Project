# Rentfaster_Regression_Project
The purpose of this notebook is to develop a regression model that will accurately predict the price the of rental properties across Canada.
Links used: https://www.kaggle.com/datasets/sergiygavrylov/25000-canadian-rental-housing-market-june-2024
https://www.rentfaster.ca/

## Data and Feature Engineering:
Data was cleaned and prepared by removing unnecessary columns, condensing data, and removing non-applicable data.
Several columns were encoded using OneHotEndocer and the “city” column was encoded with LabelEncoder due to the quantity of cities.

## Models:
Two Linear Regression were made, with one only using selected features resulting in MAE:  402.32 and R2:  0.50. A polynomial Regression model did not produce viable results. A Lasso Cross Validation model resulted in MAE:  378.39 and R2:  0.65.

## Predictions: 
The Linear Regression model with selected features was used as the final prediction model and successfully predicted a rental unit at $1566.49 when the actual listing was $1349 resulting in a $217.49 difference.
