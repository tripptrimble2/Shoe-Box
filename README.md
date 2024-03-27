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
<img width="643" alt="Screenshot 2024-03-27 at 5 44 21 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/456b2536-7414-47de-b1a7-d66f27de5122">
<img width="493" alt="Screenshot 2024-03-27 at 5 45 35 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/1efea541-a4b0-413a-88f5-6a53f87f6430">
<img width="496" alt="Screenshot 2024-03-27 at 5 46 49 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/0036de30-9082-42cc-98df-59ab7750248f">
<img width="503" alt="Screenshot 2024-03-27 at 5 47 02 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/f7784297-2fce-4b7c-b934-94186218762f">
<img width="516" alt="Screenshot 2024-03-27 at 5 47 31 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/0d3d1a40-2eff-46e2-97ec-51e0fafd826b">
<img width="497" alt="Screenshot 2024-03-27 at 5 46 27 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/f6d7cf01-e856-47f7-8077-5f66a1d2c5bc">
<img width="511" alt="Screenshot 2024-03-27 at 5 47 44 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/364188e5-0f81-46b2-990a-1b46984b7973">
<img width="494" alt="Screenshot 2024-03-27 at 5 47 57 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/25082938-f8b2-4709-9eb0-28aa64635ad9">
<img width="478" alt="Screenshot 2024-03-27 at 5 48 32 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/02d9a64e-7fc3-416b-8c86-a161d98068ec">
<img width="492" alt="Screenshot 2024-03-27 at 5 48 49 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/dfd64c4a-1a43-4ab7-8cf4-0e034eee8138">
<img width="504" alt="Screenshot 2024-03-27 at 5 49 02 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/fd4737b7-422b-4555-8eaf-55778675e463">



## Queries
### Query Descriptions
[Provide a brief description of each query and its purpose]

#### Query 1
[Description]

#### Query 2
[Description]

...

## Database Information
**Database Name:** ns_Sp24_21484_Group8

**Additional Information:** [Any additional details about the database]

## How to Run Queries
[Instructions on how to execute the queries, e.g., "CALL TP_Q1();"]

## About the Project
[Additional information about the project, its goals, outcomes, etc.]

## Resources
[Links to resources, documentation, or any other material relevant to the project]
