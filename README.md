# acm-project
Performing logistic regression on a dataset containing international football results from 1872-2021
This project was done based on the various data given in the dataset such as:
  * date - date of the match
  * home_team - the name of the home team
  * away_team - the name of the away team
  * home_score - full-time home team score including extra time, not including penalty-shootouts
  * away_score - full-time away team score including extra time, not including penalty-shootouts
  * tournament - the name of the tournament
  * city - the name of the city/town/administrative unit where the match was played
  * country - the name of the country where the match was played
  * neutral - TRUE/FALSE column indicating whether the match was played at a neutral venue
I added another column for home result in order to facilitate the analysis.
Logistic regression is used to determine the probability of an event using certain parameters.
For this project the first challenge was determining what I could predict given the basic details in the dataset. Considering the fact that the dataset doesn't provide significant in game statistics and only the final scores, venues etc. I decided to perform logical regression to prove the 'Home Advantage' concept in football.

In football it is often considered a great boost if a match is played at the team's home venue. Thus, a correlation between the amount of goals scored by the home team to the final outcome of the match can be drawn using this analysis.

* First step was to weed out International Friendly matches as they don't provide a true competitive sense for the sake of this analysis.
* Then we consider only the games where the 'Home Advantage' came into play by selecting only those entries where the country matched the home team
* Then training the model with the dataset and testing it and determining the accuracy of the model was the final step.

Additionally, I attempted to create the Logistic Regression plot but given the nature of Data and lack of adequate parameters the graph appeared to not prove much value, however I have added the code for that in quotes in case anyone wants to view it.
