## step 1

First step is to establish what questions I have or what I want to look into to fully understand  how it came to be that Man City won the premier League:

- How did teams fair offensively?
- How did teams fair defensively?
- Analyze disciplinary records for teams

## step 2
In this second step I'm thinking that I should organize the data into categories to to define the type of data they hold within them. The three main categories are as follows:

### Offensive
- big_chance_team.csv
- player_expected_assists.csv
- player_expected_goals.csv
- possession_percentage_team.csv
- team_goals_per_match.csv
- touches_in_opp_box_team.csv

### Defensive
- clean_sheet_team.csv
- goals_conceded_team_match.csv
- saves_team.csv
- won_tackle_team.csv

### Disciplinary
- player_fouls_committed.csv
- player_red_cards.csv
- total_red_card_team.csv
- total_yel_card_team.csv ❌
    - (upon looking through the tables `total_yel_card_team.csv` and `total_red_card_team.csv` had the exact same data, makimg it redundant info, leading me to drop `total_ryel_card_team.csv`)

The remaining tables `pl_table_2023_24.csv` & `pl_table_xg_2023_24.csv` are  tables that show the final Premier League Table and the latter is a table holding predictive values for goals, points, and etc.

## step 3
Third step in this process is to just see what data I have available to me, how it all relates to eachother or doesn't relate, if it helps me answer the questions i've posed and to essentially trim the fat if any tables dont aide me in this cause.

- my initial look through brought to my attnetion that majority of the tables had columns that really werent of any use when it came to my analysis so i started by trimming the fat there. Below are a couple screenshots of what I essentially did for all the tables:

dropping `player_expected_assists.csv` columns:

![player expected assists column drop](https://github.com/user-attachments/assets/51b8cc1e-982d-4e30-ae01-23cc790a183d)


output:

![player expected assists column drop output](https://github.com/user-attachments/assets/84ec1dd4-b1df-4935-91c6-1f98bd3db5d7)

dropping `player_expected_goals.csv` columns:

![player expected goals column drop](https://github.com/user-attachments/assets/5d374dfb-6282-4f99-af5f-678eb752335b)

output:

![player expected goals column drop output](https://github.com/user-attachments/assets/c16773fd-cbcd-44f4-bdc5-43834503e947)

- ⬆️ This was repeated throughout the database on all the various tables.

- As mentioned above, I had to get rid of the `total_yel_card_team.csv` due to duplicate information shared with `total_red_card_team.csv`:

Information included in `total_yel_card_team.csv`:

![yellow card team table](https://github.com/user-attachments/assets/56a6aff0-264b-4621-9c1e-6acbb9a9c4b8)


dropping `total_yel_card_team.csv`:

![DROP yellow card team](https://github.com/user-attachments/assets/6ec7fce0-0e7f-4457-ae9b-06922f76e1b4)


## step 4
I'm thinking my next step in this process is to:
- Join tables and save the joins as new tables
- further trim off any repetitive information or non-essential information
- differentiate tables between individual stats and team stats ( the basis on how the joins will be executed)


HEY!!👋🏿 IM BACK, and im happy to say I finished what I set out to accomplish in step 4!







  




