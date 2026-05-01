# HR_PAYROLL-SYSTEM-CAPSTONE-PROJECT-
Inheritance Design

The system implements object-oriented inheritance to model different types of employees.

A base class Employee is created to define shared properties and behavior:

Id
Name
Department
BaseSalary
CalculatePay() method

Two specialized classes inherit from this base class:

1. FullTimeEmployee
Inherits from Employee
Adds:
BonusProperty
Salary Logic:
Monthly salary is calculated as:
BaseSalary + Bonus
2. ContractEmployee
Inherits from Employee
Adds:
HourlyRate
HoursWorked
Salary Logic:
Payment is calculated as:
HourlyRate × HoursWorked
Each derived class provides its own implementation of the CalculatePay() method, enabling polymorphism, where the system can treat all employees uniformly while applying different salary logic internally.


LINQ Usage

LINQ (Language Integrated Query) is used extensively to perform efficient data operations without manual loops.

Key LINQ operations used:
Filtering
Where()

Used to:

Find high earners
Search employees by department
Sorting
OrderBy()
OrderByDescending()

Used to:

Rank employees by salary
Retrieve top earners
Aggregation
Sum()
Average()
Count()

Used to:

Calculate total payroll
Determine average salary
Count employees per department
Projection
Select()

Used to:

Extract specific fields (e.g., names only)
Grouping
GroupBy()

Used to:

Organize employees by department
Generate departmental analytics
Existence Checks
Any()
FirstOrDefault()

Used to:

Validate employee existence before payroll processing
Check if a department has employees

These LINQ methods ensure the system remains efficient, readable, and aligned with best practices, avoiding manual iteration.





Admin Functionality

The system includes an Admin control layer responsible for system-wide analytics and management.

 Access Control
Admin access is protected using an authentication system (AuthService)
Only valid credentials allow access to admin features
Admin Capabilities
Financial Reports
Total Payroll Expenditure
Average Salary
Highest Paid Employee
Top 5 Earners
