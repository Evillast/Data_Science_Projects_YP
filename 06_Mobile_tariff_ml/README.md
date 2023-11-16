# Mobile tariff recommendation model

#### Introduction

The mobile operator Megaline offers customers two tariff plans to choose from: “Smart” and “Ultra”. We have data on the behavior of customers who have already switched to one of these tariffs.

#### Purpose of the study:

To build a machine learning model that will select the appropriate tariff for the user.

#### Tasks:
- To explore the data;
- To explore the quality of various models with different hyperparameters;
- To check models for adequacy;
- To build a model with the highest accuracy value (at least 0.75).

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Sklearn

#### Short summary:
- We examined 6 classifier models:
  - Decision Tree Classifier;
  - Random Forest Classifier;
  - Logistic regression;
  - Adaptive boosting;
  - Gradient boosting;
  - K-Nearest Neighbors Classifier.
- We also selected the best hyperparameters for these models using the validation set. Accuracy was used as a quality assessment metric.
- The best prediction accuracy on the validation set was shown by the Random Forest Classifier model with a maximum allowable tree depth of 11 and a number of trees of 55 (accuracy 0.827). Therefore, we recommend using it to select a tariff that suits the user.
