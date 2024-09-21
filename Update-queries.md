# Week 05

## Exercise 07

### Task 01

UPDATE game
SET location = (SELECT ident FROM airport WHERE name = "Nottingham Airport"),
co2_consumed = co2_consumed + 500
WHERE screen_name = "Vesa";

![task_01](https://github.com/user-attachments/assets/f0f3e952-290a-4f95-9953-ee6eeb8ced86)
