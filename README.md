# Breast_Cancer_Prediction



The motivation for applying machine learning to breast cancer prediction is multifaceted and significant. Breast cancer is one of the most common cancers worldwide and early detection is crucial for effective treatment and improved patient outcomes. Here are some key motivations:

**Early Detection and Diagnosis:** Machine learning models can assist in the early detection of breast cancer, often identifying malignancies that may be missed by traditional methods. Early diagnosis is crucial as it can significantly increase the chances of successful treatment.

**Enhancing Accuracy:** Machine learning algorithms can process vast amounts of data and recognize complex patterns that might not be apparent to human observers. This can lead to more accurate diagnoses, reducing the rate of false positives and negatives, which are common in traditional diagnostic methods like mammography.

**Personalized Treatment Plans:** Machine learning can help in predicting the most effective treatment plans for individual patients based on their unique genetic makeup and the characteristics of their tumors. This personalized approach can improve treatment efficacy and reduce side effects.

Data: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data

Description: https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names

In this problem, I tried multiple machine learning model such as decision tree, logistic regression and k-nearest neighbors, Support vector machine that predicts the diagnose
result based on ten real-valued features (mean, standard error, and "worst" or largest of these features).
Explore how well different model perform for several different parameter values. 

This solution tried to detect when is overfitting and when is underfitting in order to optimize the best predictive performance. 
In addition to manually review for hyperparameter optimization, I also applied nested cross-validation with multiple hyper parameter in the grid search aiming at maximizing the usage of different sub-dataset in training data, which may also reduce possibility of overfitting.

<img width="829" alt="Screenshot 2023-12-12 at 09 20 35" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/7422ed4f-7515-4caa-93b1-c93a298f870d">



<img width="702" alt="Screenshot 2023-12-28 at 23 10 34" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/132bda0e-e76c-49b5-89f5-a1690d584457">
