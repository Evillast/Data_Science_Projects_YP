# Model for predicting bank customer churn

#### Purpose of the study:

To build a machine learning model that can predict, whether a customer will leave the bank in the near future or not, based on historical data on customer behavior and termination of contracts with the bank.

#### Tasks:
- To explore the data;
- To perform data preprocessing;
- To build a machine learning model with an extremely large F1-measure value (at least 0.59);
- To measure AUC-ROC and to compare its value with the F1-measure.

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Sklearn

#### Short summary:
- We trained 5 models on an unbalanced sample:
  - Decision Tree Classifier;
  - Random Forest Classifier;
  - Adaptive boosting;
  - Gradient boosting;
  - Logistic regression.
- We also selected the best hyperparameters for these models using the validation set. We took the F1-measure as the main metric, and AUC-ROC as an additional metric.
- We then tried 4 methods to combat class imbalance:
  - Weighing of classes;
  - Increasing the sample;
  - Reducing the sample;
  - Changing the classification threshold.
- For testing, we chose one of the models that showed the best metric results on the validation set - the Random Forest Classifier model with the best hyperparameters 'max_depth': 6, 'n_estimators': 85. As a way to combat class imbalance, we chose to change the classification threshold and set it to the optimal value we found was 0.28. On the test set we achieved an F1-measure value of 0.63 and an AUC-ROC value of 0.87.
- Thus, to predict customer churn from the bank, we propose to use the Random Forest Classifier model with the above hyperparameters and a modified classification threshold.
