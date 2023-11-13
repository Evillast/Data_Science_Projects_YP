# Research of advertisements for the sale of apartments in Saint Petersburg and the Leningrad region

#### Purpose of the study:

To study the data of the Yandex Real Estate service - an archive of advertisements for several years about the sale of apartments in St. Petersburg and the Leningrad region in order to find interesting features and dependencies that exist in the real estate market, and determine the factors that most strongly influence the cost of apartments.

#### Tasks:
- To review the data;
- To perform data preprocessing;
- To conduct exploratory data analysis:
  - To determine which parameters most influence the total cost of the object;
  - To identify settlements with the highest and lowest cost per square meter;
  - To study the distribution of apartment prices in St. Petersburg.

#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Phik
- Geopy

#### Short summary:
- We found that the following parameters most strongly influence the cost of apartments:
  - total area;
  - living space;
  - kitchen area;
  - number of rooms;
  - ceiling height;
  - distance to the center of St. Petersburg;
  - year of publication of the advertisement.
- Among the settlements from the top 10 by the number of advertisements, the highest average cost per square meter, as expected, is in St. Petersburg and Pushkin, and the lowest is in Gatchina, Vsevolzhsk and Vyborg.
- The rating of advertisements with the highest average cost per square meter among all settlements was topped by Zelenogorsk. In second place is St. Petersburg. Pushkin ended up only in 5th place.
- We also studied how the average cost per square meter is distributed in St. Petersburg depending on the distance to the center. We came to the conclusion that the closer to the center, the higher the cost per square meter.
