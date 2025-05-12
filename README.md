# Multiple Models
This repository contains different strategies for using multiple models, such as Hard Voting, Soft Voting, Voting for Regression, OneVsRest, OneVsOne... .

## Voting
The weighted ensemble approach averages the predictions of several models, adjusting their contribution based on their performance through voting.

### Hard Voting (Classification)
- The voting process selects the class that receives the majority of votes from the involved classifiers.

### Soft Voting (Classification)
- The probabilities of each class from the classifiers are averaged, and the class with the highest average probability is chosen as the final prediction.

### Voting for Regression
- The Voting Regressor in regression averages the continuous values of the model predictions. There is no hard or soft voting like in classification.

## OneVsRest
The approach consists of transforming a multi-class classification problem into several binary classification problems by training a binary classifier for each class. To predict the class of a new instance, the probability or score of each classifier is calculated, and the class with the highest score is selected as the prediction.

## OneVsOne
It divides a multi-class classification into a binary classification problem for each pair of classes. Since the model is trained for each pair of classes, it can better handle class imbalances between different pairs, which can improve accuracy and the handling of minority classes.
