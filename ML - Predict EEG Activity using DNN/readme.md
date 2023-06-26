# Performance Evaluation of Deep Neural Networks for EEG Activity Prediction in Epileptic Patients

### Introduction
The data_epileptic.RData file contains data related to electroencephalography (EEG) measurements of patients with epilepsy and healthy subjects. 
This report focused on the analysis and comparison of two deep neural networks in predicting the type of condition and brain area associated with EEG signals. 
The neural networks were trained, validated, and tested using the provided data matrices. The evaluation of their performances, including the impact of an additional hidden layer, provides insights into the effectiveness of each network. The best-performing network in terms of accuracy for predicting EEG signals of patients with tumor formations is identified, backed by a rationale based on the evaluation results. 
These findings contribute to understanding the suitability of deep neural networks for EEG activity prediction in patients with epilepsy.

#### Dataset Description
The dataset comprises categorical variables indicating various EEG activities related to different subjects, conditions, and brain areas. The target variable has the following categories:

1: Epileptic seizure activity

2: Patient with tumor formation, EEG activity recorded on a healthy area during an epilepsy-free interval

3: Patient with tumor formation, EEG activity recorded on the tumor location area during an epilepsy-free interval

4: EEG activity of a healthy subject with eyes closed

5: EEG activity of a healthy subject with eyes open

The dataset includes data matrices (x, y, x_test, and y_test). Matrices x and y are used for model training and validation, while matrices x_test and y_test are utilized for testing purposes. The matrices denoted with "x" represent the input data, whereas those denoted with "y" contain the target class labels.

#### Neural Network Comparison
To predict the type of condition and brain area associated with EEG signals, two deep neural networks are deployed: one with 2 hidden layers and another with 3 hidden layers. The following steps are performed to compare their performances:

a. Train and validate both neural networks using the data matrices x and y.

b. Assess the predictive performance of each network using appropriate evaluation metrics.

c. Compare the performance of the two networks in terms of accuracy, precision, recall, and F1-score.

#### Impact of Additional Hidden Layer
To evaluate the impact of adding an extra hidden layer to the network architecture, the performances of the two neural networks are analyzed. The improvement in predictive performance is discussed briefly, considering metrics such as accuracy and other relevant evaluation measures.

#### Test Accuracy and Performance Evaluation
The test accuracy of the two deep neural networks is evaluated using the data matrices x_test and y_test. The performance of each network in predicting EEG signals of patients with tumor formations is assessed. A brief commentary is provided, highlighting the network that achieves the best accuracy on the test data. The reasoning behind this choice is motivated based on the evaluation results and the network's ability to accurately predict EEG signals associated with tumor formations.
