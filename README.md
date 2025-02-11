# Loan-Approval
Loan Approval
The goal of this project is to develop a model for predicting wheteher or not an applicant will be approved for a bank loan. The project is carried out as part of Kaggle Playground Series Season 4 Episode 10 and as part of my journey of learning data science and machine learning.

In this project, I will explore the data to discover the quirks of this specific dataset, by analyzing summary statistics, distributions of numerical and categorical variable, as well as correlations between features.

Next, I will prepare the data for modeling, which includes encoding features and imputing missing values. Since we are working with a synthetic dataset, I will not be performing any feature engineering.

I will construct 4 different classifiers, GradientBoostingClassifier, XGBoostClassifier, LightGBMClassifier and CatBoostClassifier, all of which are based on gradient boosting decision trees. These models are efficient for performing classification tasks.

To optimize the performance of the models, I will use Optuna to tune hyperparameters. The model performance will be evaluated using 5-fold cross-validation. Since the target variable is unevenly distributed, I will use StratifiedKFold to keep this relationship when performing the splits into folds.

I will compare the performance of the individual models, and create an ensemble model combining the predictions of the models using hill climbing. The models will be evaluated based on the area under the receiver operating characteristics (ROC) curve, or AUC for short. The ROC is the plot of the true positive rate versus the false positive rate, which is indicative of the performance of a binary classifier. A perfect model would yield an AUC of 1.0 and a bad model would likely be close to an AUC of 0.5, which is as good as guessing.
