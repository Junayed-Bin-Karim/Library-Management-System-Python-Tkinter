# Library Management System (Python Tkinter)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)

This is a simple Library Management System built using Python's Tkinter library for the graphical user interface and PyMySQL for database interaction. It allows librarians and students to manage books and borrowing activities.

---

## Table of Contents

- [Features](#features)  
- [Prerequisites](#prerequisites)  
- [Installation](#installation)  
- [Database Setup](#database-setup)  
- [Usage](#usage)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## Features

**Student/Librarian Functionalities:**

- **Login:** Secure login for both students and librarians  
- **Donate Book:** Add new books to the database  
- **Apply Book:** Request to borrow available books  
- **Return Book:** Return borrowed books (late returns may include penalties)  
- **View Books:** View all books available in the library  
- **Applied Books:** Check currently borrowed books  
- **Logout:** Safely logout of the session  

**Admin Functionalities (use "admin" credentials):**

- **Add Student:** Register new students  
- **View Students:** Display a list of all registered students  
- **Delete Student:** Remove a student account  
- **Add Book (Admin):** Add books from the admin panel  
- **View Books (Admin):** View books from the admin perspective  
- **Delete Book:** Remove books from the database  
- **Logout (Admin):** Securely log out of the admin panel  

---

## Prerequisites

Make sure the following dependencies are installed:

- **Python 3.x**  
  [Download from python.org](https://www.python.org/downloads/)

- **PyMySQL**  
  Install using pip:  
  ```bash
  pip install pymysql
## MySQL Server

A running MySQL instance is required. You can download it from the [MySQL official site](https://dev.mysql.com/downloads/).

---

## Installation

### Clone the Repository:
```bash
git clone [git@github.com:Junayed-Bin-Karim/Library-Management-System-Python-Tkinter.git]
```
Save the Application Code:
Save the provided code as library_app.py.

Database Setup
Create the Database:
Open your MySQL client (Workbench or CLI) and execute:

## sql

CREATE DATABASE IF NOT EXISTS Library;
User Credentials:
The script connects using:

Username: root

Password: (empty)

Note: For production, create a dedicated user with proper permissions.
Update the connectdb() function in the Python script if your credentials differ.

## Table Creation:
When you run the app, it will automatically create the required tables:

Login

Book

BookIssue

Usage

### Run the App:
python library_app.py
Login Screen:
Student Login: Use your Student ID and Password (added by admin)

Admin Login: Use credentials admin / admin

Navigate:
Use the buttons to manage books, apply/return books, and more.

###   Contributing
Contributions are welcome. To contribute:

Fork the repository

Create a new branch

Make your changes

Push to your fork

Submit a pull request


### Contact
If you have questions, feedback, or need assistance, feel free to reach out:

GitHub: https://github.com/Junayed-Bin-Karim

LinkedIn: https://www.linkedin.com/in/junayed-bin-karim-47b755270/
