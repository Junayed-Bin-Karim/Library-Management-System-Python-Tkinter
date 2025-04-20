Library Management System (Python Tkinter)



A simple Library Management System built using Python's Tkinter for the GUI and PyMySQL for MySQL database interaction. This system allows librarians and students to manage books and borrowing activities efficiently.

Table of Contents
Features

Prerequisites

Installation

Database Setup

Usage

Contributing

License

Contact

Features
Student/Librarian Functionalities:

Login: Secure login for both students and librarians

Donate Book: Add new books to the database

Apply Book: Request to borrow available books

Return Book: Return borrowed books (late returns may include penalties)

View Books: View all books available in the library

Applied Books: Check currently borrowed books

Logout: Safely logout of the session

Admin Functionalities (use "admin" credentials):

Add Student: Register new students

View Students: Display a list of all registered students

Delete Student: Remove a student account

Add Book (Admin): Add books from the admin panel

View Books (Admin): View books from the admin perspective

Delete Book: Remove books from the database

Logout (Admin): Securely log out of the admin panel

Prerequisites
Make sure the following dependencies are installed:

Python 3.x
Download from python.org

PyMySQL
Install using pip:

bash
Copy
Edit
pip install pymysql
MySQL Server
A running MySQL instance is required. You can download it from the MySQL official site.

Installation
Clone the Repository (if available on GitHub):

bash
Copy
Edit
git clone [repository URL]
cd [project directory]
Save the Application Code:
Save the provided code as library_app.py.

Database Setup
Create the Database:
Open your MySQL client (Workbench or CLI) and execute:

sql
Copy
Edit
CREATE DATABASE IF NOT EXISTS Library;
User Credentials:
The script connects using:

Username: root

Password: (empty)

Note: For production, create a dedicated user with proper permissions. Update the connectdb() function in the Python script if your credentials differ.

Table Creation:
When you run the app, it will automatically create required tables:

Login

Book

BookIssue

Usage
Run the App:

bash
Copy
Edit
python library_app.py
Login Screen:

Student Login: Use your student ID and password (added by admin)

Admin Login: Use credentials admin / admin

Navigate:
Use the buttons to manage books, apply/return, and more.

Contributing
Contributions are welcome. To contribute:

Fork the repository

Create a new branch

Make your changes

Push to your fork

Submit a pull request

License
This project is licensed under the MIT License.

Contact
If you have questions, feedback, or need assistance, feel free to reach out:
[Add your email or GitHub profile link here]
