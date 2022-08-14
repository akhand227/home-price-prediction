### Predicting Home Prices Regression 

### Problem Statement
How can we predict the future sale price of homes, given its characteristics and previous examples of how much similar homes have been sold for?

With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this dataset is used to predict the final price of each home.

### Data 
Data has been collected from <a href="https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview">here </a>.

### Evaluation
Trained on the RandomForestRegressor, data was evaluated using the Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the logarithm of the observed sales price. (Taking logs means that errors in predicting expensive houses and cheap houses will affect the result equally.)

**After training the RandomForestRegressor model following was performed:
 - Hypyterparameter tuning
 - Feature importance
 - Mean Absolute Error
 - RMSE

For evaluation check:  Predicting-Homes-Sales-Price---Regression.ipynb 

### Data Features
Kaggle (author of the dataset) has provided data dictionary detailing all of the features of the dataset. To view click <a href="https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data">here</a>. 

### Used Libraries and Pre-Defined Metrics/Models
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import sklearn 
from sklearn.ensemble import RandomForestRegressor
 ```
 ### Conclusion
 RandomForestRegressor post-training showed a scored of 0.0139 RMSE with the following bestparameters: 
 ```
 {'n_estimators': 10,
 'min_samples_split': 16,
 'min_samples_leaf': 3,
 'max_features': 'sqrt',
 'max_depth': 10}
 ```
 
 

