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








