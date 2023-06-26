# Analysis of Predictive Models for Matching Individuals in Speed Dating Events

### Introduction
This report presented the analysis of two classifiers, a logistic regression model, and a classification tree, 
for predicting positive matches between users in a speed dating context. The predictive performance of these models was evaluated using the "data_test" 
dataset, and the models were compared based on their ability to correctly identify positive matches. The findings and insights gained from this analysis 
will help guide the development of a machine learning system for the speed dating app, providing valuable information for the company's decision-making process.

#### Dataset Description
The dataset "data_speed_dating.csv" was collected during an experimental social and speed dating event. 
It contains information gathered from the speed dating event, where participants engaged in four-minute "first dates" 
with every other attendee. After each interaction, participants were asked if they would like to see their date again. 
The variable "match" indicates whether both individuals answered "yes" to this question, indicating a positive match. 
In addition to the match variable, participants also rated their date on six dimensions: attractiveness, sincerity, intelligence, 
fun, ambition, and shared interests. They also provided a score on "how much" they liked their date (like) and "how much" they thought their date 
liked them (guess_liked). The dataset also includes information on the age difference between individuals in a date and the gender identity of participants.

#### Logistic Regression Model
To assess the predictive performance, a logistic regression model was fitted using the dataset "data_speed_dating.csv." Logistic regression is a popular method for binary classification problems. In this case, the aim is to predict positive matches between users based on the input variables.

#### Classification Tree
Alongside the logistic regression model, a classification tree was also constructed using the same dataset. Classification trees are decision trees that partition the data based on input variables to classify observations into different groups. This model was built to compare its performance with the logistic regression model.

#### Predictive Performance Evaluation
To evaluate the predictive performance of the two classifiers, the dataset "data_test" was utilized. 
This dataset contains unseen data that was not used during the model training phase. 

The following steps were followed to assess and compare the performance of the classifiers:
- Apply the logistic regression model and the classification tree to the "data_test" dataset.
- Evaluate the models' ability to correctly identify positive matches between users.
- Compare the models based on appropriate evaluation metrics such as accuracy, precision, recall, and F1-score.
- Comment on the performance of the models, focusing on their ability to identify positive matches as it aligns with the company's primary interest.
