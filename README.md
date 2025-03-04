Analysis of Soccer Center Defender Counting Stats
===
By: Grady Lynch

Data from Opta Analyst and PremierLeague.com for 2024/2025 season as of 2/7/2025

Introduction
------------
The statistical data for the sport of soccer is different than it is for most other sports because of the low scoring nature of the game. In basketball and baseball, it's easy to quantify a players performance by their stats. An NBA All-Star might average 25 points and 10 assists per game, and an MLB All-Star might have a .300 batting average. In soccer you can use the number of goals scored to measure the performance of forwards, but what stats can you look at to measure the performance of other positions? For this project, I am focusing on the performance of center defenders in the English Premier League. A center defender's jobs are to prevent goals and win the ball back for their team. Interestingly, the center defenders that concede fewer goals usually accumulate fewer defensive counting stats than the defenders that concede more goals. Soccer fans often interpret these counting stats as evidence that these defenders that concede more goals are better defenders. However, a high number of goals conceded, as well as low team possession, are indicators of a badly performing team. Team possession is the percentage of the match during which the team has control of the ball. The first plot I created uses a trendline to show the relationship between goals conceded and defensive actions. The second plot aslo uses a trendline, but instead shows the relationship between average team possession and defensive actions.

![image](https://github.com/user-attachments/assets/c1295a9c-be2e-4236-b6f3-b1df20dbf0df)

![image](https://github.com/user-attachments/assets/5b5ee4f5-1fdd-45c8-9d4f-adb2fb179325)



How do we statistically determine which center defenders are performing the best?
----------------------------------------------------------------------------------------

The primary reason that defenders on worse performing teams have higher defensive counting stats is that they do more defending, and therefore have more opportunities to make tackles, blocks, clearances, etc. In order to get a better statistical picture of these stats, I created some visualizations that use stats I called 'True stats per 45'.

To create these stats, I first gathered the data for each team's average possession, which is the percentage of a 90 minute game during which the team possesses the ball and is not defending. I then used the inverse of these percentages to calculate a stat, DefMinutes, that showed how many minutes the player has played this season on defense. Considering a baseline possession percentage of 50%, and therefore 45 minutes of the 90 playing defense, I then calculated these True stats per 45 using 'DefMinutes'.

These first two plots show players' blocks and clearances. The first one uses just regular per 90 stats, and the second one uses TrueBlocksPer45 and TrueClearancesPer45.

![image](https://github.com/user-attachments/assets/e183d21d-fd55-4038-a990-a60bf5889c63)

![image](https://github.com/user-attachments/assets/c0ff39e3-2ea7-4eba-9580-2680437ab62f)

With the True stats per 45 plot, you can see a small drop off in the stats of players from low average possession teams like Ipswich Town and Notingham Forest (O'Shea and Murillo), and an increase in the stats of players from high possession teams like Manchester City and Chelsea (Dias and Chalobah).

Comparison of per 90 and True per 45 Plots for Tackles vs Interceptions
--------------------------------------------------

![image](https://github.com/user-attachments/assets/f2ad8d95-fcac-4139-8f24-51ec43faa3da)

![image](https://github.com/user-attachments/assets/0b8c67db-9660-4154-910b-b7dd56659024)

Notable differences: Chalobah (Chelsea) and Lacroix (Crystal Palace)

Comparison of per 90 and True per 45 Plots for Ground Duels Won vs Aerial Duels Won
--------------

![image](https://github.com/user-attachments/assets/155eadca-5c5b-4184-a46d-17dd6bcf379a)

![image](https://github.com/user-attachments/assets/807b2270-9fd7-450f-bd22-f8d254a86b5e)

Notable differences: Van Dijk (Liverpool) and O'Shea (Ipswich)

The final two scatter plots are the first plot shown, goals conceded per 90 vs defensive actions per 90, and a version of that plot that has been adjusted for team possession, true goals conceded per 45 vs true defensive actions per 45. 

![image](https://github.com/user-attachments/assets/cff7e55b-0403-4a86-9cc7-9f05f506a8fc)

![image](https://github.com/user-attachments/assets/92b634f7-72b5-418e-ba2f-50a07cf30e0d)



Conclusion
===========

Looking at the true goals conceded per 45 vs true defensive actions per 45 plot, the change in the slope of the trend line is very important. The slope of the trend line in the unadjusted plot is 0.75 and the slope of the trend line in the adjusted plot is 0.025. The significantly positive slope of the trend line of the unadjusted plot indicates the correlation between goals conceded, which is an indicator of a teams performance, and defensive actions. When the plot is adjusted for the calulated time each player actually spends defending, and therefore is able to make defensive actions and concede goals, The slope of the trend line gets very close to zero. A zero slope of the trend line indicates no strong relationship between true goals conceded per 45 and true defensive actions per 45. This means that the adjustments made are effective in correcting the inflation of defensive actions made by players on poorly performing teams.

The adjustments made to these stats, when compared side by side, do clearly improve the quality of the statistical data. The True Per 45 stats paint a more accurate statistical picture of center defender performance than per 90 stats do. The difference is most significant when it comes to analyzing blocks and clearances. For the tackle, interception, and duel stats, I think that even more adjustments can be made. These stats are often accumulated in periods of transition during the game, and teams that play a more risky and volatile style of soccer will naturally have more periods of transition. If there is a way to quantify the frequency of transitional periods in each teams game, those transitional counting stats could be adjusted and become much more indicative of the actual performance of center defenders.
