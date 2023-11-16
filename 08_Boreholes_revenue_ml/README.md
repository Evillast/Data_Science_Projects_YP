# Model for selecting a region for oil wells drilling
​
#### Introduction

The production company “GlavRosGosNeft” needs to decide where to drill new oil wells.

We were provided with oil samples in three regions: in each 100.000 wells, where the quality of oil and the volume of its reserves were measured.

#### Purpose of the study:

To select a region for developing new wells.

#### Tasks:

- To explore the data;
- To perform data preprocessing;
- To build a machine learning model that will help to select the region where mining will bring the greatest profit;
- To аnalyze possible profits and risks using the Bootstrap technique.

#### Conditions of the problem

- Only linear regression is suitable for model training;
- When exploring a region, 500 wells are examined, from which the best 200 are selected for development using machine learning;
- The budget for well development in the region is 10 billion rubles;
- At current prices, one barrel of raw materials brings 450 rubles in income. The income from each unit of product is 450 thousand rubles, since the volume is indicated in thousands of barrels;
- After assessing the risks, we need to leave only those regions in which the probability of losses is less than 2.5%. Among them, the region with the highest average profit is selected.

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Sklearn

#### Short summary:
- We trained and tested a model for each region. Region 3 had the highest average predicted oil reserves: about 95 thousand barrels.
- The model showed the best (lowest) value of the RMSE (0.89) and MAE (0.72) metrics, as well as the best (highest) value of the R2 metric (0.9996) in region 2. However, despite the high accuracy of the model’s prediction, this region received the smallest average reserve of predicted oil - 68.7 thousand barrels.
- We then calculated sufficient oil reserves to break even on developing a new well. It is equal to 111.11 thousand barrels. We compared sufficient oil reserves to the average oil reserves in each region. The average oil reserve in all regions turned out to be below the minimum required for break-even development, but this fact in itself says little, since out of 100 thousand wells, the best 200 out of a randomly selected 500 will go into development. The largest average oil reserves were also obtained in region 3: 95 thousand barrels.
- In the final part of the study, we implemented the Bootstrap technique with 1000 samples and found the profit distribution, calculated the average profit, found the 95% confidence interval of the profit, and calculated the probability of losses for each region.
- We came to the conclusion that for further development of oil wells it is recommended to choose region 2, since only this region has a probability of losses within the acceptable range (1%) and the average profit is higher than that of other regions (515.22 million rubles).
