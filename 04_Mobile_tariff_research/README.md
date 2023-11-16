# Determining a promising tariff for a mobile operator

#### Introduction

The mobile operator "Megaline" offers customers two tariff plans to choose from: “Smart” and “Ultra”. To adjust the advertising budget, the commercial department wants to understand which tariff brings in more money.
We have at our disposal the data of 500 "Megaline" users: who they are, where they are from, what tariff they use, how many calls and messages each person sent in 2018.

#### Purpose of the study:

To analyze customer behavior and to draw a conclusion: which tariff, “Smart” or “Ultra,” brings the company more money.

#### Tasks:
- To explore the data;
- To perform data preprocessing;
- To conduct exploratory data analysis and calculate monthly revenue from each user;
- To test hypotheses:
  - Average revenue from users of “Ultra” and “Smart” tariffs differs;
  - Average revenue from users from Moscow differs from revenue from users in other regions.

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Folium
- Scipy

#### Short summary:
- We tested two hypotheses:
  1. Hypothesis about the difference in average revenue from users of “Smart” and “Ultra” tariffs;
  2. Hypothesis about the difference in average revenue from users from Moscow and from other cities.<br>
  
  Based on the statistical test, we were unable to reject the first hypothesis. Upon manual check, it turned out that average revenues differ significantly in favor of the “Ultra” tariff.<br>
  But our second hypothesis about the difference in average revenue from users from Moscow and from other cities was not statistically confirmed. Although, when we manually calculated average revenues, it turned out that the average revenues from users from Moscow and from other cities differ, but not too significantly: by a little over 20 rubles.

- Based on the results of our research, we can conclude which tariff is more promising for the company in order to adjust the advertising budget. We believe that the “Smart” tariff is the most promising, and here’s why:
  - More users and more intensive growth of their number;
  - Users of the “Smart” tariff are much less likely to terminate the contract;
  - “Smart” tariff users bring more profit to the company than “Ultra” tariff users - 58.5% versus 41.5%;
  - The average revenue per user of the “Smart” tariff, although lower than that from the user of the “Ultra” tariff, increased by 2 times during the year, while the average revenue per user of the “Ultra” tariff remained almost unchanged;
  - Considering the trend of intensive growth in the number of users of the “Smart” tariff and the growth in the volume of services consumed by them, and consequently the average revenue per user, we can expect that the share of the company’s profit from the “Smart” tariff will only grow, and the share of profit from the “Ultra” tariff - decline.<br>
  
- Therefore, we recommend more actively advertising the “Smart” tariff.
