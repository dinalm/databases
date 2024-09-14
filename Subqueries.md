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

### Task 02

SELECT airport.name
FROM airport
WHERE airport.iso_country IN (
		SELECT country.iso_country
		FROM country
		WHERE country.name = "Monaco"
		);

![task_02](https://github.com/user-attachments/assets/7fd55592-c909-4b65-8cf0-69db1f948bf9)

### Task 03

SELECT game.screen_name
FROM game
WHERE game.id IN (
		SELECT goal_reached.game_id
		FROM goal_reached
		WHERE goal_reached.goal_id IN (
			SELECT goal.id
			FROM goal
			WHERE goal.name = "CLOUDS"
		));

![task_03](https://github.com/user-attachments/assets/93102e3f-db70-41fd-ad9f-70434fb9dc02)

### Task 04

SELECT country.name 
FROM country
WHERE country.iso_country NOT IN (
		SELECT DISTINCT airport.iso_country
		FROM airport
		);

![task_04](https://github.com/user-attachments/assets/ca32df4a-0408-4cb7-8718-be6f76729749)

### Task 05

SELECT goal.name 
FROM goal
WHERE goal.id NOT IN (
		SELECT goal_reached.goal_id
		FROM goal_reached
		WHERE goal_reached.game_id IN (
			SELECT game.id
			FROM game
			WHERE game.screen_name = "Heini"
		));

![task_05](https://github.com/user-attachments/assets/69bf565a-73e8-4848-b951-69fc8bcdfb85)

























  
