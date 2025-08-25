---
title: grade tracker
feed: show
date: 2024-01-15
tags:
  - "#projects/future"
  - "#personal"
---
![[Grade Tracker.png]]
my overcomplicated grade tracker - hopefully I can actually code a functional one that looks good soon 
### table outline 
|                                                                                       |                     |           | HIDE    | HIDE         |                | HIDE             | HIDE           |                   |                 |     |
| ------------------------------------------------------------------------------------- | ------------------- | --------- | ------- | ------------ | -------------- | ---------------- | -------------- | ----------------- | --------------- | --- |
| **TITLE**                                                                             | **CATEGORY**        | **GRADE** | **100** | **MULTIPLY** | **WEIGHT**     | **POINT EARNED** | **POINT LOST** | **CURRENT GRADE** | **POINTS TILL** |     |
| Discussion: Class Introductions                                                       | Start Here          | 100       | 100     | 100          | 0.01           | 1                | 0              | 1                 | 89              | A   |
| [M1: Assignment \| Introduction to R](https://canvas.tamu.edu/)                       | Assignments         |           | 100     | 0            | 0.09           | 0                | 0              |                   | 79              | B   |
| [M1: Interactive Lesson \| Data Mining Algorithms Overview](https://canvas.tamu.edu/) | Interactive Lessons |           | 100     | 0            | 0.006          | 0                | 0              | **LOST POINTS**   | 69              | C   |
| [M1: Perusall Assignment \| Lab: Introduction to R](https://canvas.tamu.edu/courses/) | Persual Labs        |           | 100     | 0            | 0.006666666667 | 0                | 0              | 0                 | 59              | D   |
| [Quiz \| Syllabus Acknowledgement](https://canvas.tamu.edu/courses/)                  | Start Here          |           | 100     | 0            | 0.01           | 0                | 0              |                   | 59              | F   |
|                                                                                       |                     |           |         |              |                |                  |                |                   |                 |     |
### process
1. copy and paste all assignments from the 'Grades' tab in Canvas 
	- this will bring in the full assignment title as well as a link to the assignment
2.  fill in category according to what category the assignment is
3. add weights by filtering the category column, then divide the weight by the number of assignments
	- if Assignments is 54% of the course, and there are 6 assignments, each one is weight 0.09 

### definitions
- table: name of the assignment
- category: category of the assignment
- grade: grade I earned
- 100: a column that literally says 100  
	- can be changed if assignments is out of 20 points for example
- multiply: percentage earned in assignment
	- $grade/'100'*100$
- weight: weight of the assignment 
	- read process to see how to assign weights 
	- has conditional formatting to highlight important assignments 
- point earned: points earned from assignment
	- $multiply*weight$
- lost points: points lost from assignment
	- $IF(grade<100,(weight*100-point earned),0)$
		- if to deal with all the zeros 
- current grade: current grade in class based on graded assignments
	- $sum(points earned)$
- lost points: current points lost based on graded assignments
	- $sum(points lost)$
- point till: tier system that states points till grade
	- $pointstreshold - currentgrade$
	- conditional formatting to highlight when a tier has been reached 

### what grade do I need? 
1. highlight unfilled assignments with red 
2. add proposed grade to 'GRADE' column
3. watch points till to see when desired grade is reached 