# Project 2: Machine Learning for Predicting Employee Attrition

## Introduction
This project focuses on leveraging Big Data analytics to predict employee attrition. Using a dataset of various employee characteristics, we explore several machine learning models to identify patterns and factors that contribute to employee turnover.

## Data Loading and Exploration
The data is loaded using Pandas, and preliminary data exploration is conducted to assess feature distributions and identify non-contributing features that can be removed.

# Load the dataset
data = pd.read_csv('path_to_train.csv')
data.head()
# Feature Engineering and Preprocessing

The dataset undergoes preprocessing where categorical variables are encoded using one-hot encoding, and irrelevant features are dropped to streamline the dataset for machine learning algorithms.

## Model Training

Several models are evaluated for their performance:
- Logistic Regression
- Random Forest
- Gradient Boosting
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Decision Tree
- Voting Classifier (ensemble method)

## Model Evaluation

Models are assessed based on accuracy, precision, recall, and F1-score metrics. Cross-validation is used to ensure robust evaluation.

## Results

The Voting Classifier, which combines predictions from multiple models, showed the highest accuracy and robustness, making it the preferred model for predicting employee attrition.

## Discussion

Pros and cons of various models are discussed, and the advantages of ensemble learning methods such as the Voting Classifier are highlighted.

## Conclusion

The application of ensemble methods in Big Data analytics proves to be highly effective in predicting employee attrition, demonstrating the potential of machine learning in HR analytics for organizational planning and management.

## Full Report

For a detailed methodology, comprehensive analysis, and insightful visualizations, please refer to the [full project report][(link_to_full_project_report)](https://github.com/LCQck/Y4S1-Big-Data-Analytics/blob/95d85ae62af0950c69667ca057f8233d226c536a/Project%202%20Machine%20Learning%20for%20Predicting%20Healthcare%20Employee%20Attrition/2039153_Changqing%20Lin%20Project%202%20Report.pdf) by Changqing Lin.

## Requirements

The requirements and specifications for Project 2 can be found in the [Project 2 Requirements][(link_to_project_2_requirements)](https://github.com/LCQck/Y4S1-Big-Data-Analytics/blob/95d85ae62af0950c69667ca057f8233d226c536a/Project%202%20Machine%20Learning%20for%20Predicting%20Healthcare%20Employee%20Attrition/Project%202%20Requirements.pdf) document.

## Source Code

The complete source code for all analyses, model training, and evaluations is available in the [Jupyter Notebook][(link_to_jupyter_notebook)](https://github.com/LCQck/Y4S1-Big-Data-Analytics/blob/95d85ae62af0950c69667ca057f8233d226c536a/Project%202%20Machine%20Learning%20for%20Predicting%20Healthcare%20Employee%20Attrition/2039153_Changqing%20Lin%20Source%20Code.ipynb).
