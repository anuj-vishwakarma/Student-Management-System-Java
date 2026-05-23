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

  <img width="977" height="586" alt="image" src="https://github.com/user-attachments/assets/fadc7a2b-cf42-4ac7-bca1-570cb34f99bd" />
## Signup Page
- User creation system
- Credential storage in hash form
  <img width="987" height="588" alt="image" src="https://github.com/user-attachments/assets/3930002d-b334-4a17-bb70-0e1addf421f0" />


## Dashboard

- Student management panel
- Navigation system
- TableView integration

  <img width="1090" height="597" alt="image" src="https://github.com/user-attachments/assets/564b4d64-db7b-46ce-880b-8feb8919d555" />

## Student Management

- Add students

  <img width="1093" height="601" alt="image" src="https://github.com/user-attachments/assets/516e5222-5f73-43e9-846c-c26048085012" />

- Course

  <img width="1087" height="590" alt="image" src="https://github.com/user-attachments/assets/e17c00d7-f581-4a0f-9311-00b907e4aa41" />

- Grades of Students

  <img width="1096" height="596" alt="image" src="https://github.com/user-attachments/assets/f4c72d20-e8b6-40e6-9d00-9f5b31b1e8f1" />

- Attendance System

  <img width="1091" height="597" alt="image" src="https://github.com/user-attachments/assets/9462aa8f-d862-4f01-8627-912755373148" />

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
