# Library Management System (Python Tkinter)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)

This is a simple Library Management System built using Python's Tkinter library for the graphical user interface and PyMySQL for database interaction. It allows librarians and students to manage books and borrowing activities.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Database Setup](#database-setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

This application provides the following functionalities:

**Student/Librarian Features:**

- **Login:** Secure login for both students and librarians.
- **Donate Book:** Librarians can add new books to the library database.
- **Apply Book:** Students can request to borrow available books.
- **Return Book:** Students can return borrowed books. Late returns might have penalties (as indicated in the code).
- **View Books:** Students and librarians can view all available books in the library.
- **Applied Books:** Students can view the books they have currently borrowed.
- **Logout:** Securely log out of the system.

**Admin Features (Accessible with "admin" credentials):**

- **Add Student:** Add new student accounts to the system.
- **View Students:** View a list of all registered students.
- **Delete Student:** Remove student accounts from the system.
- **Add Book (Admin):** Similar to "Donate Book" but accessible via admin panel.
- **View Books (Admin):** Similar to student/librarian view.
- **Delete Book:** Remove books from the library database.
- **Logout (Admin):** Securely log out of the admin panel.

## Prerequisites

Before running the application, ensure you have the following installed:

- **Python 3.x:** Download from [python.org](https://www.python.org/downloads/).
- **PyMySQL:** Install using pip:
  ```bash
  pip install pymysql
  ```
  MySQL Server: You need a running MySQL server instance. You can download it from MySQL Downloads.
Installation
Clone the repository (if you have one on GitHub):
Bash

git clone [repository URL]
cd [project directory name]
Save the provided Python code: Save the code you provided as a Python file (e.g., library_app.py).
Database Setup
Create a database: Connect to your MySQL server using a MySQL client (like MySQL Workbench or the command line) and create a database named Library:
SQL

CREATE DATABASE IF NOT EXISTS Library;
User Credentials: The script attempts to connect to MySQL using the username root and an empty password (passwd=""). It is highly recommended to set up a dedicated user with appropriate permissions for this application in a production environment. You'll need to modify the connectdb() function in the Python script with your MySQL server details if they are different.
Table Creation: The script automatically creates the necessary tables (Login, Book, and BookIssue) if they don't exist when the connectdb() function is called for the first time.
Usage
Run the Python script: Navigate to the directory where you saved the library_app.py file in your terminal and run:
Bash

python library_app.py
Login: The main window will appear, prompting you to log in as either a "STUDENT" or "ADMIN".
Student Login: Enter your Student ID and Password (which would have been added by an admin).
Admin Login: Use the credentials "admin" for both User ID and Password.
Navigate the application: Use the buttons in the subsequent windows to perform the desired actions.
Contributing
Contributions to this project are welcome. If you find any bugs or have suggestions for improvements, feel free to:   

Fork the repository.
Create a new branch for your feature or bug fix.
Make your changes and commit them.   
Push your changes to your fork.
Submit a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for more details.   

Contact
If you have any questions or issues, feel free to [add your contact information here, e.g., email address or GitHub profile link].
