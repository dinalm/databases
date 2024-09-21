# Week 05

## Exercise 07

### Task 01

UPDATE game
SET location = (SELECT ident FROM airport WHERE name = "Nottingham Airport"),
co2_consumed = co2_consumed + 500
WHERE screen_name = "Vesa";

![task_01](https://github.com/user-attachments/assets/f0f3e952-290a-4f95-9953-ee6eeb8ced86)

### Task 02

![task_02](https://github.com/user-attachments/assets/e09e6ee3-dd7f-4150-9551-6fa427d08dd6)

### Task 03

DELETE FROM goal_reached;

![task_03](https://github.com/user-attachments/assets/c7232b83-ce03-4af7-84fe-657a7acd065d)

### Task 04

DELETE FROM game;

![task_04](https://github.com/user-attachments/assets/6020e285-e626-46a1-a3b0-e1e7fb929224)

