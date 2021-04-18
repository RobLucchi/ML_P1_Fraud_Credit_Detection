# Credit Card Fraud Analysis
### By Ahmed Alaa Mousa


* [Dataset](#dataset)
* [SVM Model Predictions](#model-predictions)
* [Keras DL Model Predictions](#keras-dl-model-predictions)

## Dataset

### Context
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

### Content
The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

### Ref: https://www.kaggle.com/mlg-ulb/creditcardfraud

### Methods Used
* Data Wrangling
* Data Preprocessing
* Feature engineering
* Imbalanced Data methods
  - Class weights
  - SMOTE
* Machine Learning (Support Vector Machine)
* Deep Learning (keras)
* Metric Visualization 
  - ROC
  - Confusion Matrix
* etc.

### Technologies
* Python
* Pandas, , Numpy
* Matplotlib, Seaborn, plotnine
* jupyter
* sklearn, Imblearn, keras
* etc. 

<hr>

## SVM Model Predictions

Confusion matrix

	[[55476  1175]
	 [   15    80]]

- f1       : 0.11851851851851852
- recall   : 0.8421052631578947
- precision: 0.06374501992031872
- roc auc  : 0.906650042875631

## Keras DL Model Predictions

Confusion matrix

	[[56626    25]
	 [   13    82]]

f1       : 0.8118811881188119
recall   : 0.8631578947368421
precision: 0.7663551401869159
roc auc  : 0.9650526910381105
