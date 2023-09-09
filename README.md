## Predictive Modelling: Stacking ML model for high prediction accuracy
Stacking is an ensemble machine learning technique in which the outputs of multiple different machine learning models (base models) are fed into a higher-level meta-model to make the final output. Stacking can be useful to improve the overall accuracy of the predictions by utilising the strengths of each individual base model and minimising the effects of overfitting. In this example, a combination of multiple ML models (XGBoost, GBM, Ridge and ElasticNet) is used to develop the stacking model. The Ames housing dataset (machine learning competition on Kaggle) was used to demonstrate the model's capability to predict house prices with high accuracy. To begin with, download the jupyter notebook files (the old ones use a combined ML technique whereas the new one uses a stacking model). You can download the train and test data (csv) files from [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques). Run the notebook step by step to get a thorough understanding. 

### A. Load and Preprocess data
* Imports packages
* Import Data

![plot1](https://user-images.githubusercontent.com/29087240/186298908-e4e74bc9-026e-4b2b-ac0d-ffc87883df2b.png)

* Clean Data
* Statistical data types and missing values
### B. Initial Analysis and Baseline Score
* Visualise the relation between numerical features and Target (SalePrice)

![plot2](https://user-images.githubusercontent.com/29087240/186298661-f23a6ceb-c686-47a3-bb15-5bd516382109.png)

* Root Mean Squared Logaritmic Error (RMSLE)
### C. Feature Engineering
* Mutual Information Score

![plot3](https://user-images.githubusercontent.com/29087240/186299083-5bfe246e-2e1d-45fc-98b1-6e4078671b50.png)

* Interaction Features

![plot4](https://user-images.githubusercontent.com/29087240/186299108-79b82b93-d430-4eee-a8d4-4dcb268022dd.png)
![plot5](https://user-images.githubusercontent.com/29087240/186299128-ae1bc5c3-90c9-4ec7-ac81-a135abdaa810.png)

* Transforming Skewed Features

![image](https://github.com/muntasirhsn/Combined-ML-Models-for-House-Prices-Prediction/assets/29087240/34ee38f5-a8a5-4916-925f-72ca10b3e78b)


* Create Features with Pandas

* Additional Features from Principal Component Analysis (PCA)

![plot6](https://user-images.githubusercontent.com/29087240/186299153-a48d45ed-d919-49b3-9bf7-28e4cdc626c4.png)
![plot7](https://user-images.githubusercontent.com/29087240/186299173-d5134e9b-5149-447f-8d7b-763b87cde13d.png)
![plot8](https://user-images.githubusercontent.com/29087240/186299188-3c760c0c-b413-46ce-ba5c-c91902d99f4a.png)

### D. Stacking Model for improved prediction
* Hyperparameter Tuning
* XGB Regressor
* Gradient Boosting Regressor
* Ridge Regressor
* ElasticNet Regressor
* Stacking Regressor

![image](https://github.com/muntasirhsn/Stacking-ML-Model-for-House-Prices-Prediction/assets/29087240/5739c5aa-f92e-4ee8-baec-c20b473caafc)
  
* Compare the scores of the different models
* Fit stacking model to full training data
* Make predictions

### Prediction Accuracy
* Combined model scored an RMSLE of 0.11365 (< Top 1% on Leaderboard)
