![icon](./assets/images/icon.jpeg "icon")

# This is the link to the github repo:
https://github.com/SINCHOCHAN/hw12

# This is the link to the live website:

https://sinchochan.github.io/hw12/

# PROJECT TITLE

Unit 12 MySQL Homework: Employee Tracker

Developers are often tasked with creating interfaces that make it easy for non-developers to view and interact with information stored in databases. Often these interfaces are known as **C**ontent **M**anagement **S**ystems. In this homework assignment, your challenge is to architect and build a solution for managing a company's employees using node, inquirer, and MySQL.

# User story

As a business owner
I want to be able to view and manage the departments, roles, and employees in my company
So that I can organize and plan my business


# How to run:

[runforhw12](./assets/images/runforhw12.mov "npm start") 

[run the test](./assets/images/runtest.png "screenshot of run the test") 

## Instructions

Design the following database schema containing three tables:

![Database Schema](./assets/images/schema.png "database schema") 

* **department**:

  * **id** - INT PRIMARY KEY
  * **name** - VARCHAR(30) to hold department name

* **role**:

  * **id** - INT PRIMARY KEY
  * **title** -  VARCHAR(30) to hold role title
  * **salary** -  DECIMAL to hold role salary
  * **department_id** -  INT to hold reference to department role belongs to

* **employee**:

  * **id** - INT PRIMARY KEY
  * **first_name** - VARCHAR(30) to hold employee first name
  * **last_name** - VARCHAR(30) to hold employee last name
  * **role_id** - INT to hold reference to role employee has
  * **manager_id** - INT to hold reference to another employee that manager of the current employee. This field may be null if the employee has no manager
  
Build a command-line application that at a minimum allows the user to:

  * Add departments, roles, employees

  * View departments, roles, employees

  * Update employee roles

Bonus points if you're able to:

  * Update employee managers

  * View employees by manager

  * Delete departments, roles, and employees

  * View the total utilized budget of a department -- ie the combined salaries of all employees in that department
