# Credit_Risk_Analysis

### Overview Of The Analysis:

In this week's project we will apply machine learning algorithms to solve a credit card risk problem. This kind of problem is called imbalanced problem because there are much more credit cards with a low risk of credit compared with the ones with high risk. Therefore, we are going to use imbalanced-learn and scikit-learn libraries to build and evaluate classification models and sampling algorithms.

#### Resampling Models to Predict Credit Risk

An imbalanced dataset is a dataset where each output class is represented by different number of input samples. In these cases is necessary to make a process for balancing the number of samples before classifying the dataset. Here, we are going to test four sampling models: Two oversampling methods: RandomOverSampler and SMOTE, one undersampling method: ClusterCentroids, and SMOTEENN that is a mixture between overversampling and undersampling.

The sampling and classification code in Python are shown here and the comparison between the sampling models is performed based on three classification metrics: Accuracy, Confusion Matrix and Precision/Recall rates. For all four cases, the same classifier: Logistic Regression is used.

Because our interest is to compare how different classification methods perform at identifying high risk credit cards, we are going to focuse on Precision and Recall rates for the high risk class.

#### Oversampling Algorithm: Random Oversampler:


<img width="1102" alt="Screen Shot 2022-04-28 at 11 44 00 AM" src="https://user-images.githubusercontent.com/95304774/165791743-7c504869-de3a-479a-b3bc-a920c80f0d92.png">

* Balance Accuracy: 77%
* Precision: 0.99
* Recall: 0.92

#### Oversampling Algorithm: SMOTE Algorithm:

<img width="1083" alt="Screen Shot 2022-04-28 at 2 32 29 PM" src="https://user-images.githubusercontent.com/95304774/165822552-8e504f3d-45f7-4a67-8cdc-5f8064afeae4.png">

* Balance Accuracy: 79%
* Precision: 0.99
* Recall: 0.88

#### Undersampling Algorithm: Cluster Centroids:

<img width="806" alt="Screen Shot 2022-04-29 at 1 48 25 PM" src="https://user-images.githubusercontent.com/95304774/165996602-e295acb7-5203-4c3a-8e9b-0f0a508c3c75.png">

* Balance Accuracy: 77%
* Precision: 0.99
* Recall: 0.77

#### Over and Under sampling Algorithm: SMOTEENN:

<img width="806" alt="Screen Shot 2022-04-29 at 1 51 55 PM" src="https://user-images.githubusercontent.com/95304774/165997151-54d1093e-d8a4-42db-9727-b41049b1c8fc.png">

* Balance Accuracy: 79%
* Precision: 0.99
* Recall: 0.88

### Ensemble Classifiers to Predict Credit Risk

In addition to the sampling and classification approach, we test two ensemble classifiers that resample the dataset and classify the dataset. As the previous four cases, we calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report. The code can be found in here.

#### Balance Random Forest Classifier:

<img width="806" alt="Screen Shot 2022-05-02 at 2 20 36 PM" src="https://user-images.githubusercontent.com/95304774/166303170-92e0165a-385b-4a6d-a8b5-038070145cda.png">

* Balance Accuracy: 77%
* Precision: 0.99
* Recall: 0.92

#### Easy Ensemble Classifier:

<img width="806" alt="Screen Shot 2022-05-02 at 2 24 57 PM" src="https://user-images.githubusercontent.com/95304774/166303678-9a58f274-3085-40f5-b473-5977c592ef29.png">

* Balance Accuracy: 93%
* Precision: 0.99
* Recall: 0.94








