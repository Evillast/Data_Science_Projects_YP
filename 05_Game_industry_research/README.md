# Computer games industry research

#### Purpose of the study:

To researcg historical data available from open sources on game sales, user and expert ratings, genres and platforms and to identify patterns that determine the success of a game in order to predict the potential success of a product and plan advertising campaigns.

#### Tasks:
- To review the data;
- To perform data preprocessing;
- To conduct exploratory data analysis:
  - Research the dynamics of game releases over the entire period;
  - Research sales dynamics by platform over the years. Determine the average lifespan of the platform;
  - To explore:
    - Sales dynamics by platformm and to select several potentially profitable platforms;
    - How do user reviews and critics affect sales?
    - General distribution of games by genre and to find the genres with the highest and lowest sales;
  - To create a user profile for each region (North America, Europe, Japan):
    - To determine the most popular platforms and most popular genres;
    - To determine whether the ESRB rating affects sales in the region;
- To test hypotheses:
  - Average user ratings for the Xbox One and PC platforms are the same;
  - The average user ratings for the Action and Sports genres are different.
    
#### Used Libraries:
- Pandas
- Matplotlib
- Seaborn
- Numpy
- Scipy

#### Short summary:
- Active growth in the number of games released per year began in 1994 after the appearance of the first Pentium-based computers in 1993. Since 2002, the growth rate has accelerated even further with the introduction of Windows XP in 2001. The number of games released peaked in 2008-2009. Then, from 2010, a sharp decline began, caused by the consequences of the global economic crisis of 2008. Since 2014, a slight increase in the number of releases is again planned. It’s difficult to say anything about 2016, because data is incomplete.
- The absolute leader in sales was the PS2 platform. The top 6 also included the X360, PS3, Wii, DS and PS platforms. We also found that the average lifespan of each platform is 10 years. The peak of sales usually occurs in the middle of this period.
- We've found that the most potentially promising platforms for the coming years are the PlayStation 4 and Xbox One, as well as the perhaps still underrated Nintendo 3DS.
- We've found that critic reviews generally have a stronger positive impact on gaming platform sales than user reviews.
- The absolute leader in terms of the number of games released and the number of copies sold per year is the Action genre. However, it is impossible to call this genre 100% profitable, since it ranks 8th in terms of the number of sales per game. The most profitable genre is the Shooter genre. Also in the top 5 in terms of sales per game were the genres Platform, Sports, Role-Playing and Racing. The lowest sales were in the Strategy, Puzzle and Adventure genres.
- We also compiled a general portrait of the most common user for each region:
  - in Europe: a user playing 17+ Action games on PlayStation 4;
  - in North America: a user playing 17+ Action games on Xbox 360;
  - in Japan: a user who plays unspecified role-playing games on Nintendo 3DS.
- We then tested two hypotheses:
    1. The hypothesis about the equality of average user ratings for the Xbox One and PC platforms;
    2. The hypothesis about the inequality of average user ratings for the Action and Sports genres. <br>

  Based on the statistical test, we were unable to reject both hypotheses. During a manual check, we found that the average user ratings for the Xbox One and PC platforms differ slightly by a couple of tenths, and the average user rating for the Action genre is indeed noticeably higher than the average user rating for the Sports genre. <br>

- Thus, based on the results of our research, we can draw conclusions about which games (in which genres, on which platforms, in which regions) will be popular and bring profit.
In Europe and North America, it is worth advertising shooters and sports games for adults (17+, rated M by ESRB) on the PlayStation 4 and Xbox One platforms (in Europe they prefer PlayStation, in America Xbox), in Japan - Japanese role-playing games on Nintendo 3DS . You should pay attention to reviews from critics rather than from users - good reviews from critics have a positive effect on sales, but user reviews do not have the same effect.
