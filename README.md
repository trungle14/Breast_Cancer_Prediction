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


<img width="466" alt="Screenshot 2023-12-28 at 23 03 15" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/a9421e98-9dc9-4d09-8d26-82f624bc35be">

<img width="471" alt="Screenshot 2023-12-28 at 23 03 39" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/4e5ba535-af8b-415f-b53a-a93dd189d1ab">

<img width="458" alt="Screenshot 2023-12-28 at 23 01 48" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/507757f7-2859-47fd-9a6c-0e08abc89cef">

<img width="497" alt="Screenshot 2023-12-28 at 23 02 26" src="https://github.com/trungle14/Breast_Cancer_Prediction/assets/143222481/0a728246-5f43-48be-807b-3fd125e183a2">
