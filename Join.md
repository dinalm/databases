# Week 04

## Exercise 04

### Task 01

SELECT country.name AS "country name", airport.name AS "airport name"
FROM country
INNER JOIN airport ON airport.iso_country = country.iso_country
WHERE country.name = "Finland" AND airport.scheduled_service = "yes";

![task_01](https://github.com/user-attachments/assets/21a1463b-9703-4a51-ad1c-aa4cfa3edd96)













