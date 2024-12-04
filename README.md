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













