# MIST4610 Group Project 1
ASS DICK DOCK BOOTY
## Team Information
**Team Name:** 21484 Group 8

**Team Members:**
- Jennifer Kim [@sobaworm](https://github.com/sobaworm)
- Kevin Shen [@kevinshen8](https://github.com/kevinshen8)
- Michael Smith [@msmith165](https://github.com/msmith165)
- Nick Lanoce [@nicklanoce7] (https://github.com/Nicklanoce7)
- Tripp Trimble @[] (

## Problem Description
We are tasked with developing a regional database that effectively organizes the complex dynamics of a professional sports team. The core entity is the ‘Team’, which represents the organization around which all activities, including player management, match scheduling, and fan interactions revolve. Key components include maintaining detailed records of players, their engagements, game statistics, training sessions, and youth player progress. The database must be capable of reflecting real-life associations, such as which players are part of which teams, the historical performance in matches, and fan purchases. We aim to create sample data that will populate the database and replicate a realistic operational scenario. By performing various queries on this data, the database should provide in insights into team performance, fan engagement, and financial health, thereby supporting strategic business decisions for the sports organization. 

## Data Model
### Explanation of the Data Model
Our data model is a streamlined representation of our sports organization’s operations. At its core is the Team entity, encompassing our main roster and the developmental youth academy. 

The Player entity captures individual athlete profiles, forming a one-to-many relationship with Team. A team fields numerous players, yet each player commits to only one team. GameStats stem from each player's record, charting performance metrics in various matches, illustrating a player's journey through the seasons.

TrainingSessions are systematically recorded, linked to the Team to track the preparation and skill enhancement of our squads. Matches intersect with teams via the Match_has_Team junction table, a many-to-many link mirroring the reality that matches are the confluence of competing teams.

TicketSales and FanEngagement are the fan-focused entities, the former documenting the seats sold per match and the latter mapping players to their fan interactions through the PlayerEngagements junction.

Emerging talents are noted in the YouthPlayers entity, each with a direct link to their professional counterpart in Player, showcasing the growth path from junior ranks to the professional stage.

The Coach entity reflects the strategic minds guiding each team, while Merchandise offers a one-to-many snapshot of team-branded products available to fans.

In essence, this model captures the essence of our sports entity—team composition, player development, match day experiences, and fan relations—all working in concert to drive our organization forward.




### Entity Relationship Diagram (ERD)

<img width="590" alt="Screenshot 2024-03-27 at 5 36 27 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/54597857-da6e-4db8-a06e-adb71cdb0891">

## Data Dictionary
[Explain your data dictionary, or provide a link/image if it's external]

## Queries
### Query Descriptions
[Provide a brief description of each query and its purpose]

#### Query 1
[Description]

#### Query 2
[Description]

...

## Database Information
**Database Name:** [Database Name]
**Additional Information:** [Any additional details about the database]

## How to Run Queries
[Instructions on how to execute the queries, e.g., "CALL TP_Q1();"]

## About the Project
[Additional information about the project, its goals, outcomes, etc.]

## Resources
[Links to resources, documentation, or any other material relevant to the project]
