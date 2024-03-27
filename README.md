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




## Queries

#### Query 1
[Description]

#### Query 2
[Description]
#### Query 3

#### Query 4

#### Query 5

#### Query 6

#### Query 7

#### Query 8

#### Query 9

#### Query 10

...

## Database Information
**Database Name:** ns_Sp24_21484_Group8

Additional information:

