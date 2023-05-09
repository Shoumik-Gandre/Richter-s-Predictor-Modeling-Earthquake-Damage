# Richter's Predictor: Modeling Earthquake Damage [[Link]](https://www.drivendata.org/competitions/57/nepal-earthquake/)
We're trying to predict the ordinal variable damage_grade, which represents a level of damage to the building that was hit by the earthquake.
This is me: [Shoumik](https://www.drivendata.org/users/Shoumik/)

## Feature Extraction [[Notebook]](src/Feature%20Extraction.ipynb)
This answers the following questions:
1. Geo Dimensionality Reduction: How to Use Neural Network Dimensionality Reduction to get dense embeddings out of Geo Level IDs
2. Geo 3 Rollup: How to obtain dense embeddings from Geo Level IDs by treating geo levels as a supervised training problem of predicting geo level IDs 1 and 2 from Geo Level 3 ID as input. 

## XGBoost [[Notebook]](src/XGBoost-Colab.ipynb)
Using [Feature Extraction](src/Feature%20Extraction.ipynb) and Hyperparameter Optimization using Optuna, A well performing XGBoost Model is obtained.  
A Bagging Model is attempted.

## CatBoost [[Notebook]](src/Catboost.ipynb)
Using [Feature Extraction](src/Feature%20Extraction.ipynb) and Hyperparameter Optimization using Optuna, A well performing CatBoost Model is obtained.

## LightGBM [[Notebook]](src/Lightgbm.ipynb)
Using [Feature Extraction](src/Feature%20Extraction.ipynb) and Hyperparameter Optimization using Optuna, A well performing LightGBM Model is obtained.
