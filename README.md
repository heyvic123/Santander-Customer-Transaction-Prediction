Santander Customer Transaction Prediction

This is a Kaggle competition to predict the probability of event of the target, which would be evaluated by area under the ROC curve.

Dataset given is a masked data, with 200 unknown numerical variables and total records of 200K lines of records. The result of the event is imbalanced.

1. Sklearn models

    ##### Gradient Boosting 
    ##### Random Forest 
    ##### BernoulliNB 
    ##### GaussianNB
    ##### LogisticRegression
    ##### XGBClassifier 


   ####  Gaussian NB obtained the best result among the above models. AUC 0.887


2. Light GBM 

    Result of the fitting

    Early stopping, best iteration is:
    [10153]	valid_0's l2: 0.131712	valid_0's auc: 0.8947
    Starting predicting...
    The rmse of prediction is: 0.3629216599181957

    #### AUC:  0.8946998836662459


3. Light GBM added with 10 interaction terms (The best result so far) 

    Result of the fitting

    Early stopping, best iteration is:
    [5982]	valid_0's l2: 0.127459	valid_0's auc: 0.900184
    Starting predicting...
    The rmse of prediction is: 0.35701375549931996
    
    #### AUC:  0.9001844143709659
