# Employee Management System

## Overview

The Employee Management System is a C++ console application designed to manage employee records efficiently. It allows administrators to view, add, edit, and delete employee details while ensuring data security through a login system.

## Features

- **List Employees**: Display all employees with their names, IDs, and designations.
- **Show Employee Details**: View detailed information about an employee using their ID.
- **Edit Employee Details**: Modify the designation and CTC of an existing employee.
- **Add New Employee**: Input details to add a new employee record to the database.
- **Delete Employee**: Remove an employee record using their ID.
- **Login System**: Secure access for administrators and new employees.

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/10shivanibm/Employee-Management-System.git
    ```
2. **Navigate to the project directory:**
    ```sh
    cd Employee-Management-System
    ```
3. **Compile the code:**
    ```sh
    g++ -o employee_management_system employee_management_system.cpp
    ```
4. **Run the executable:**
    ```sh
    ./employee_management_system
    ```

## Usage

1. **Start the program:**
   Run the executable file. A login screen will appear.

2. **Login:**
   - For admin access, use the default username `user` and password `1234`.
   - New employees can register by choosing the appropriate option.

3. **Choose an option from the menu:**
   Use the menu to list employees, show details, edit details, add new employees, or delete employees. The main menu options are:
   - `1`: View List of Employees
   - `2`: View Employee Details
   - `3`: Modify Existing Employee Details
   - `4`: Add New Employee Details
   - `5`: Remove an Employee
   - `0`: Exit the application

## Code Structure

- **Class `employee`:** Handles employee data and operations.
  - **Private Variables:**
    - `char name[30]`: Stores the employee's name.
    - `char id[5]`: Stores the employee's ID.
    - `char designation[10]`: Stores the employee's designation.
    - `int age`: Stores the employee's age.
    - `int ctc`: Stores the employee's CTC.
    - `int experience`: Stores the employee's experience.
  - **Private Methods:**
    - `void waitForEnter()`: Utility to pause execution.
    - `void listEmployees()`: Lists all employees.
    - `void showDetails()`: Displays details of a specific employee.
    - `void editExisting()`: Edits details of an employee.
    - `void addNewEmployee()`: Adds a new employee.
    - `void deleteEmployeeDetails()`: Deletes an employee.
  - **Public Methods:**
    - `void options()`: Displays the main menu and handles user input.

- **Function `int login()`:** Manages the login process for admin and new employees.

## Requirements

- **Compiler:** GCC or compatible C++ compiler.
- **OS:** The application is developed for Windows but can be adapted for other operating systems.
