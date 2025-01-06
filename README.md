# Gaming LeaderBoard Management System-PLSQL

## Project Created By:
Sabban Vedant Prakash student of Amrutwahini College of Engineering from Computer Engineering Department
(under Zensar SQL and Python Training)

## Project Description:
This project is a Gaming Leaderboard Management System designed to track and manage player scores, rankings, and match results across multiple games. The system comprises six interconnected tables: 
Players, Games, Scores, Matches, Match_Scores, and Rankings. It allows administrators to store player and game details, record match results, calculate total scores, and dynamically update player rankings
based on their performance in specific games. The system also supports features like ranking updates using total scores, historical tracking with timestamps, and cascading deletions to maintain database integrity. 
This solution provides a robust foundation for managing competitive gaming platforms or tournaments efficiently.

## Key Features:
1.Dynamic Player Rankings:Automatically calculates and updates player rankings based on their total scores for specific games, ensuring real-time leaderboard accuracy.
2.Comprehensive Match and Score Management:Tracks individual match results, player scores, and overall performance across multiple games, providing detailed insights into player statistics.
3.Database Integrity and Cascading Updates:Maintains referential integrity with cascading deletions and constraints, ensuring consistent data across tables like matches, scores, and rankings.

## Objective:
The objectives of this project are to efficiently manage players, games, scores, and match data in a centralized system, and to ensure accurate calculation and dynamic updates of player rankings 
for fair competition and transparent performance tracking.

## Technologies Used:
PL/SQL (Oracle Database) SQL(for queries , stored procedure)

## Output:

Player Table
----------------------------------------
| Player_id | Player_Name | Created_at |
|-----------|-------------|------------|
|     1     |    John     |  02-Jan-25 |
|     2     |    David    |  22-Dec-24 |
|     3     |   George    |  29-Dec-24 |
|     4     |    Mike     |  15-Dec-24 |
|     5     |   Steve     |  04-Jan-25 |
----------------------------------------

Games Table
-----------------------
| Game_id | Game_Name |
|---------|-----------|
|    1    |   Chess   |
|    2    |    OX     |
|    3    | BombSquad |
|    4    |   Ludo    |
|    5    |  Checkers |
-----------------------

Scores Table
----------------------------------------------------------
| Score_id | Player_id | Game_Name | Score | Achieved_at |
|----------|-----------|-----------|-------|-------------|
|    1     |    4      |   Ludo    |  50   |  06-Jan-25  |
|    2     |    1      |   Chess   |  850  |  01-Jan-25  |
|    3     |    4      | BombSquad |  900  |  02-jan-25  |
|    4     |    3      |    OX     |  700  |  03-Jan-25  |
|    5     |    2      | BombSquad |  1270 |  04-Jan-25  |
----------------------------------------------------------

Matches Table
-----------------------------------
| Match_id | Game_id | Match_date |
|----------|---------|------------|
|   151    |    1    |  05-Jan-25 |
|   152    |    3    |  06-Jan-25 |
|   153    |    1    |  03-Jan-25 |
|   154    |    2    |  05-Jan-25 |
|   155    |    2    |  03-Jan-25 |
-----------------------------------

Match_Scores Table
-------------------------------
| Match_id | Player_id | Score |
|----------|-----------|-------|
|    151   |     1     |  250  |
|    152   |     2     |  300  |
|    153   |     3     |  200  |
|    154   |     1     |  180  |
|    155   |     2     |  270  |
--------------------------------

Rankings Table
----------------------------------------------------------
| Player_id | Game_id | Total_Score | Rank | Last_Updated |
|-----------|---------|-------------|------|--------------|
|     1     |    1    |     430     |   2  |   04-Jan-25  |
|     2     |    1    |     570     |   1  |   04-Jan-25  |
|     3     |    1    |     200     |   3  |   04-Jan-25  |
|     1     |    2    |     180     |   1  |   04-Jan-25  |
|     2     |    2    |     0       |   2  |   04-Jan-25  |
-----------------------------------------------------------

# Conclusion:
In conclusion, the Gaming Leaderboard System provides an efficient way to manage players, games, scores, and rankings in a centralized database. It ensures accurate and dynamic ranking updates based on 
player performance, promoting fair competition and transparency. With its robust structure and integrity, the system is well-suited for managing competitive gaming platforms effectively.

## Guidance:
Project created under the guidance of Sir Anirudh Gaikwad.
