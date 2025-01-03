#Titanic Survival Prediction Model
This repository contains the implementation of a machine learning model for predicting the survival of passengers on the Titanic. The model uses various machine learning algorithms to achieve accurate predictions based on the dataset provided by the Kaggle Titanic competition.

#Data Preprocessing
The Preprocess function combines the training and test datasets and performs several preprocessing steps:

Drops irrelevant columns ('Name' and 'Ticket').

Fills missing values in the 'Age' column with the mean age.

Fills missing values in the 'Cabin' column with 'X000'.

Fills missing values in the 'Embarked' column with 'X'.

Fills missing values in the 'Fare' column with the mean fare.

Extracts cabin letters and numbers into separate columns.

Converts categorical columns ('cabin_letter', 'Embarked', 'Sex') into dummy variables.

Drops unnecessary dummy variables ('cabin_X', 'Embarked_X').

Creates new features ('Pclass_bin_Fare' and 'Pclass_bin_sex').

#Model Training and Evaluation
The code trains and evaluates multiple machine learning models:

Logistic Regression: Trains a logistic regression model and evaluates its accuracy.

XGBoost Classifier: Trains an XGBoost classifier and evaluates its accuracy.

Random Forest Classifier: Trains a random forest classifier and evaluates its accuracy.

The accuracy of each model is printed for comparison.

#Prediction on Test Data
The best-performing model (Random Forest Classifier) is used to make predictions on the test dataset. The predictions are saved to an output CSV file (output.csv) with the following columns:

PassengerId: ID of the passenger.

Survived: Predicted survival (0 or 1).

#Cloning the repository
git clone https://github.com/yourusername/Titanic-Survival-Prediction.git
cd Titanic-Survival-Prediction
