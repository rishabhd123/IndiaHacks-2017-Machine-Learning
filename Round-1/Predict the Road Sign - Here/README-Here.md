# Predict the Road Sign-Here :IndiaHacks-2017-Machine-Learning

link to the competition: https://www.hackerearth.com/challenge/competitive/machine-learning-indiahacks-2017/machine-learning/predict-the-road-sign-1/  
Tools Used: Jupyter Notebook, python2.  
Library Used: numpy, pandas, matplotlib, seaborn, sklearn, xgboost.  

Preprocessing: Same as given in the demoscript with slight changes.  
1. Rotated AngleOfSign.
2. Applied sin/cos function on AngleOfSign to tune params.

Final Model Used: 
## XGBoost
 XGB-params:
    'eta':0.15,  
    'max_depth':4,  
    'colsample_bytree':1.0,  
    'colsample_bylevel':0.6,  
    'subsample' :0.9,  
    'objective':'multi:softprob',  
    'eval_metric':'mlogloss',  
    'min_child_weight':4,  
    'silent':1,  
    'seed':2017,  
    'nthread':4,  
    'gamma' : 0.2,  
    'num_class':4,'lambda':7  
    I've tuned these parameters using GridSearchCV.  
    
Final-Score on Leaderboard=99.90110

Refer Notebook for more details.
