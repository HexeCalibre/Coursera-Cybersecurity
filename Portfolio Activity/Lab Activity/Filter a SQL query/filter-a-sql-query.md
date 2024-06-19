# Activity: Filter a SQL query

## Introduction
In this lab, you’ll apply basic filters to SQL queries to retrieve information from a database. You’ll use SQL to get specific information about employees, their machines, and the departments they’re in. You’ll be using the MariaDB shell to run SQL queries.

## Activity overview
As a security analyst, knowing how to make better queries to retrieve specific pieces of data can help you find the security-related information you need more efficiently.

In this lab activity, you’ll apply basic filters to SQL queries to retrieve information from a MariaDB database.

MariaDB is a popular open source relational database that is compatible with MySQL.

This activity provides you with a great opportunity to apply what you’ve learned and add filters to SQL queries.

> ***Note:** The terms **row** and **record** are used interchangeably in this lab activity.*

## Scenario
In this scenario, you need to get specific information about employees, their machines, and the departments they’re in. Your team needs this data to perform various tasks, such as running updates, posting a privacy notice in certain departments, and sending an alert to an employee with an issue on a machine.

You are responsible for finding the required information by querying a database. You’ll add filters to your queries to locate the information more quickly.

Here’s how you’ll do this task: **First**, you’ll list all organization machines and their operating systems. **Second**, you’ll list all machines with the operating system OS 2. **Third**, you’ll list all the employees in the Finance and Sales departments. **Fourth**, you’ll obtain information about machines.

You’re ready to add filters to SQL queries.

## Task 1. List all organization machines
In this task, you need to get a list of all organization machines and their operating systems. The data is contained in the `machines` table. You’ll need to use the `SELECT` keyword to return specific columns.

Run a SQL query to retrieve only the `device_id` and `operating_system` columns from the `machines` table.

## Task 2. Retrieve a list of the machines with OS 2
In this task, you need to obtain a list of all machines with the `'OS 2'` operating system because these machines need an update. To get this information, you’ll run your first SQL query with a filter.

Select all the records from the `machines` table with a value of `'OS 2'` in the `operating_system` column. Replace the value `X` with the correct string:

```SQL
SELECT device_id, operating_system
FROM machines 
WHERE operating_system = 'X';
```

> ***Note:** The WHERE clause allows you to filter the results returned by a query by returning only the records that satisfy the condition.*

## Task 3. List employees in specific departments
In this task, you need to retrieve a list of all the employees in the Finance and Sales departments to obtain their office numbers. A notice about handling confidential financial information will be posted to these offices.

1. Filter the rows returned from `department` column in the `employees` table to include only employees from the `'Finance'` department. Replace `X` with the appropriate column name and `Y` with the appropriate value to complete the filter:

```SQL
SELECT * 
FROM employees 
WHERE X = 'Y';
```

2. Modify the previous query so that it returns employees who are in the `'Sales'` department.

## Task 4. Identify employee machines
Your team recently discovered that there are issues with machines in the South building. In this task, you need to obtain certain employee and computer information.

A machine in `'South-109'` has an issue. You need to determine which employee uses that computer so you can send them an alert.

Write a query to identify which employee uses the office in `'South-109'`. (The data must be returned from the `office` column in the `employees` table.)

Next, your team has determined that there is an issue with all the machines in the South building. Offices in the organization are named with the building name, a hyphen, and the office number in that building (for example, `'South-109'`).

2. Modify the query you used in the previous step so that it returns information on all the employees in the `'South'` building. Use the `LIKE` operator with `%` in this query.

> ***Note:** The `LIKE` keyword in SQL performs simple string matches. The matching pattern may include the wildcard `%` to represent a string of any length. This wildcard may be placed both before and after the targeted substring.*

## Conclusion
Great work!

You now have practical experience in using SQL to

- apply the `WHERE` clause to filter what a SQL query returns and
- use the `LIKE` operator to filter for patterns.

You’re well on your way to running SQL queries to get specific data from a database.