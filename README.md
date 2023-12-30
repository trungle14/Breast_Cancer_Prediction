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


**Confusion Matrix**

<img width="702" alt="Screenshot 2023-12-28 at 23 10 34" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/132bda0e-e76c-49b5-89f5-a1690d584457">



**Performance Summary** 


<img width="875" alt="Screenshot 2023-12-30 at 10 20 42" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/cf188bbd-b328-47af-a678-e66381472dcb">




In general, based on the accuracy and F1 score among 4 models, decision tree give us the most optimal predictive model with the performance at 99%  on the test dataset, while the other models achived at around 97%. For the further enhancement, we may consider tuning hyperparameter in SVM, however the problem has been almost resolved quite effectively with a significant hugh accuracy and F1-Score


**Feature Importance** **Decision Tree**

<img width="829" alt="Screenshot 2023-12-12 at 09 20 35" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/7422ed4f-7515-4caa-93b1-c93a298f870d">



**Explorations**
 


In this scenario, a missed diagnosis in breast cancer may cause more serious consequence, a high recall means that there are fewer false negatives. Thus, I would like to use Recall as the main performance matrix, decision tree perform quite well with the Recall > 95% while Recall of Logistic regression and kNN are approximately 92%.

In addition, we also look at the feature importance in Decision tree and coefficient in Logistic regression to see which factors are the most important to the prediction of breast cancer. 
- Apparently, **Worst Radius**,**Worst Concave Point**  appears in the top 5 important factors in the model, which can help medical professionals good implication to predict the patient. 
- Moreover, based on the above decision tree we can easily notice that if **Worst Radius <= 16.79** and **Worst Concave Point <= 0.136** , **SE Radius < 1.048** has more probability to be maglinant
- We are also able to seperate 2 groups of factor  having different effect on breast cancer based on the coeficient of logistic model almost factor show positive relationship the more or higher they are, the more probability of breast cancer maglinant, however, it is opposite to the groups of factor of **Compactness** and **Fractal Dimension**
