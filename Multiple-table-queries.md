# Week 03 

## Exercise 03

### Task 01

SELECT country.name AS "country name", airport.name AS "airport name"
FROM country 
JOIN airport ON country.iso_country = airport.iso_country 
WHERE country.name = "Iceland";

![task_01](https://github.com/user-attachments/assets/de44a56c-4a82-4785-992b-9c444eed1b90)

### Task 02

SELECT airport.name AS "airport name" 
FROM airport 
JOIN country ON airport.iso_country = country.iso_country
WHERE country.name = "France" AND airport.type = "large_airport";

![task_02](https://github.com/user-attachments/assets/5f2da724-80ec-4d05-84e7-2e7d927eeb51)

### Task 03

SELECT country.name AS "country_name", airport.name AS "airport_name"
FROM country 
JOIN airport ON country.iso_country = airport.iso_country
WHERE country.continent = "AN";

![task_03](https://github.com/user-attachments/assets/e99d38f3-ad57-4e74-9888-70a45ded1825)

### Task 04

SELECT airport.elevation_ft 
FROM airport 
JOIN game ON airport.ident = game.location 
WHERE game.screen_name = "Heini";

![task_04](https://github.com/user-attachments/assets/07a6a94a-6f93-4eda-b433-a1b887487e1d)

### Task 05

SELECT airport.elevation_ft * 0.3048 AS "elevation_m" 
FROM airport 
JOIN game ON airport.ident = game.location 
WHERE game.screen_name = "Heini"

![task_05](https://github.com/user-attachments/assets/f924c583-f3e2-440a-8908-8912b7c2ab02)

### Task 06

SELECT airport.name 
FROM airport 
JOIN game ON airport.ident = game.location 
WHERE game.screen_name = "Ilkka";

![task_06](https://github.com/user-attachments/assets/ed4537cc-e4db-4298-9833-07ba040d9929)

### Task 07

SELECT country.name 
FROM country 
JOIN airport ON airport.iso_country = country.iso_country
JOIN game ON airport.ident = game.location 
WHERE game.screen_name = "Ilkka";

![task_07](https://github.com/user-attachments/assets/0d61034a-7f7f-42a5-9067-d59931f26e25)

### Task 08

SELECT goal.name 
FROM goal_reached 
INNER JOIN goal ON goal_reached.goal_id = goal.id
INNER JOIN game ON goal_reached.game_id = game.id
WHERE game.screen_name = "Heini";

![task_08](https://github.com/user-attachments/assets/f3105a4c-d2f2-4acf-bcf3-d3072c4f7946)

### Task 09

SELECT airport.name 
FROM goal_reached 
INNER JOIN goal ON goal_reached.goal_id = goal.id
INNER JOIN game ON goal_reached.game_id = game.id
INNER JOIN airport ON airport.ident = game.location
WHERE game.screen_name = "Ilkka" AND goal.name = "CLOUDS";

![task_09](https://github.com/user-attachments/assets/20ddc9d0-5d60-4e13-b436-e3b0edbf1160)

### Task 10

SELECT country.name 
FROM goal_reached 
INNER JOIN goal ON goal_reached.goal_id = goal.id
INNER JOIN game ON goal_reached.game_id = game.id
INNER JOIN airport ON airport.ident = game.location
INNER JOIN country ON country.iso_country = airport.iso_country
WHERE game.screen_name = "Ilkka" AND goal.name = "CLOUDS";

![task_10](https://github.com/user-attachments/assets/a3675094-3a1e-47e8-a46a-bb77aa578ec9)













