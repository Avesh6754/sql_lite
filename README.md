

# Employee Database Management System (DBMS) Queries

This repository demonstrates basic DBMS operations using SQL queries for an **Employee Management System**. The database contains the following fields: 

**`id`**, **`name`**, **`role`**, **`salary`**, **`age`**, **`address`**, **`phone`**.

---

## Table of Contents
1. [Add a New Employee](#1-add-a-new-employee)
2. [Retrieve All Employee Information](#2-retrieve-all-employee-information)
3. [Get Specific Columns](#3-get-specific-columns)
4. [Filter by Role](#4-filter-by-role)
5. [Search Employees by Name](#5-search-employees-by-name)
6. [Find Employees Older Than 30 & Earning Above $70,000](#6-find-employees-older-than-30--earning-above-70000)
7. [Update Salary by Employee ID](#7-update-salary-by-employee-id)
8. [Update Address for Sales Role](#8-update-address-for-sales-role)
9. [Remove Employee by ID](#9-remove-employee-by-id)
10. [Delete Employees Under 20 Years](#10-delete-employees-under-20-years)
11. [Insert Multiple Employees](#11-insert-multiple-employees)

---
### Create table for employee
```sql
CREATE TABLE "employee" (
	"id"	INTEGER NOT NULL,
	"name"	TEXT NOT NULL,
	"role"	TEXT,
	"salary"	INTEGER NOT NULL,
	"address"	TEXT,
	"age"	INTEGER NOT NULL,
	"phone"	INTEGER
);
```
---
### 1. Add a New Employee
```sql
INSERT INTO employee (id, name, role, salary, age, address, phone) 
VALUES (55, "Naresh Patil", "Manager", 45000, 20, "Plot 50 Sun Residency Sociret Vapi", 9674589842);
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/5e9c864d-6927-4d4b-80cf-e73c578491c8" height="250">
</p>

---

### 2. Retrieve All Employee Information
```sql
SELECT * FROM employee;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/3da84fc4-d8ff-4db8-b3c4-297736d6e713" height="250">
</p>

---

### 3. Get Specific Columns
Retrieve specific fields like `name` and `salary`:
```sql
SELECT name, salary FROM employee;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/566aa300-018d-4aa4-8f50-497210178cc4" height="250">
</p>

---

### 4. Filter by Role
Find all employees with the role of "Manager":
```sql
SELECT * FROM employee WHERE role = "Manager";
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/ec5cd682-b117-46a7-8640-ffbda97b4e51" height="250">
</p>

---

### 5. Search Employees by Name
Retrieve employees whose names start with "A":
```sql
SELECT * FROM employee WHERE name LIKE "A%";
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/e66ee2e2-b52a-4edc-9bb6-269ed1bedcee" height="250">
</p>

---

### 6. Find Employees Older Than 30 & Earning Above $70,000
```sql
SELECT * FROM employee WHERE age > 30 AND salary > 70000;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/8780a21b-ed05-4d8e-a5b0-442bd043690a" height="250">
</p>

---

### 7. Update Salary by Employee ID
Change the salary of an employee with `id = 100`:
```sql
UPDATE employee SET salary = 65953 WHERE id = 100;
SELECT * FROM employee WHERE id = 100;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/faf27753-af5d-49ff-a065-9ff2c21a37d1" height="250">
</p>

---

### 8. Update Address for Sales Role
Update the address for employees with the "Sales" role:
```sql
UPDATE employee 
SET address = "A 204 RjHans Society Vesu" 
WHERE role = "Sales" AND id = 150;
SELECT * FROM employee WHERE role = "Sales" AND id = 150;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/c8d75e64-0e9e-4881-8fed-618003e5a564" height="250">
</p>

---

### 9. Remove Employee by ID
Remove an employee with `id = 101`:
```sql
DELETE FROM employee WHERE id = 101;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/8ad9f7eb-91c4-4952-944d-a8807f3c4a43" height="250">
</p>

---

### 10. Delete Employees Under 20 Years
Remove all employees with age less than or equal to 20:
```sql
DELETE FROM employee WHERE age <= 20;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/9fab1d2a-ba2f-4a45-8571-cc8176c70851" height="250">
</p>

---

### 11. Insert Multiple Employees
Add multiple employees with selective fields:
```sql
INSERT INTO employee (id, name, salary, age) 
VALUES (205, "Netik Patel", 45000, 25), (659, "Praful Patnecha", 68946, 28);
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/031ec569-b002-403c-afa4-3468950d95ef" height="250">
</p>

---

### 🚀 **Feel free to contribute by adding more SQL queries or use cases!**

--- 

This README is now suitable for GitHub, with images, query examples, and proper formatting! 😊
