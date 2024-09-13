# Week 03

## Exercise 03

### Task 01

SELECT country.name AS "country name", airport.name AS "airport name"
FROM country 
JOIN airport ON country.iso_country = airport.iso_country 
WHERE country.name = "Iceland";

![task_01](https://github.com/user-attachments/assets/de44a56c-4a82-4785-992b-9c444eed1b90)
