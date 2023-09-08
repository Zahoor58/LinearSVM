# Linear SVM - Email Spam Classifier

## Introduction

This case study focuses on building a linear Support Vector Machine (SVM) classifier to distinguish between spam and non-spam (ham) emails. The dataset, obtained from the UCI Machine Learning Repository, comprises approximately 4600 emails labeled as either 'spam' or 'ham'. 

The dataset can be downloaded [here](https://archive.ics.uci.edu/ml/datasets/spambase).

## Data Understanding

To begin, we load and explore the dataset. The columns are initially labeled as integers, which are then renamed based on the attributes provided by the UCI website [here](https://archive.ics.uci.edu/ml/machine-learning-databases/spambase/spambase.names).

## Data Preparation

The preliminary data preparation steps include rescaling the variables and splitting the data into training and testing sets. Rescaling is performed to standardize the features, ensuring that each column has a mean of zero and a standard deviation of one. The dataset is then split into features (X) and labels (Y) for further processing.

## Model Building

A linear SVM model is constructed using the `SVC()` class from the scikit-learn library. The model is trained on the training data and evaluated using metrics such as accuracy, precision, recall, and specificity. The results are presented, providing insights into the model's performance.

## Interpretation of Results

The interpretation section provides a detailed analysis of the model's performance based on the confusion matrix and various metrics, including accuracy, precision, recall, and specificity. These metrics offer valuable insights into the model's ability to classify emails correctly.

## Hyperparameter Tuning

The case study explores hyperparameter tuning using K-Fold Cross Validation and Grid Search. K-Fold Cross Validation is employed to obtain average metrics over multiple folds, offering a reliable indication of the model's performance. Grid Search is utilized to find the optimal value of the hyperparameter 'C' for the SVM model.

## Optimising for Other Evaluation Metrics

The section discusses the importance of choosing the right evaluation metric based on specific objectives. It demonstrates how different evaluation metrics (accuracy, precision, recall) can lead to variations in the optimal hyperparameter value. This emphasizes the significance of aligning model tuning with the desired outcome.

## Conclusion

In conclusion, this case study provides a comprehensive overview of building a linear SVM classifier for email spam classification. It covers data understanding, data preparation, model building, hyperparameter tuning, and the optimization of evaluation metrics. The insights gained from this study can be applied to similar classification tasks.
