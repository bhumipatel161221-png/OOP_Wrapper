# OOP Wrapper – Employee Management System

## Description
A Python console application that demonstrates Object-Oriented Programming (OOP) concepts including classes, inheritance, encapsulation, method overloading, method overriding, `super()`, and `issubclass()`.

## Features
- Create Person, Employee, Manager, and Developer objects.
- Private attributes with getter/setter methods (encapsulation).
- Method overriding in derived classes.
- Simulated method overloading using default arguments.
- Demonstrate `issubclass()` and `isinstance()` checks.
- Constructor and destructor methods.
- Menu-driven interface with input validation.

## Assumptions
- Employee ID is a string (e.g., 'E123').
- Salary is a float.
- Age is an integer.
- Method overloading is simulated using default arguments.
- Data is not persisted to disk.

## Class Hierarchy
Person
└── Employee
├── Manager
└── Developer

## How to Run
1. Ensure Python 3.x is installed.
2. Clone the repository.
3. Run: `python employee_management_system.py`

## Sample Output
(============================================================
Welcome to the Employee Management System!
============================================================
This program demonstrates OOP concepts: classes, inheritance,
encapsulation, method overloading, method overriding, super(),
and issubclass().


==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 1

--- Create a Person ---
Enter Name: bhumi
Enter Age: 21
Person created with name: bhumi and age: 21.

Person created with name: bhumi and age: 21.

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 2

--- Create an Employee ---
Enter Name: bhumi
Enter Age: 21
Enter Employee ID: 1234
Enter Salary: 50,000
Invalid salary. Defaulting to 0.0.
Person created with name: bhumi and age: 21.

Employee created with name: bhumi, age: 21, ID: 1234, and salary: $0.0.

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 3

--- Create a Manager ---
Enter Name: dimple
Enter Age: 20
Enter Employee ID: 3456
Enter Salary: 70000
Enter Department: data analyst
Person created with name: dimple and age: 20.

Manager created with name: dimple, age: 20, ID: 3456, salary: $70000.0, and department: data analyst.

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 4

--- Create a Developer ---
Enter Name: sameer
Enter Age: 24
Enter Employee ID: 5678
Enter Salary: 80000
Enter Programming Language: python, java  
Person created with name: sameer and age: 24.

Developer created with name: sameer, age: 24, ID: 5678, salary: $80000.0, and programming language: python, java.

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 5

--- Show Details ---
Choose details to show:
1. All Objects
2. Persons Only
3. Employees Only
4. Managers Only
5. Developers Only
Enter your choice: 1

----------------------------------------

[Person Details]
Name: bhumi
Age: 21
----------------------------------------

[Employee Details]
Name: bhumi
Age: 21
Employee ID: 1234
Salary: $0.0
----------------------------------------

[Manager Details]
Name: dimple
Age: 20
Employee ID: 3456
Salary: $70000.0
Department: data analyst
----------------------------------------

[Developer Details]
Name: sameer
Age: 24
Employee ID: 5678
Salary: $80000.0
Programming Language: python, java
----------------------------------------

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 5

--- Show Details ---
Choose details to show:
1. All Objects
2. Persons Only
3. Employees Only
4. Managers Only
5. Developers Only
Enter your choice: 1

----------------------------------------

[Person Details]
Name: bhumi
Age: 21
----------------------------------------

[Employee Details]
Name: bhumi
Age: 21
Employee ID: 1234
Salary: $0.0
----------------------------------------

[Manager Details]
Name: dimple
Age: 20
Employee ID: 3456
Salary: $70000.0
Department: data analyst
----------------------------------------

[Developer Details]
Name: sameer
Age: 24
Employee ID: 5678
Salary: $80000.0
Programming Language: python, java
----------------------------------------

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 6

--- OOP Concepts Demonstration ---

1. issubclass() Checks:
   issubclass(Employee, Person)   -> True
   issubclass(Manager, Employee)  -> True
   issubclass(Manager, Person)    -> True
   issubclass(Developer, Employee)-> True
   issubclass(Person, Employee)   -> False

2. Encapsulation Demonstration:
   Employee 'bhumi' salary via getter: $0.0
   After setter (+$5000): $5000.0

3. Method Resolution Order (MRO):
   Manager MRO: ['Manager', 'Employee', 'Person', 'object']
   Developer MRO: ['Developer', 'Employee', 'Person', 'object']

4. isinstance() Checks:
   bhumi: isinstance(obj, Person) = True
   bhumi: isinstance(obj, Person) = True
   dimple: isinstance(obj, Person) = True

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 6

--- OOP Concepts Demonstration ---

1. issubclass() Checks:
   issubclass(Employee, Person)   -> True
   issubclass(Manager, Employee)  -> True
   issubclass(Manager, Person)    -> True
   issubclass(Developer, Employee)-> True
   issubclass(Person, Employee)   -> False

2. Encapsulation Demonstration:
   Employee 'bhumi' salary via getter: $5000.0
   After setter (+$5000): $10000.0

3. Method Resolution Order (MRO):
   Manager MRO: ['Manager', 'Employee', 'Person', 'object']
   Developer MRO: ['Developer', 'Employee', 'Person', 'object']

4. isinstance() Checks:
   bhumi: isinstance(obj, Person) = True
   bhumi: isinstance(obj, Person) = True
   dimple: isinstance(obj, Person) = True

--- Choose another operation ---

==================================================
--- Python OOP Project: Employee Management System ---
==================================================
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Demonstrate OOP Concepts
7. Exit
==================================================
Enter your choice: 7

Exiting the system. All resources have been freed.
Goodbye!
Developer object for sameer has been deleted.
Employee object for sameer has been deleted.
Person object for sameer has been deleted.
Manager object for dimple has been deleted.
Employee object for dimple has been deleted.
Person object for dimple has been deleted.
Employee object for bhumi has been deleted.
Person object for bhumi has been deleted.
Person object for bhumi has been deleted.)

## Author
[Bhumi]
