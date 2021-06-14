# NFL-Play-Call-Classification

## Project Description

This project investigates how well we can predict if an opponent is going to run or pass the ball before the play even happens.  We’re looking to determine if we can find any patterns in the data set that can tell us which factors are most important in determining if a team is more likely to run the ball or pass for given situations.

### The Data

The data used for this project comes from one source:

NFLsavant.com  (play data from 2018-2020)

### Key Findings

Which situations are rushing situations?

Which situations are passing situations?

By determining what a team will do with the ball before they do it, we can position our defense much more confidently to stop the expected play type.  By positioning our defense more effectively, we can be successful much more often.

![image](https://raw.githubusercontent.com/Andoson22/Customer-Churn-Data/main/Images/Ratio%20of%20Churn.png)

Here we can see that our data has more passes than rushes.  Our goal will be to predict passes and rushes at a higher accuracy than the given frequencies.

Our most important features to the models are formation, down, and distance to go.

![image](https://raw.githubusercontent.com/Andoson22/Customer-Churn-Data/main/Images/Ratio%20of%20Churn.png)

#### Recommendations

1. On defense, game plan for SITUATIONS, not teams.  Situations are much more useful in predicting whether a team will rush or pass, rather than the team you’re going against.
2. Expect the expected.  Be prepared for a pass on passing downs, and a rush in rushing spots. (In general, as the down gets later and the distance gets longer, passing is more likely.)
3. On offense, employ a mixed games strategy.  Being unpredictable in play calling can significantly increase your yards on a play, and in turn increase potential points.  

## Conclusion



#### Future Work

- Incorporate score going into the play.  Being ahead or behind in a game may not matter much early on, but at what point down the stretch in games do teams tend to turn away from the game plan and go to a more pass dependent play-calling strategy to save time on the clock in hopes of coming back.  
- Look into a possible relationship between an offensive coordinator and the plays they call in situations.  (If an offensive coordinator changes teams, do they stick with the same system of plays, or adapt to their strategy to new players.  Useful against teams with veteran, first year coordinators.)
- Track data more robustly.  For example, record more meaningful ‘formations’.  Each team/coaching staff has different terminology for formations and plays...more insight can be gained from more specific formations and packages. (Player personnel can help determine what an opponent is most likely to do if their 'star' player is on or off the field)





