# Chess Data Analysis and Predictive Models

In this project the aim was to analyse the data from chess games and get useful insights. Moreover, building predictive models to answer following three questions:

1. Is it possible to determine the winner (White or Black) using the existing data?
2. Is it possible to predict how the game will end (Draw, Checkmate, Resign, Timeout) using the existing data?
3. Is it possible to determine which opening move has the highest winning probability for white?

In this projecy, all the analysis and models were built using R codes. Therefore, all documents are in R Markdown and HTML format. 

## 1. Dataset
The dataset is from Kaggle with an open license. [Data Source](https://www.kaggle.com/code/zingo3245/chess-dataset-with-eda-and-logistic-regression/data)

## 2. Methodology and Models
Following models were fitted and compared together with all assumption checks.

For Question 1:

* Recursive Partioning and Regression Tree (RPART)
* Logistic Regression
* Linear Discriminant Analysis (LDA)
* Quadratic Discriminant Analysis (QDA)

For Question 2:

* Recursive Partioning and Regression Tree (RPART)
* Multinomial Regression
* Linear Discriminant Analysis (LDA)
* Quadratic Discriminant Analysis (QDA)

For Question 3:

* Logistics Regression

To deal with categorical variables containing too much unique categories, Weigth of Evidence (WOE) transformations were made to avoid increasing the dataset dimensions. 

Also model performaces were not only checked with the Accuracy (from the Confusion Matrix) but also Receiver Operating Characteristic (ROC) curves and Area Under the Curve (AUC) calculations. 