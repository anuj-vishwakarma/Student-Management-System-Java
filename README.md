# Student Management System (JavaFX + MySQL)

A modern desktop-based **Student Management System** developed using **JavaFX**, **Scene Builder**, **JDBC**, and **MySQL**.  
This application provides an easy-to-use graphical interface for managing student records efficiently with full CRUD functionality and database integration.

---

# Features

- User Registration & Login
- Secure Authentication using JDBC
- Add Student Records
- Update Existing Student Information
- Delete Student Records
- View All Students
- Search Students
- Responsive JavaFX UI
- CSS Styled Interface
- MySQL Database Connectivity
- Modular Project Structure

---

# Tech Stack

| Technology | Purpose |
|---|---|
| Java | Core Programming Language |
| JavaFX | GUI Framework |
| Scene Builder | UI Design |
| CSS | UI Styling |
| JDBC | Database Connectivity |
| MySQL | Database Management System |

---

# Project Structure

```bash
Student-Management-System-Java/
│
├── src/
│   ├── application/
│   ├── controller/
│   ├── model/
│   ├── database/
│   ├── view/
│   └── css/
│
├── lib/
├── database/
├── README.md
└── pom.xml / build files
```

---

# Screenshots

## Login Page

- User authentication system
- Credential validation
- JavaFX-based responsive UI

## Dashboard

- Student management panel
- Navigation system
- TableView integration

## Student Management

- Add students
- Edit student information
- Delete student records
- Search functionality

---

# Functionalities

## 1. User Authentication

The system allows users to:

- Register a new account
- Login using credentials
- Validate credentials using MySQL database

### Technologies Used

- JDBC
- PreparedStatement
- MySQL

---

## 2. Add Student

Users can add student information such as:

- Student ID
- Name
- Email
- Course
- Phone Number
- Address

### Database Operation

```sql
INSERT INTO students VALUES (?, ?, ?, ?, ?, ?);
```

---

## 3. View Students

Displays all students in a JavaFX `TableView`.

### Features

- Dynamic data loading
- ObservableList support
- Clean UI representation

---

## 4. Update Student

Allows modification of existing student details.

### Database Operation

```sql
UPDATE students
SET name=?, email=?, course=?
WHERE student_id=?;
```

---

## 5. Delete Student

Removes student records permanently from the database.

### Database Operation

```sql
DELETE FROM students WHERE student_id=?;
```

---

## 6. Search Student

Search students by:

- Student ID
- Name
- Course

---

# Database Design

## Users Table

```sql
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(100),
    password VARCHAR(100)
);
```

---

## Students Table

```sql
CREATE TABLE students (
    student_id INT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    course VARCHAR(100),
    phone VARCHAR(20),
    address VARCHAR(255)
);
```

---

# Installation & Setup

## Prerequisites

Make sure you have installed:

- Java JDK 17+ (or compatible version)
- JavaFX SDK
- MySQL Server
- Scene Builder (Optional)
- IDE (IntelliJ IDEA / Eclipse / NetBeans)

---

# Clone the Repository

```bash
git clone https://github.com/anuj-vishwakarma/Student-Management-System-Java.git
```

---

# Database Setup

## Step 1: Create Database

```sql
CREATE DATABASE student_management_system;
```

---

## Step 2: Use Database

```sql
USE student_management_system;
```

---

## Step 3: Create Tables

Run the SQL queries mentioned above.

---

# Configure JDBC Connection

Update your database credentials inside the database connection file.

Example:

```java
String url = "jdbc:mysql://localhost:3306/student_management_system";
String username = "root";
String password = "your_password";
```

---

# Run the Project

1. Open the project in your IDE
2. Configure JavaFX SDK
3. Add MySQL JDBC Connector
4. Run the main JavaFX application file

---

# Concepts Used

This project demonstrates understanding of:

- Object-Oriented Programming (OOP)
- Event-Driven Programming
- JavaFX Architecture
- JDBC Connectivity
- SQL Queries
- CRUD Operations
- MVC Design Pattern
- UI/UX Design
- Database Management

---

# Future Improvements

Some features that can be added in future versions:

- Password Encryption
- Attendance Management
- Role-Based Authentication
- Export to PDF/Excel
- Dashboard Analytics
- Email Notifications
- Pagination
- Student Profile Photos
- Cloud Database Support

---

# Advantages of the Project

- Beginner-Friendly Java Project
- Real Database Integration
- Modern JavaFX UI
- Good for Resume & College Projects
- Demonstrates Full Stack Java Concepts

---

# Learning Outcomes

By building this project, you can learn:

- JavaFX Development
- Database Connectivity with JDBC
- SQL Operations
- Desktop Application Development
- MVC Architecture
- Java Event Handling
- UI Styling using CSS

---

# Interview Topics Covered

This project helps prepare for interview questions on:

- JavaFX
- JDBC
- MySQL
- OOP Concepts
- CRUD Operations
- MVC Architecture
- SQL Queries
- Exception Handling

---

# Author

## Anuj Vishwakarma

- GitHub: https://github.com/anuj-vishwakarma

---

# License

This project is open-source and available for educational purposes.

---

# Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create a new branch
3. Commit changes
4. Push the branch
5. Create a Pull Request

---

# Support

If you found this project helpful, consider giving it a ⭐ on GitHub.

---
