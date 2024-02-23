# Rice Datathon 2023
This group project looked to determine whether an MLB team’s travel schedule and fatigue had any effect on a team’s in game performance. Initially through our exploratory data analysis, we found that there was significant evidence for the prevelance of home-field advantage, and, through a Granger Causality Test, we found that there was no evidence to support causality between the distance travelled by a team, and their offensive and defensive on-base percentage(OBA).

We looked to get a baseline understanding of a team’s ability by developing an ELO ranking system derived from 538’s NFL ELO system, accounting for margin of victory and pitching form. Additionally, two scalars which controlled the extent of ELO change were found by determining what the scalars were when the AUC-ROC score was highest.

We then used ELO and a mixture of fatigue metrics(distance travelled, jet lag, days away team has been on the road, and the difference in travel direction for both teams) in an XGBoost model which looked to predict the probability of the home team winning for each game. Through a feature analysis, we found that the fatigue metrics had very little effect on the model’s predictions, concluding that fatigue and travel had very little effect on a team’s in game performance.

This project was a submission for the 36-hour 2024 Rice Datathon, where we finished 2nd place overall out of 59 teams.
