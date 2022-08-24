## House prices prediction - [Machine learning competition on Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) - Top 1% 
#### Thanks for visiting my work. I have tried to explain the steps in detail wherever posible. Please do not hesitate to contact me if you have any questions. I'll try my best to follow up. You can also find this notebook on [Kaggle](https://www.kaggle.com/code/muntasirphy/house-prices-top-1/notebook?scriptVersionId=103817570). This notebook was partly inspired by the Feature Engineering for House Prices notebook from instructors Ryan Holbrook and Alexis Cook in their [Feature Engineering](https://www.kaggle.com/learn/feature-engineering) course for machine learning.  

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
* Create Features with Pandas
* Additional Features from Principal Component Analysis (PCA)
![plot6](https://user-images.githubusercontent.com/29087240/186299153-a48d45ed-d919-49b3-9bf7-28e4cdc626c4.png)
![plot7](https://user-images.githubusercontent.com/29087240/186299173-d5134e9b-5149-447f-8d7b-763b87cde13d.png)
![plot8](https://user-images.githubusercontent.com/29087240/186299188-3c760c0c-b413-46ce-ba5c-c91902d99f4a.png)
### D. Combine different models for improved prediction
* Hyperparameter Tuning
* XGB Regressor
* Gradient Boosting Regressor
* Ridge Regressor
* ElasticNet Regressor
* Compare the score of the different models
* Fit each model to full training data
* Define combined models for prediction
* Make predictions and create submissions
### Prediction Accuracy
* Combined model scored an RMSLE of 0.11405 (< Top 1% on Leaderboard)
