# NBA2k20 player database analysis Project with Python

## EDA and Correlation Python Pandas, MatPlotLib and Seaborn project that analyses NBA2k20 player database

In this project, I used Python Pandas, MatPlotLib and Seaborn, as well as my analytical skills to Export and Clean the data, Depict and Analyse the correlation of values and Visualise the data. It is initially a showcase of skills I have as an aspiring data analyst in Python, where I use a themed database that matches my personal interest in sports and gaming. "EDA and Correlation NBA 2k" consists of three main parts:

* Pandas Exporting And Cleaning: precise and specific preparation process for data used in the project
* Correlation Analysis: using a heat map and .corr to study correlation between values of the cleaned table with Pearson's correlation coefficient
* MatPlotLib and Seaborn EDA and Visualisations: using cleaned data and information about the correlated measures to plot and see the information from a different point of view

### See some data visualisation examples

![heightbar2k](https://github.com/dimitriousss/nba2k/assets/136066480/7f7ec0cc-776b-4b9a-9f37-dadf9f1fb646)
![linegraph2k](https://github.com/dimitriousss/nba2k/assets/136066480/55d85e8a-4dcc-4287-8e3a-5428f8faa7fd)
![pies2k](https://github.com/dimitriousss/nba2k/assets/136066480/732fd48f-8f64-4214-9f86-18869d8448a9)

### Project Conclusions

Correlation-Based Conclusions:
- We can see two pairs of highly correlated measures. Firstly, height and weight. These measures are generally correlated across all humans, especially ones that do competitive sports. Salary and rating are not too obvious. Rating in NBA2K games is generally used to represent the skill level of a player, whereas high salaries are often paid to better players and vice versa. Therefore, high correlation between these two pairs of measures is not surprising to see. Only thing to conclude is that player rating can be a good representation of salary range player is in, even though it is a subjective measure of players' skill sets.
- All three of draft-related measures presented and player ages have medium (or very close to medium) correlations with both salary and rating. This proves the previous point about the similarity between rating and salary in terms of representation from another perspective. However, the main conclusion is that generally players who stayed in the NBA for many years, as well as players picked early in the draft have better ratings and salaries.
- There is one very specific and extraordinary correlation discovered. Boolean is_american that represents if players are from the US or not has a close-to-medium correlation with players' height. It means that generally non-American players in the NBA are taller than the Americans. From my personal knowledge and the further analysis, I can think of one reason of this event. In the NBA, popular foreign players often play forward or center positions, which require physical abilities and, most importantly, the minimum of 2m of height on average.

Data Analysis-Based Conclusions:
- First graph gives us an insight on how height is distributed across the players' positions. Guards are under the 2-meter mark, while forwards and centers are taller than 2 meters on average.
- Second chart is showing the relationship between strongly correlated ratings and salaries. There is an extraordinary point visible on the visualisation - rating 84. Fall in average salary was most likely caused by following 2 factors: decline in real-life performance (ex. Kyle Kuzma) and players being on a verge of resigning (ex. Jamal Murray). This anomaly really shows that even though ratings and salaries are connected, these measures are very far from being perfectly correlated.
- Third visualisation consists of two pie charts that are showing the nationality distribution in the league. First graph shows that only a quarter of players are not from the United States, which, in my opinion, states a lack of diversity in the NBA. The biggest part of foreign players is from Canada. It is logical, knowing the fact that Canada is bordering the US and the city of Toronto has its own team in the league.
- Fourth and Fifth graphs show the best draft classes and pick numbers according to the average player ratings. Negative medium correlation takes place and it is visible on both visualisations. One of the earliest draft classes - 2003 is by far the best by rating. First seven picks obviously appear in table 5, but there are some extraordinary placements: pick 13 and 15 are in the top-10 and, most importantly, pick 27 is 4th on the list. It is interesting and unexpected for players drafted this late in the draft to all have great ratings (ex. Rudy Gobert and Pascal Siakam).
- Sixth set of bars charts show that:
  - the best rated team is Clippers, the most valuable player that season was not in any team of this top-5 and NBA champions were just fifth place by rating;
  - Warriors are by far the best-paying team, second team by rating is first in this category and vice versa;
  - Timberwolves is the youngest team, none of the teams in this category are the best-paying or best-rated;
  - Hornets are the highest-picked team; category consists of two of the youngest teams.
- Seventh swarm plot depicts the relationship of is_american and height, which was discovered in the correlation analysis. It shows that non-Americans have a tendency of being taller than Americans in the NBA (see correlation conclusion number 3).
- Eighth and last pair of graphs shows the relationship of is_american and height, but from another perspective. As said before (see correlation conclusion number 3 and analysis conclusion number 7), foreign players tend to be taller, and, theoretically, more frequently play forward and center positions. These two plots prove the theoretical assumption I made. There are more foreign centers than American centers, even though only a quarter of all players are from another countries (see analysis conclusion number 3). There is a ton of non-American guards, but there are more forwards from other countries, whereas Americans have the opposite situation.

Known issues: SettingWithCopyWarning: A value is trying to be set on a copy of a slice from a DataFrame. Will be fixed shortly

@ Dmytro Kvasha
