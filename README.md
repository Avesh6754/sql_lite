**Create a DBMS for employees...**

- Field names: id, name, role, salary, age, address, phone.

### 1.Add a new employee with all the details

```dart
INSERT INTO employee (id,name,role,salary,age,address,phone) VALUES (55,"Naresh Patil","Manager",45000,20,"Plot 50 Sun Residency sociret Vapi",9674589842)
```

<p>
 

  <img src="https://github.com/user-attachments/assets/5e9c864d-6927-4d4b-80cf-e73c578491c8" Height="35%">
  </p>

### 2.Retrieve all employee information:

```dart
SELECT * From employee
```

<p>
 

  <img src="https://github.com/user-attachments/assets/3da84fc4-d8ff-4db8-b3c4-297736d6e713" Height="35%">
  </p>

  ### 3.Get specific columns for all employees (e.g., name, salary):
  ```dart
SELECT name,salary From employee
```
<p>
  <img src="https://github.com/user-attachments/assets/566aa300-018d-4aa4-8f50-497210178cc4" Height="35%">
  </p>

### 4.Find employees with a particular role (e.g., Manager):

```dart
SELECT * From employee WHERE role="Manager";
```
<p>
  <img src="https://github.com/user-attachments/assets/ec5cd682-b117-46a7-8640-ffbda97b4e51" Height="35%">
</p>


### 5.Search for employees with names containing "An" (case-insensitive):

```dart
SELECT * From employee WHERE name Like "A%";
```
<p>
  <img src="https://github.com/user-attachments/assets/e66ee2e2-b52a-4edc-9bb6-269ed1bedcee" Height="35%">
</p>


### 6.Find employees older than 30 and earning more than $70,000:

```dart
SELECT * From employee WHERE age>30 AND salary>70000;
```
<p>
  <img src="https://github.com/user-attachments/assets/8780a21b-ed05-4d8e-a5b0-442bd043690a" Height="35%">
</p>

### 7.Change the salary of an employee with ID 100::

```dart

UPDATE employee SET salary=65953 WHERE id=100;
SELECT * From employee WHERE id=100;
```
<p>
  <img src="https://github.com/user-attachments/assets/faf27753-af5d-49ff-a065-9ff2c21a37d1" Height="35%">
</p>


### 8.Update the address for employees in the 'Sales' role:

```dart



UPDATE employee SET address="A 204 RjHans Society Vesu" WHERE role="Sales" AND id=150;
SELECT * From employee WHERE role="Sales" AND id=150;
```
<p>
  <img src="https://github.com/user-attachments/assets/c8d75e64-0e9e-4881-8fed-618003e5a564" Height="35%">
</p>

### 9.Remove an employee with ID 101:

```dart
DELETE FROM employee WHERE id=101;
```
<p>
  <img src="https://github.com/user-attachments/assets/8ad9f7eb-91c4-4952-944d-a8807f3c4a43" Height="35%">
</p>



