# MIST4610 Group Project 1

## Team Information
**Team Name:** 21484 Group 8

**Team Members:**
- Jennifer Kim [@sobaworm](https://github.com/sobaworm)
- Kevin Shen [@kevinshen8](https://github.com/kevinshen8)
- Michael Smith [@msmith165](https://github.com/msmith165)
- Nick Lanoce [@nicklanoce7](https://github.com/Nicklanoce7)
- Tripp Trimble [@tripptrimble2](https://github.com/tripptrimble2)

## Problem Description
We are tasked with developing a regional database that effectively organizes the complex dynamics of a professional sports team. The core entity is the ‘Team’, which represents the organization around which all activities, including player management, match scheduling, and fan interactions revolve. Key components include maintaining detailed records of players, their engagements, game statistics, training sessions, and youth player progress. The database must be capable of reflecting real-life associations, such as which players are part of which teams, the historical performance in matches, and fan purchases. We aim to create sample data that will populate the database and replicate a realistic operational scenario. By performing various queries on this data, the database should provide in insights into team performance, fan engagement, and financial health, thereby supporting strategic business decisions for the sports organization. 

## Data Model
### Explanation of the Data Model
Our data model is a streamlined representation designed to capture the ecosystem of a sports organization. Central to our model is the Team entity, which is considered the core for a constellation of players, staff, and their interactions.

Player profiles form the foundation of our model, which details the demographics but also contractual and performance data, each linked to a single Team yet part of an intricate web that includes GameStats and TrainingSessions. The one-to-many relationship between Player and Gamestats reflect a detailed record of their contributions across matches, while their growth and development are tracked through various TrainingSessions, tied to their respective teams.

The Match entity chronicles the competitive engagements of our teams, intertwining with the Results to capture the outcomes and metrics that matter the most. It stands as a beacon for fan experiences, tied directly to TicketSales, each match generates various transactions, creating a one-to-many relationship that maps out the journey from ticket purchase to real time.

FanEngagement events, represent our commitment to interactive fan experiences, form a many-to-many relationship with Player through PlayerEngagements. This depicts the multifaceted interactions our athletes have with their supporters.

The Coach entity and the Team are in one-to-many partnership, showcasing the leadership and tactical expertise that drive team performance. Meanwhile, Merchandise connects to the Team to present a suite of branded items available to fans. This shows the one-to-many bond between products and their team affiliations.

This data model not only charts the current state ranging from player statistics to match day sales, but also serves as a tool for planning and development, highlighting key areas like talent, progression, fan engagement, and revenue, all while maintaining a fan-centric approach to the business of sports. 




### Entity Relationship Diagram (ERD)
![FBF9E232-75E1-45F3-AE93-78587083CC09](https://github.com/sobaworm/Shoe-Box/assets/164225733/09b60b52-a34b-40d1-aebe-975b40755a0f)



## Data Dictionary
<img width="588" alt="Screenshot 2024-03-27 at 7 00 08 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/8d685565-6874-44d8-badd-d2fae479306d">
<img width="596" alt="Screenshot 2024-03-27 at 7 00 18 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/97478f00-5d10-421a-af38-b5e196fe4c47">
<img width="580" alt="Screenshot 2024-03-27 at 7 00 42 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/0cbf2d92-359b-4f8b-9862-6cbbc9bde380">
<img width="592" alt="Screenshot 2024-03-27 at 7 00 53 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/c3c2e599-9f97-4c82-b6ae-46386afbebf9">
<img width="586" alt="Screenshot 2024-03-27 at 7 01 03 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/446424d2-015d-406f-a621-07a715b4dd2f">
<img width="592" alt="Screenshot 2024-03-27 at 7 01 15 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/00202db8-15f5-403f-a87a-26c71308ca41">
<img width="580" alt="Screenshot 2024-03-27 at 7 01 23 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/dc487bb5-428e-4106-a5de-b9c9e807d2ce">
<img width="579" alt="Screenshot 2024-03-27 at 7 01 37 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/05d96502-8084-4ebe-a378-03a7333b0ba5">
<img width="604" alt="Screenshot 2024-03-27 at 7 01 46 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/92aa7be7-c558-44b0-8e5e-f5284b254396">
<img width="601" alt="Screenshot 2024-03-27 at 7 01 54 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/fb9df46a-b1f0-4297-b0f4-be2350845f1a">
<img width="586" alt="Screenshot 2024-03-27 at 7 02 03 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/cb59cc64-16b3-4b65-8d41-56747da68df3">




## Queries

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/2550a149-c312-478e-8552-becb397fe590)

#### Query 1

Query 1: Write a query to determine the number of events each goalkeeper is registered for 

This query identifies the number of fan engagement events each goalkeeper is registered for along with their names and positions. It provides insights into the level of involvement of goalkeepers in fan engagement activities which is essential for understanding their public engagement and potential marketing opportunities. The use of GROUP BY cause organizes the data by individual goalkeepers which allows a clear view of the player’s engagement level.

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/303391bc-8d52-4165-b3d2-8ff991d18d48)


#### Query 2
Query 2: Write a query to determine matches where ticket prices are higher than average, given the match occurs in Goal Arena

This query focuses on matches held at the Goal Arena. The ticket prices here are higher than average. By joining the Match and TicketSales tables, it helps in pinpointing those matches that might be of interest or higher value which guides marketing and pricing strategies. The conditional structure of the query ensures that only matches with above-average prices at this specific venue are selected. 

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/a75f4c56-6259-4ed3-8cba-73c50c9c8bd7)


#### Query 3
Query 3: Write a query to determine the total number of tickets sold for each match

This query calculates the total number of tickets sold for each match along with the match dates. This is crucial for guaging the popularity of different matches and managing stadium capacities and logistics. Grouping by match ID and date provides a clear breakdown of ticket sales per event which assists in revenue analysis and forecasting. 

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/f509c0a0-7a4f-45a4-b6db-3cd748247ca9)

#### Query 4
Query 4: Write a query to find any players who have not participated in any fan engagement events

This query identifies players who have not participated in any fan engagement events. This information can be pivotal for player management and marketing teams to encourage greater involvement from these players or to understand potential reasons for their lack of engagement. 

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/9691997e-6531-472c-96dc-9b9a0972acee)

#### Query 5

Query 5: Write a query to list the players with the highest market value and what team they play for and how many training sessions they have attended to see if the amount of training sessions attended has a correlation with market value.

This query lists players with the highest market value, their teams, and the number of training sessions they have attended. By examining the correlation between market value and training attendance, this provides insights into player development and valuation. Sorting by market value emphasizes the top-valued players, which in turn offers a clear perspective on high-value assets in the team. 

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/9ac62e7b-112b-465b-be39-4ebafbdda004)

