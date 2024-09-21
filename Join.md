# Week 04 

## Exercise 04

### Task 01

SELECT country.name AS "country name", airport.name AS "airport name"
FROM country
INNER JOIN airport ON airport.iso_country = country.iso_country
WHERE country.name = "Finland" AND airport.scheduled_service = "yes";

![task_01](https://github.com/user-attachments/assets/21a1463b-9703-4a51-ad1c-aa4cfa3edd96)

### Task 02

SELECT game.screen_name, airport.name 
FROM game
INNER JOIN airport ON airport.ident = game.location;

![task_02](https://github.com/user-attachments/assets/2454976b-ee17-48d7-a2e6-ea0c5edded47)

### Task 03

SELECT game.screen_name, country.name
FROM game
INNER JOIN airport ON airport.ident = game.location
INNER JOIN country ON country.iso_country = airport.iso_country;

![task_03](https://github.com/user-attachments/assets/7ae3f6b4-7e9c-4126-af88-c020c72569e5)

### Task 04

SELECT airport.name, game.screen_name
FROM airport
LEFT JOIN game ON game.location = airport.ident
WHERE airport.name LIKE "%Hels%";

![task_04](https://github.com/user-attachments/assets/7d5c5c29-adde-48ba-a78b-78fcad8f9b4b)

### Task 05

SELECT goal.name, game.screen_name
FROM goal_reached
LEFT JOIN game ON game.id = goal_reached.game_id
RIGHT JOIN goal ON goal.id = goal_reached.goal_id;

![task_05](https://github.com/user-attachments/assets/e2a98d56-6e3a-43b8-868b-555c0aba01db)













