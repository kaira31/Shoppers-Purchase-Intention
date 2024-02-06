# Shoppers-Purchase-Intention
## Introduction
In an era where brick-and-mortar businesses are dwindling, online shopping has become the norm for consumers. From clothes to household goods and groceries, users are increasingly choosing virtual shopping. This project delves into the factors that influence users' decisions to make online purchases, including factors such as the month, weekend presence, and product type. We employ custom machine learning tools like logistic regression, support vector machines (SVM), Naive Bayes, and Neural Networks to analyze what drives revenue generation and determine the most performant machine learning methods.

## Data Description
## Dataset Link: Online Shoppers Purchasing Intention Dataset

The dataset comprises 12,330 observations with 18 features. Most features are numeric and were pre-encoded before preprocessing. Key features include Bounce Rates, Special Day, Month, Weekend, and the response variable, Revenue, indicating purchase outcomes. There were no null values in the dataset.

## Methods
## Pre-processing
Conversion of non-numeric values using a label encoder.
Resampling to balance the y-values (0 and 1).
Removal of feature pairs with correlations above 0.5 to avoid collinearity.
## Modeling
Logistic Regression as a baseline model.
Soft margin SVM to allow for some misclassification.
Naive Bayes for its simplicity and low data requirements.
Manual hyperparameter tuning and regularization terms.
Evaluation metrics include accuracy, F1 score, precision, and recall.
Cost analysis of time to influence model selection.
## Exploratory Data Analysis (EDA)
Visualization of the proportion of True (1) and False (0) for balancing insights.
Analysis of visitor types by month and special day correlations.
Understanding the impact of month and visitor type on revenue (True/False).
## Results
## Logistic Regression Model
Logistic Regression models the probability of input belonging to a class using a logistic function. The logistic regression hypothesis:

After modeling, the optimal lambda value of 0.01 yielded the highest performance metrics:

Accuracy: 0.84
F1 Score: 0.91
Precision: 0.85
Recall: 0.97
## Naive Bayes Model
Naive Bayes, rooted in Bayes' theorem, offers simplicity and efficiency. Results include:

Accuracy: 0.81
F1 Score: 0.88
Precision: 0.89
Recall: 0.88
## SVM Model
Support Vector Machines aim to find the optimal hyperplane for classification. Results:

Various SVM models with different techniques.
Optimal lambda value: 0.1.
Accuracy: 0.84
F1 Score: 0.91
Precision: 0.85
Recall: 0.97
## Neural Networks Model
A feedforward neural network with two hidden layers and dropout regularization. Results:

Test Accuracy: 0.85
Test Loss: 0.41
## Conclusion
Logistic Regression strikes a balance between performance and practicality. It performs well where relationships between features and the target variable are approximately linear. While Neural Networks offer power, they can be computationally expensive and less interpretable, making Logistic Regression a suitable choice for many classification tasks.
