# Model for predicting the recovery rate of gold from ore
​
#### Purpose of the study:

To prepare a prototype of a machine learning model that will predict the recovery rate of gold from gold ore and thereby help optimize production in order not to launch an enterprise with unprofitable characteristics.

#### Tasks:
- To explore data and to check whether the efficiency of ore enrichment is calculated correctly;
- To perform data preprocessing;
- To conduct exploratory data analysis:
  - To compare the size distribution of raw material granules on the training and test samples;
  - To explore how the concentration of gold, silver and lead changes at different stages of purification;
  - To explore the total concentration of all substances at different stages: in raw materials, in rough and final concentrates;
- To build and train various models and evaluate their quality using the sMAPE metric using cross-validation. It is necessary to predict two quantities at once:
  - gold recovery rate from the rough concentrate rougher.output.recovery;
  - gold recovery rate from the final concentrate final.output.recovery;
- To test the best model on a test sample.

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Sklearn

#### Short summary:
- First we compared the size distributions of raw material granules on the training and test samples. We came to the conclusion that the sizes of granules on the training and test samples do not differ too much, which means that models can be built;
- Then we explored the dynamics of changes in the concentration of metals - gold, silver and lead - at various stages of ore processing. We made sure that the concentration of gold increases with each stage. It was noted that the concentration of silver increases after flotation, but with each purification it begins to decrease. The lead concentration increases significantly until the second purification, then decreases slightly.
- We also explored the dynamics of changes in the total concentration of substances in the ore at various stages of processing: the share of gold in the raw material is on average only 14.4%, but in the final concentrate it is already more than 64%. While the average sol fraction, on the contrary, decreases from 64% to 13.7%. The average share of silver decreases by 2 times, the average share of lead increases by more than 2 times. The total concentration of all substances increases with each stage - especially after the final purification.
- We examined 7 regression models:
  - Linear regression;
  - Lasso regression;
  - Multitasking Lasso;
  - Multi-tasking elastic network;
  - Decision Tree Regressor;
  - Random Forest Regressor;
  - K-Nearest Neighbors Regressor.
- We assessed the efficiency of the models using cross-validation and the final sMAPE metric, for which we wrote a function. We used GridSearchCV to select the best hyperparameters for our models.
- Using the median DummyRegressor strategy, we set the model adequacy threshold on the training set to 9.35%. For real regression models, the final sMAPE on the training set should have been less than this value.
- The best result (8.18%) was demonstrated by the Random Forest Regressor model with hyperparameters: 'max_depth': 5, 'max_features': 0.7, 'min_weight_fraction_leaf': 0.1, 'n_estimators': 70.
- In the final part of our study, we tested the best model. Using the median DummyRegressor strategy, we set the model adequacy threshold on the test set to 7.32%. On the Random Forest Regressor model with the best hyperparameters, which showed the best result in cross-validation on the training data set, we got a result of 6.5%.
- Thus, to predict the recovery rate of gold from ore, we propose to use the Random Forest Regressor model with the hyperparameters indicated above.
