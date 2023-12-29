# Breast_Cancer_Prediction



Used classification technique on the Breast Cancer dataset. 

Data: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data

Description: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names

Specifically, build a decision tree, logistic regression and k-nearest neighbors, Support vector machine that predicts the diagnose
result based on ten real-valued features (mean, standard error, and "worst" or largest of these features).
Explore how well different model perform for several different parameter values. 

This solution tried to detect when is overfitting and when is underfitting in order to optimize the best predictive performance. 
In addition to manually review for hyperparameter optimization, I also applied nested cross-validation with multiple hyper parameter in the grid search aiming at maximizing the usage of different sub-dataset in training data, which may also reduce possibility of overfitting.

<img width="829" alt="Screenshot 2023-12-12 at 09 20 35" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/7422ed4f-7515-4caa-93b1-c93a298f870d">


