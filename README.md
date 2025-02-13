Analysis of Soccer Center Defender Counting Stats
===
By: Grady Lynch

Data from Opta Analyst and PremierLeague.com for 2024/2025 season as of 2/7/2025

Introduction
------------
The statistical data for the sport of soccer is very different than it is for most other sports. The low scoring nature of the game contributes to this. Specifically, I am focusing on the performance of center defenders in the English Premier League. In basketball and baseball, it's very easy to quantify a players performance by their stats. An NBA All-Star might average 25 points and 10 assists per game, and an MLB All-Star might have a .300 batting average. Well, what stats do you look at to determine what center defenders are the best? A center defender's jobs are to prevent goals and win the ball back for their team, but interestingly, the center defenders that concede less goals usually have less defensive counting stats while the defenders that concede more goals usually have higher defensive counting stats. The first plot that I created shows this interesting realtionship with a positive trend line. 

![image](https://github.com/user-attachments/assets/c1295a9c-be2e-4236-b6f3-b1df20dbf0df)

So how do we statistically determine which center defenders are performing the best?
----------------------------------------------------------------------------------------

The primary reason that defenders on worse performing teams have higher defensive counting stats is that they do more defending, and therefore have more opportunities to make tackles, blocks, clearances, etc. In order to get a better statistical picture of these stats, I created some visualizations that use stats I called 'True stats per 45'.

To create these stats, I first gathered the data for each teams average possesion, which is the percentage of a 90 minute game during which the team possesses the ball and is not defending. I then used the inverse of these percentages to calculate a stat, DefMinutes, that showed how many minutes the player has played this season on defense. Considering a baseline possesion percentage of 50%, and therefore 45 minutes of the 90 playing defense, I then calculated these True stats per 45 using 'DefMinutes'.

These first two plots show players blocks and clearances. The first one uses just regular per 90 stats, and the second one uses TrueBlocksPer45 and TrueClearancesPer45.

![image](https://github.com/user-attachments/assets/e183d21d-fd55-4038-a990-a60bf5889c63)

![image](https://github.com/user-attachments/assets/c0ff39e3-2ea7-4eba-9580-2680437ab62f)

With the True stats per 45 plot, you can see a small drop off in the stats of players from low average possesion teams like Ipswich Town and Southampton, and an increse in the stats of players from high possesion teams like Manchester City and Chelsea.

Comparison of per 90 and True per 45 Plots for Tackles vs Interceptions
--------------------------------------------------

![image](https://github.com/user-attachments/assets/f2ad8d95-fcac-4139-8f24-51ec43faa3da)

![image](https://github.com/user-attachments/assets/0b8c67db-9660-4154-910b-b7dd56659024)

Comparison of per 90 and True per 45 Plots for Ground Duels Won vs Arial Duels Won
--------------

![image](https://github.com/user-attachments/assets/155eadca-5c5b-4184-a46d-17dd6bcf379a)

![image](https://github.com/user-attachments/assets/807b2270-9fd7-450f-bd22-f8d254a86b5e)

Conclusion
===========

The adjustments made to these stats, when compared side by side, do clearly improve the quality of the statistical data. The True Per 45 stats paint a more accurate statistical picture of center defender performance than per 90 stats do. I think that the difference is most significant when it comes to analysing blocks and clearances. For the tackle, interception, and duels stats, I think that even more adjustments can be made. These stats are often accumulated in periods of transition during the game, and teams that play a more risky and volitile style of soccer will naturally have more periods of transition. I think that if there is a way to quantify the frequency of transitional periods in each teams game, those transitional counting stats could be adjusted and become much more indicative of the actual performance of center defenders.. 
