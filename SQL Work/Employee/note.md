SELECT FirstName, LastName FROM employee WHERE City = 'Calgary';
SELECT FirstName, LastName, max(BirthDate) FROM Employee;
SELECT FirstName, LastName, min(BirthDate) FROM Employee;

///Query employee to find Nancy Edwards ID\\\
SELECT * FROM Employee;
SELECT * FROM Employee WHERE ReportsTo = 2;
SELECT COUNT (*) FROM Employee WHere City = 'Lethbridge'; 

