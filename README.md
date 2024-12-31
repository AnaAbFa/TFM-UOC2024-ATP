# Lucky Losers and Protected Ranking in ATP Tour
Code used for the analysis of the retirements in previous ATP matches. Data obtained from https://github.com/JeffSackmann/tennis_atp.

**Variables**: 

Tourney_id: unique identifier for the tournament and the year it was played, includes 4418 different values. 
tourney_name: Name of the tournament, represented as a text variable. 561 possible values. 
surface: Type of surface the match was played on. Possible values: carpet, clay, grass, hard, or not available.
tourney_level: The level of the tournament. Categories include:
G: Grand Slams
M: Masters 1000 events
A: Other tour-level events
F: Tour finals and other season-ending events
year: the year the match took place, can take values from 1988 to 2022
best_of: indicates the format of a tennis match, referring to the number of sets required to win the match. It can be 3 or 5. 
round: The round of the tournament where the match occurred. Possible values include:
BR: Bye Round
ER: Early Round
F: Final Round
QF: Quarterfinal
SF: Semifinal
R16, R32, R64, R128: Preliminary rounds
RR: Round Robin
games: The games variable was created using the variable score from the original database.

Similarly, for the player characteristics: 

winner_id:
Unique identifier for the winning player. Includes 3,144 distinct values.
winner_entry:Type of entry for the winning player. Possible values:
WC: Wild card
Q: Qualifier
LL: Lucky loser
PR: Protected ranking
ITF: ITF entry
Additional values found in the database but not defined in the documentation: SE, ALT, Alt, NA
winner_hand: Dominant hand of the winning player. Possible values:
R: Right
L: Left
NA: Unknown
winner_ioc: Country of the winning player. Includes 96 distinct values.
winner_age: Age of the winning player. A continuous variable.
winner_rank: World ranking of the winning player at the time of the match. An integer variable.
loser_id: Unique identifier for the losing player. Includes 57,774 distinct values.
loser_entry: Type of entry for the losing player. Follows the same categories as winner_entry.
loser_hand: Dominant hand of the losing player. Follows the same categories as winner_hand.
loser_ioc: Country of the losing player. Includes 113 distinct values.
loser_age: Age of the losing player. A continuous variable.
loser_rank: World ranking of the losing player at the time of the match. An integer variable.
dif_age: Difference in age between the winner and loser. A continuous variable, can take negative values. Missing values (NA) are present in the data.
dif_rank: Difference in ranking between the winner and loser. A continuous variable, can take negative values. Missing values (NA) are present in the data.

