# Lucky Losers and Protected Ranking in ATP Tour
Code used for the analysis of the retirements in previous ATP matches. Data obtained from https://github.com/JeffSackmann/tennis_atp.

**Variables**: 
| **Variable**      | **Description**                                                                                   | **Values/Type**                                                                 |
|--------------------|---------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| `tourney_id`       | Unique identifier for the tournament and the year it was played.                                  | 4,418 distinct values.                                                         |
| `tourney_name`     | Name of the tournament.                                                                            | 561 possible values.                                                           |
| `surface`          | Type of surface the match was played on.                                                          | Categories: `carpet`, `clay`, `grass`, `hard`, `not available`.                |
| `tourney_level`    | The level of the tournament.                                                                      | Categories: `G` (Grand Slams), `M` (Masters 1000 events), `A` (Other tour-level events), `F` (Tour finals and other season-ending events). |
| `year`             | The year the match took place.                                                                    | Values from 1988 to 2022.                                                       |
| `best_of`          | Indicates the format of a tennis match, referring to the number of sets required to win the match. | Possible values: `3` or `5`.                                                   |
| `round`            | The round of the tournament where the match occurred.                                             | Categories: `BR` (Bye Round), `ER` (Early Round), `F` (Final Round), `QF` (Quarterfinal), `SF` (Semifinal), `R16`, `R32`, `R64`, `R128` (Preliminary rounds), `RR` (Round Robin). |
| `games`            | The games variable was created using the variable score from the original database.               | Continuous variable derived from the score.                                    |


Similarly, for the player characteristics: 
| **Variable**      | **Description**                                                                                   | **Values/Type**                                                                 |
|--------------------|---------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| `winner_id`        | Unique identifier for the winning player.                                                        | 3,144 distinct values.                                                         |
| `winner_entry`     | Type of entry for the winning player.                                                            | Categories: `WC`, `Q`, `LL`, `PR`, `ITF`, `SE`, `ALT`, `Alt`, `NA`.            |
| `winner_hand`      | Dominant hand of the winning player.                                                             | Categories: `R` (Right), `L` (Left), `NA` (Unknown).                           |
| `winner_ioc`       | Country of the winning player.                                                                   | 96 distinct values.                                                            |
| `winner_age`       | Age of the winning player.                                                                       | Continuous variable.                                                           |
| `winner_rank`      | World ranking of the winning player at the time of the match.                                    | Integer variable.                                                              |
| `loser_id`         | Unique identifier for the losing player.                                                         | 57,774 distinct values.                                                        |
| `loser_entry`      | Type of entry for the losing player.                                                             | Categories: `WC`, `Q`, `LL`, `PR`, `ITF`, `SE`, `ALT`, `Alt`, `NA`.            |
| `loser_hand`       | Dominant hand of the losing player.                                                              | Categories: `R` (Right), `L` (Left), `NA` (Unknown).                           |
| `loser_ioc`        | Country of the losing player.                                                                    | 113 distinct values.                                                           |
| `loser_age`        | Age of the losing player.                                                                        | Continuous variable.                                                           |
| `loser_rank`       | World ranking of the losing player at the time of the match.                                     | Integer variable.                                                              |
| `dif_age`          | Difference in age between the winner and loser.                                                  | Continuous variable (can be negative); missing values (`NA`) present.          |
| `dif_rank`         | Difference in ranking between the winner and loser.      
loser_ioc: Country of the losing player. Includes 113 distinct values.
loser_age: Age of the losing player. A continuous variable.
loser_rank: World ranking of the losing player at the time of the match. An integer variable.
dif_age: Difference in age between the winner and loser. A continuous variable, can take negative values. Missing values (NA) are present in the data.
dif_rank: Difference in ranking between the winner and loser. A continuous variable, can take negative values. Missing values (NA) are present in the data.

