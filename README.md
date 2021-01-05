# Kaggle-NFL
### NFL Big Data Bowl 2021

An evaluation of defensive performance on passing plays during the 2018 NFL season.

### Contents

### data

#### Input files

- distance.csv
- distance_2.csv
- full_play.csv
- full-play_2.csv
- full_play_3.csv
- player_rankings.csv

#### Output files

- coverage_speed.xsls - output spreadsheet of coverage speed used in Table 4
- matchup1.xlsx - output spreadsheet of matchups used in Table 7
- matchup2.xlsx - output spreadsheet of matchups used in Table 7
- play_rankings_1s.xlsx - output spreadsheet of 1st-0 to 4 used in Table 5
- play_rankings_1m.xlsx - output spreadsheet of 1st-5 to 10 used in Table 5
- play_rankings_1l.xlsx - output spreadsheet of 1st-11+ used in Table 5
- play_rankings_2s.xlsx - output spreadsheet of 2nd-0 to 4 used in Table 5
- play_rankings_2m.xlsx - output spreadsheet of 2nd-5 to 10 used in Table 5
- play_rankings_2l.xlsx - output spreadsheet of 2nd-11+ used in Table 5
- play_rankings_3s.xlsx - output spreadsheet of 3rd-0 to 4 used in Table 5
- play_rankings_3m.xlsx - output spreadsheet of 3rd-5 to 10 used in Table 5
- play_rankings_3l.xlsx - output spreadsheet of 3rd-11+ used in Table 5
- play_rankings_4s.xlsx - output spreadsheet of 4th-0 to 4 used in Table 5
- play_rankings_4m.xlsx - output spreadsheet of 4th-5 to 10 used in Table 5
- play_rankings_4l.xlsx - output spreadsheet of 4th-11+ used in Table 5
- player_rankings.xlsx - output spreadsheet of players used in Table 2 and Table 3
- routes.xlsx - output spreadsheet of routes used in Table 6
- team_rankings.xlsx - output spreadsheet of team rankings used in Table 1


### notebooks
Many of the notebooks require input files created by other notebooks, so running the notebooks in the following order will ensure the proper results.

#### 1 - teams

- Defensive_Team_Rankings.ipynb - outputs team_rankings.xlsx

#### 2 - players

- Defensive_Player_Rankings.ipynb - outputs full_play.csv
- Defensive_Player_Rankings1.ipynb - uses full_play.csv to output player_rankings.xlsx and player_rankings.csv

#### 3 - coverage

- Defensive_Coverage.ipynb - uses full_play.csv to output full_play_2.csv
- Defensive_Coverage_1.ipynb - uses full_play_2.csv to output full_play_3.csv

#### 4 - proximity

- Defensive_Proximity.ipynb - uses full_play_2.csv to output distance.csv
- Defensive_Proximity1.ipynb - uses full_play_2.csv to output distance_2.csv
- Defensive_Proimity_2.ipynb - uses distance_2.csv and player_rankings.csv to output coverage_speed.xlsx

#### plays

- Defensive_Play_Rankings.ipynb - uses full_play_3.csv to output the 12 play_rankings spreadsheets.

#### routes

- Defensive_Route.ipynb - uses full_play_3.csv to output routes.xlsx

#### matchups

- Defensive_Matchups.ipynb - uses full_play_3.csv to output matchup1.xlsx and matchup2.xlsx

### main

- Final_Submission.ipynb
