# Module17Assignment
Comparing Classifiers for Predicting Term Deposit Subscriptions
Project Overview
This project explores the use of various machine learning classification models to predict whether clients will subscribe to a term deposit based on their characteristics and the results of previous marketing campaigns. The dataset used is from the UCI Machine Learning Repository and contains detailed information on marketing campaigns from a Portuguese bank.

The goal is to compare the performance of four classifiers—k-Nearest Neighbors (kNN), Logistic Regression, Decision Trees, and Support Vector Machines (SVM)—and determine which model is best suited for predicting client subscriptions.

Dataset
The dataset used for this project is titled "Bank Marketing" and includes data from marketing campaigns conducted by a Portuguese banking institution. The dataset contains the following key features:

Demographics: Age, Job, Marital Status, Education Level
Banking Information: Loan Status, Housing Loan, Default Status
Campaign Features: Number of Contacts, Last Contact Duration, Outcome of Previous Campaign
Economic Indicators: Employment Variation Rate, Consumer Price Index, Euribor 3-month rate
Target Variable: Whether the client subscribed to a term deposit (y)
Business Problem
The business problem revolves around predicting client behavior in marketing campaigns. Specifically, we aim to predict whether a client will subscribe to a term deposit (binary classification). The results can help the bank optimize future marketing strategies by targeting clients who are more likely to respond positively.

Models Used
The following machine learning models were implemented and compared:

k-Nearest Neighbors (kNN)
Logistic Regression
Decision Trees
Support Vector Machines (SVM)
Data Preparation
The dataset required cleaning and transformation before modeling:

One-Hot Encoding: Categorical variables were one-hot encoded to convert them into numerical form.
Feature Scaling: Continuous variables were scaled using StandardScaler to ensure models like SVM and logistic regression performed optimally.
Train/Test Split: The dataset was split into training (70%) and testing (30%) sets to evaluate model performance.
Evaluation Metrics
The models were evaluated based on:

Accuracy
Precision
Recall
F1 Score
ROC-AUC Score
These metrics provide a comprehensive understanding of model performance, especially for an imbalanced dataset where predicting the minority class (subscription) is crucial.

Findings
Baseline Model: A DummyClassifier using the most frequent class achieved a baseline accuracy of 88.76%.
Logistic Regression: After tuning, Logistic Regression reached a Test Accuracy of 90.07%, showing a slight improvement over the baseline. This indicates that the model is effective in predicting term deposit subscriptions but may not be capturing all data nuances.
Model Comparisons: While Logistic Regression showed strong performance, further model comparisons are ongoing. The Decision Tree model also showed competitive results after tuning, though its full evaluation is still in progress. Due to computational limits, the Support Vector Machine (SVM) model is pending further evaluation as the training process was lengthy.
Next Steps and Recommendations
Hyperparameter Tuning: Further optimization of hyperparameters could improve performance across all models.
Feature Engineering: Introducing new features based on domain knowledge may enhance prediction capabilities.
Imbalanced Data Handling: Investigating techniques like SMOTE or undersampling could be beneficial for dealing with class imbalance.
Conclusion
This project demonstrated the effectiveness of different classification models in predicting client subscriptions. Logistic Regression emerged as a strong contender, but additional fine-tuning and comparisons with Decision Trees and other models could further refine the results.
