# Week 04

## Exercise 05

### Task 01

SELECT country.name
FROM country
WHERE country.iso_country IN (
		SELECT airport.iso_country
		FROM airport
		WHERE airport.name LIKE "Satsuma%"
		);

![task_01](https://github.com/user-attachments/assets/58e6b8ff-01e3-4b0e-ab4e-ed5a95038721)











  
