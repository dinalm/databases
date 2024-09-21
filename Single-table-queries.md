# Week 03 

## Exercise 02

### Task 01

SELECT * FROM goal;

![task_01](https://github.com/user-attachments/assets/96445653-a84a-4272-be89-3115878c5cf5)

### Task 02

SELECT name, type FROM airport WHERE iso_country = "FI";

![task_02](https://github.com/user-attachments/assets/67d34853-aaf2-4a02-a801-bc1797163e5e)

### Task 03

SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;

![task_03](https://github.com/user-attachments/assets/3ac98f97-a613-43d8-a175-5ac264ad1ba4)

### Task 04

SELECT name, type FROM airport WHERE iso_country = 'FI' ORDER BY type ASC, name ASC;

![task_04](https://github.com/user-attachments/assets/201ff4cd-7db2-463c-9724-86916ca8839d)

### Task 05

SELECT name FROM country WHERE name LIKE "F%";

![task_05](https://github.com/user-attachments/assets/d9c7bbe8-7076-4c1d-9191-22fdfdad0e07)

### Task 06

SELECT name FROM country WHERE name LIKE "%F%";

![task_06](https://github.com/user-attachments/assets/793ca310-c177-406f-9bf9-a73cd5ba2acc)

### Task 07

SELECT location FROM game WHERE screen_name = "Vesa";

![task_07](https://github.com/user-attachments/assets/9d639578-c2e0-49ed-9f41-adc0976f83fb)

### Task 08

SELECT co2_consumed FROM game WHERE screen_name = "Ilkka";

![task_08](https://github.com/user-attachments/assets/f8a2cf2e-0fc2-4f48-ad5b-e3797bdf36ce)

### Task 09

SELECT co2_budget FROM game LIMIT 1;

![task_09](https://github.com/user-attachments/assets/75fa72ba-b983-438c-b336-2b01790ab03d)

### Task 10

SET @co2_budget := (SELECT co2_budget FROM game WHERE screen_name = "Ilkka");
SET @co2_consumed := (SELECT co2_consumed FROM game WHERE screen_name = "Ilkka");
SELECT screen_name, 
		@co2_budget AS co2_budget, 
		@co2_consumed AS co2_consumed, 
		(@co2_budget - @co2_consumed) AS co2_left FROM game WHERE screen_name = "Ilkka";

  ![task_10](https://github.com/user-attachments/assets/99672137-b6ef-4f74-bc86-f778238187df)












