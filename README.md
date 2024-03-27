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
<img width="643" alt="Screenshot 2024-03-27 at 5 44 21 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/456b2536-7414-47de-b1a7-d66f27de5122">
<img width="488" alt="Screenshot 2024-03-27 at 6 29 40 PM" src="https://github.com/sobaworm/Shoe-Box/assets/164225733/8f20e787-798a-43ed-88df-9b0e2da27437">
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

