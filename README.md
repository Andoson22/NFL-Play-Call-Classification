# NFL-Play-Call-Classification

## Project Description

This project investigates how well we can predict if an opponent is going to run or pass the ball before the play even happens.  We’re looking to determine if we can find any patterns in the data set that can tell us which factors are most important in determining if a team is more likely to run the ball or pass for given situations.

### The Data

The data used for this project comes from one source:

NFL Savant  -  http://nflsavant.com/about.php  (play data from 2018-2020)

### Key Findings

We want to develop a model that can figure out if an opponent is likely to pass or rush given a certain set of circumstances in the game.

Are there specific rush heavy situations?

Are there specific pass heavy situations?

How often can our model corectly predict what our opponent is going to do?

By determining what a team will do with the ball before they do it, we can position our defense much more confidently to stop the expected play type.  By positioning our defense more effectively, we can be successful much more often.  By applying knowledge of the rules of the game, as well as general NFL knowledge, we can possibly proivde valuable insights to Offensive and Defensive coordinators. (For offensive coordinators, we can show them how predictable they are or aren't, and for defensive coordinators we can show them based on certain teams and in game situations, what they can expect to see coming their way.)

![image](https://raw.githubusercontent.com/Andoson22/NFL-Play-Call-Classification/main/Images/PassRushRatio.png)

Here we can see that our data has more passes than rushes. We need to undersample our majority class in order to balance our data to train it. Our goal is to be able to predict the play correctly more than 50% of the time.

![image](https://raw.githubusercontent.com/Andoson22/NFL-Play-Call-Classification/main/Images/PassRushRatio.png)

The ROC curve below shows us that our best model was our first Random Forest.  Looking deeper into our featues we can see...

![image](https://raw.githubusercontent.com/Andoson22/NFL-Play-Call-Classification/main/Images/ROCCURVEFINAL.png)

Our most important features were formation, down(more specifically 1st and 3rd down), and distance to go.  The position the players were lined up in prior to the ball being snapped was one of the strongest indicators to our classifier.  

![image](https://raw.githubusercontent.com/Andoson22/NFL-Play-Call-Classification/main/Images/Final%20Feature%20Importance3.png)

#### Recommendations

1. On defense, game plan for SITUATIONS, not teams.  Situations like the formation a team is lined up in, the down of the series, the yards left until they reach the first down, these are much more useful features in predicting whether a team will rush or pass, rather than the team you’re going against.
2. Expect the expected.  Be prepared for a pass on passing downs, and a rush in rushing spots. (In general, as the down gets later and the distance gets longer, passing is more likely.)
3. On offense, employ a mixed games strategy.  Being unpredictable in play calling can significantly increase your yards on a play, and in turn increase potential points.  



#### Future Work

- Incorporate score going into the play.  Being ahead or behind in a game may not matter much early on, but at what point down the stretch in games do teams tend to turn away from the game plan and go to a more pass dependent play-calling strategy to save time on the clock in hopes of coming back.  
- Look into a possible relationship between an offensive coordinator and the plays they call in situations.  (If an offensive coordinator changes teams, do they stick with the same system of plays, or adapt to their strategy to new players.  Useful against teams with veteran, first year coordinators.)
- Track data more robustly.  For example, record more meaningful ‘formations’.  Each team/coaching staff has different terminology for formations and plays...more insight can be gained from more specific formations and packages. (Player personnel can help determine what an opponent is most likely to do if their 'star' player is on or off the field)





