# Predict the Segment - Hotstar  
link to the competition: https://www.hackerearth.com/challenge/competitive/machine-learning-indiahacks-2017/machine-learning/predict-the-segment-hotstar/  
Tools Used: Jupyter Notebook, python2.  
Library Used: numpy, pandas, matplotlib, seaborn, sklearn, xgboost.  

Preprocessing: Same as given in the demoscript with slight changes.
1. Performed One-Hot Encoding

Final Model Used:
## XGBoost
xgb_params={
    'eta':0.05,  
    'max_depth':5,  
    'colsample_bytree':1.0,  
    'colsample_bylevel':0.3,  
    'subsample':0.6,  
    'objective':'binary:logistic',  
    'eval_metric':'auc',  
    'min_child_weight':5,  
    'silent':1,  
    'seed':2017,  
    'nthread':4,  
    'gamma':0.4,  
    'lambda':8  
    }
    
    I've tuned these parameters using GridSearchCV.
    
    Final-Score on the leaderboard=0.79840
    Refer Notebook for details.
