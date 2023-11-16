# Encryption algorithm to protect customer data
​
#### Purpose of the study:

To develop an algorithm for protecting personal data of insurance company clients.

#### Tasks:
- To explore the data;
- To develop a data encryption algorithm so that after conversion it is difficult to recover the information, while the quality of machine learning using linear regression should not decrease;
- To justify the correctness of the algorithm.

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Phik
- Sklearn

#### Short summary:
- We have proven algebraically that when multiplying the feature matrix by an invertible matrix, the prediction quality of the linear regression model will not change.
- Therefore, we proposed and justified the following data encryption algorithm:
  1. To divide the source data into features and target;
  2. To convert features from a dataframe into a matrix;
  3. To create a random square matrix with a width equal to the width of the feature matrix;
  4. To check the matrix for invertibility. If the matrix is irreversible, we generate a new matrix and repeat the check;
  5. To save the inverse matrix to the one we generated (encryption key) in order to be able to decrypt the data;
  6. To multiply the feature matrix by the generated invertible matrix;
  7. To convert the resulting encrypted matrix into a new dataframe.
- We also proposed a way to test this algorithm:
  1. To divide the original and encrypted features, as well as the target, into training and test samples;
  2. To train and test a linear regression model on original and encrypted features;
  3. To compare R2 metric (coefficient of determination): if the metric values are the same, the task was completed correctly.
- In the final part of the study, we implemented the proposed encryption algorithm and tested the linear regression model on the original data and data encrypted using our algorithm. We obtained the same value for the R2 metric when testing the model on the original and encrypted data, which means that the quality of the model’s prediction has not changed and the algorithm works correctly.
- Thus, our algorithm is able to protect the personal data of insurance company customers without reducing the quality of machine learning using the linear regression model.
