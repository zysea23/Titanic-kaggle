# Titanic-kaggle
Starter notebook for the [Kaggle Titanic competition](https://www.kaggle.com/competitions/titanic): focus on handling missing data, feature analysis, and building a streamlined workflow.

## Initial Exploring
- The first time I approached this problem, I performed some normal data cleaning and feature engineering and fitted 3 models(logistic regression, random forest, XGBoost), achieving 82% validation accuracy and 77% test accuracy.
- The key is focusing on handling **missing data**, building a **streamlined workflow**, and **analyzing and processing various features**.

## General findings
- **Interpretability VS Accuracy:** While improving prediction accuracy is useful, for a historically significant event like the Titanic, interpretability takes precedence over accuracy.
- **Workflow:** This beginner-level competition is designed to help us develop a foundational understanding and workflow for handling datasets, building upon the balance of interpretation and predictive modeling.
- **Testset:** Data cleaning and feature engineering should consider both the training and test sets. Use a **combine list of `train_df` and `test_df`** could help and reduce complexity.
- **Quick Validation:** New-created features could be quickly validated for their predictive utility.
- **Categorical Features:** For tree-based models, using integers (e.g., 1, 2, 3) for non-ordinal categorical features often does not cause significant issues(like introducing implict ordering). However, for most models, one-hot encoding could be better(just pay attention to avoiding feature sparsity and losing implicit relationships).

## Other
- The notebook [Titanic Data Science Solutions](https://www.kaggle.com/code/startupsci/titanic-data-science-solutions/) provided valuable insights into data science workflows and in-depth analysis of each predictor. I learned a lot from this notebook.
