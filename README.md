Santander Customer Transaction Prediction

This is a Kaggle competition to predict if the customer would make a transaction. 

Dataset given is a masked data, with 200 unknown numerical variables and total records of 200K lines of records. The result of the event is imbalanced.

#

1. Sklearn models

    ##### Gradient Boosting 
    ##### Random Forest 
    ##### BernoulliNB 
    ##### GaussianNB
    ##### LogisticRegression
    ##### XGBClassifier 


   ####  Gaussian NB obtained the best result among the above models. AUC 0.887

#

3. Light GBM with adjusted parameters and KFold estimator (The best result so far) 

    Result of the fitting:    
    Fold 0
    Early stopping, best iteration is:
    [9699]	training's auc: 0.95072	valid_1's auc: 0.89884
    
    Fold 1
    Early stopping, best iteration is:
    [8865]	training's auc: 0.948158	valid_1's auc: 0.896344
    
    Fold 2
    Early stopping, best iteration is:
    [8881]	training's auc: 0.947751	valid_1's auc: 0.901579
    
    Fold 3
    Early stopping, best iteration is:
    [7308]	training's auc: 0.94172	valid_1's auc: 0.900664
    
    Fold 4
    Early stopping, best iteration is:
    [6458]	training's auc: 0.938254	valid_1's auc: 0.903294

    
#    
    Train AUC:  0.95072  ; Valid AUC: 0.89884
    Submission AUC: 0.900
    
#    
    
2. Light GBM 

    Result of the fitting

    Early stopping, best iteration is:
    [10153]	valid_0's l2: 0.131712	valid_0's auc: 0.8947
    Starting predicting...
    The rmse of prediction is: 0.3629216599181957
#
    train AUC:  0.8946998836662459
#


3. Light GBM added with 10 interaction terms 

    Result of the fitting

    Early stopping, best iteration is:
    [5982]	valid_0's l2: 0.127459	valid_0's auc: 0.900184
    Starting predicting...
    The rmse of prediction is: 0.35701375549931996
#    
    train AUC:  0.9001844143709659
#