#### Query 6

Query 6: Provides Team wins among teams who have more than 15 wins

The stored procedure WinningTeams is designed to list the teams with more than 15 wins, which showcases their team IDs, names, and total number of wins. This is achieved by joining the Results and Team tables where the procedure focuses on matches where the team’s score surpasses that of their opponents, which indicates a win. The data is grouped by team ID to accumulate wins per team, and a HAVING clause is applied to filter out teams with 15 or fewer wins. The results are ordered in descending order of wins which prioritizes teams with the highest number of victories. This is useful for analyzing team performance and is a valuable tool for sports analysts, commentators, and fans.

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/4ab83f6f-abd9-4e98-820a-fdecfdc5d6e1)


#### Query 7
Query 7: List the market value of the team

This query calculates the total market value of each team. This provides a crucial financial perspective on the teams. It achieves this by summing up the marking values of all players within each team. Additionally, by joining with the Results table and ordering the results based on the average team score in descending order, this tells us the correlation the team’s on-field performance with its collective market value. This data is necessary in understanding the financial strength and potential on-field success of each time which aids in strategic planning and assessment of team value.

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/dfb86259-cfac-414f-9dc0-c7b5dd1974c3)


#### Query 8
Query 8: Query to show the total goals for each team with at least X goals

This query is designed to display the total goals by each team, buy only for those teams that have scored more than a threshold amount. In this case, 200 goals. By summering the teamScore from the Results table and grouping by each team’s name the query filters out teams with lower total goals which focuses on high-scoring teams. This approach provides a clear view of the most successful teams within the league. This is key for analysis of team performance, planning, and for potential media and fan engagement, as it highlights the teams with notable goal-scoring record.

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/67b979d3-3e38-49bf-baf2-e72558ae2eb2)

#### Query 9
Query 9: If I wanted to know the price of a t-shirt for any player from a Republic

This query is designed to retrieve the prices of t-shirts related to players from any Republic along with their names, team names, and nationalities. By joining the Player, Team, and Merchandise tables and applying a condition to filter players based on nationality(containing Republic) and the type of merchandise(t-shirts). The query groups the results by player name, team name, price, and nationality, which ensures each entry represents a unique combination of these elements. By ordering the results by the player’s name, its easy to reference and compare. This is useful for fans or retailers looking to purchase or stock merchandise correlated to players from specific nationalities, which provides a clear overview of available options and prices.

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/a88069b1-52fa-4fd2-b19a-502ba8fa1f94)

#### Query 10
Query 10: Determines total salaries of all coaches on the team
 
The stored procedure CoachSalary is designed for calculating the total salaries of all coaches associated with a specific team within an organization. By taking an input parameter (theTeamID). This represents the unique identifier of a team. The procedure focuses on aggregating the salaries from the Coach table for those coases linked to Team_teamID. This functionality is valuable for a sports organization’s financial mamagementy and budgetary assesments which allowes for an effient way to determine the collective financial commitment towards the coaching staff of any given team. The stored procedure simplifies the task of assessing coaching expenses across different teams which promotes ease of use and ensures consistent tracking.

![image](https://github.com/sobaworm/Shoe-Box/assets/164225733/e5b9d447-afc0-4bc6-a103-fd1a2d94d670)

## Database Information
**Database Name:** ns_Sp24_21484_Group8

Additional information:

1.)  call TeamsOver200 (Query 1): Retrieves information about teams having more than 200 recorded activities or entries.


2.) call TeamMarketValue (Query 2): Gathers data on the market value of each team within the database.
   

3.) call RepublicTshirt (Query 3): Accesses details about the Republic-themed t-shirts, including sales, stock, and designs.
 

4.) call PlayersWithoutEngagements (Query 4): Lists players who currently do not have any engagements or contracts.


5.) call MatchTixSold (Query 5): Provides information on the number of tickets sold for various matches.


6.) call MarketValuePerTrainingSession (Query 6): Analyzes the market value of teams or players per training session attended.
 
7.) call GoalArenaPremiumMatch (Query 7): Extracts details about premium matches held at the Goal Arena, including ticket pricing, attendance, and special features.
 
