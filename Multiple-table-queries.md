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
WHERE screen_name = "Heini";

![task_04](https://github.com/user-attachments/assets/07a6a94a-6f93-4eda-b433-a1b887487e1d)

### Task 05









