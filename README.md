# Employee Management Console Application

This project is a simple Java console-based Employee Management Application that demonstrates basic CRUD (Create, Read, Update, Delete) operations using an in-memory storage (ArrayList). The application lets you add, search, update, and delete employee records through a menu-driven interface.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Setup and Running the Application](#setup-and-running-the-application)
- [Future Enhancements](#future-enhancements)
- [License](#license)
- [Contact](#contact)

## Overview

The application is organized into multiple packages:
- **Entity**: Contains the `Employee` class (a Plain Old Java Object) that represents an employee.
- **service**: Declares the `EmployeeService` interface with the common CRUD operations.
- **serviceimpl**: Implements the `EmployeeService` interface in `EmployeeServiceImpl` using an `ArrayList` to store employee data.
- **app**: Contains the main class (`EmployeeApp`) that drives the console-based menu.

## Features

- **Add Employee:** Input employee details and add a new employee to the list.
- **Get Employee by ID:** Search for and display an employee based on their ID.
- **Get Employee by Salary:** Search for an employee with a specified salary.
- **Update Employee:** Update employee attributes (name, salary, age, designation, or phone number) based on ID.
- **Remove Employee:** Delete an employee record using the employee ID.
- **Display All Employees:** List details of all employees.

## Project Structure

Below is a neat diagram of the project structure:

```plaintext
.
├── Entity
│   └── Employee.java           // Employee POJO with attributes (ename, eid, phoneno, esal, eage, edesgn)
├── service
│   └── EmployeeService.java    // Interface defining CRUD operations
├── serviceimpl
│   └── EmployeeServiceImpl.java// Implementation of EmployeeService using an ArrayList
└── app
    └── EmployeeApp.java        // Main class with the console menu for user interaction
  ```


## Prerequisites

- Java JDK 8 or higher
- An IDE (such as IntelliJ IDEA, Eclipse, or VSCode) or a command-line environment for compiling and running Java applications

## Setup and Running the Application

1. **Clone the Repository:**
   
```bash
   git clone  https://github.com/maruthicharanteja10/EmployeeManagementApplicationUsingCoreJava
   cd EmployeeManagementApp
   ```

2. **Compile the Project:**

   If you are using the command line, navigate to the project root and compile the classes. For example:

   ```bash
   javac -d bin Entity/Employee.java service/EmployeeService.java serviceimpl/EmployeeServiceImpl.java app/EmployeeApp.java
   ```
   
   *(Make sure to adjust the classpath separator if you're on Unix-based systems by replacing `;` with `:`.)*

3. **Run the Application:**

   Navigate to the output directory (e.g., `bin`) and run the main class:

   ```bash
   java app.EmployeeApp
   ```

   The console menu will appear. Follow the on-screen instructions to add, search, update, or delete employee records.

## Future Enhancements

- **Persistence:** Integrate a database to store employee data persistently.
- **Input Validation:** Add robust input validation to improve reliability.
- **Enhanced Error Handling:** Provide more user-friendly error messages and logging.
- **Graphical User Interface (GUI):** Develop a GUI for a more interactive user experience.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For questions or feedback, please contact:

- **Email:** [charantejdonthireddy@gmail.com](mailto:charantejdonthireddy@gmail.com)
```
