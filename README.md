# Student Management System

A Java-based Student Management System that performs CRUD operations (Create, Read, Update, Delete) using MySQL database integration. This application helps manage student records efficiently through a simple console-based interface.

---

## Features

- Add new student records
- View all students
- Search students by name
- Update student information
- Delete student records
- Input validation and exception handling
- MySQL database connectivity

---

## Technologies Used

- Java
- JDBC
- MySQL
- Object-Oriented Programming (OOP)

---

## Project Structure

```bash
Student-Management-System/
│
├── Student.java
├── StudentManagementSystem.java
├── README.md
└── database.sql
```

---

## Database Setup

### Create Database

```sql
CREATE DATABASE student_management;
```

### Create Table

```sql
USE student_management;

CREATE TABLE students (
    student_id INT PRIMARY KEY,
    name VARCHAR(100),
    birthday DATE,
    email VARCHAR(100)
);
```

---

## Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/Pravalika178/student-management-system.git
cd student-management-system
```

### 2. Configure Database

Update database credentials in `StudentManagementSystem.java`

```java
private static final String URL = "jdbc:mysql://localhost:3306/student_management";
private static final String USER = "root";
private static final String PASSWORD = "your_password";
```

### 3. Add MySQL Connector

Download MySQL Connector/J and add the JAR file to the project build path.

---

## Run the Application

### Compile

```bash
javac Student.java StudentManagementSystem.java
```

### Execute

```bash
java StudentManagementSystem
```

---

## Input Validations

### Student ID
- Must be numeric
- Duplicate IDs are restricted

### Name
- Only letters and spaces allowed

### Birthday
- Format: `YYYY-MM-DD`

### Email
- Must contain valid email format

---

## Exception Handling

- SQL Exception Handling
- InputMismatchException Handling
- User-friendly error messages

---

## Sample Functionalities

- Add Student
- List Students
- Search Student
- Update Student
- Delete Student

---

## Future Enhancements

- GUI using Java Swing
- Authentication system
- Export reports to PDF/Excel
- REST API integration

---

## Author

Developed by Pravalika

GitHub: https://github.com/Pravalika178
---

## License

This project is for educational purposes.