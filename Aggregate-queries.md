# Week 05 

## Exercise 06

### Task 01

SELECT MAX(elevation_ft) FROM airport;

![task_01](https://github.com/user-attachments/assets/0f52de35-3c50-4295-8264-155dc0a65c68)

### Task 02

SELECT continent, COUNT(*) 
FROM country
GROUP BY continent;

![task_02](https://github.com/user-attachments/assets/37dfd9a8-a664-403b-bc5f-8a0a8d78659d)

### Task 03

SELECT game.screen_name, COUNT(*)
FROM game
JOIN goal_reached ON game.id = goal_reached.game_id
JOIN goal ON goal.id = goal_reached.goal_id
GROUP BY game.screen_name;

![task_03](https://github.com/user-attachments/assets/2bac7181-d7e4-445f-bf0c-e985796753dd)

### Task 04

SELECT game.screen_name
FROM game
WHERE co2_consumed = (
	SELECT MIN(co2_consumed)
	FROM game
);

![task_04](https://github.com/user-attachments/assets/3b55d83e-988f-4a2f-aa74-8250855690e2)

### Task 05

SELECT country.name, COUNT(airport.ident) AS COUNT
FROM country
JOIN airport ON country.iso_country = airport.iso_country
GROUP BY country.name
ORDER BY COUNT DESC LIMIT 50;

![task_05](https://github.com/user-attachments/assets/ea3307c0-fa2a-40f1-a1e7-9c09f2ef1bdc)

### Task 06

SELECT country.name
FROM country
JOIN airport ON country.iso_country = airport.iso_country
GROUP BY country.name
HAVING COUNT(airport.iso_country) > 1000;

![task_06](https://github.com/user-attachments/assets/1272e8be-57d3-4482-9885-ba6066202689)

### Task 07

SELECT airport.name
FROM airport
WHERE elevation_ft = (
	SELECT MAX(elevation_ft)
	FROM airport
);

![task_07](https://github.com/user-attachments/assets/7be83d4b-0974-4d73-bbe7-aff96ed77ed2)

### Task 08

SELECT country.name
FROM country
JOIN airport ON country.iso_country = airport.iso_country
WHERE airport.elevation_ft = (
	SELECT MAX(elevation_ft)
	FROM airport
);

![task_08](https://github.com/user-attachments/assets/f847bf8b-a669-4f7e-b5a4-d9b4ddaa5bb3)

### Task 09

SELECT COUNT(*)
FROM game
JOIN goal_reached ON game.id = goal_reached.game_id
JOIN goal ON goal.id = goal_reached.goal_id
WHERE game.screen_name = "Vesa";

![task_09](https://github.com/user-attachments/assets/18d0e2cc-2b9d-4036-94b1-52c37fe97e04)

### Task 10

SELECT name
FROM airport 
WHERE ABS(latitude_deg) = (
	SELECT MAX(ABS(latitude_deg))
	FROM airport
);

 ![task_10](https://github.com/user-attachments/assets/77db752e-4a82-4fa9-ab4b-d2af017cdab2)











