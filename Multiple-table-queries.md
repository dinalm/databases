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

