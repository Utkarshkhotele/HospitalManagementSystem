# 🏥 Hospital Management System (Java + MySQL)

A simple console-based Hospital Management System built using **Java** and **MySQL**.  
This project allows you to manage patient records efficiently with options to **add** and **view** patients.


---

## 🚀 Features
- Add new patients with details (Name, Age, Gender).
- View all stored patient records.
- Persistent storage using **MySQL database**.
- Simple console menu for interaction.

---


## 🛠️ Technologies Used
- **Java** (JDBC for database connectivity)
- **MySQL** (for storing patient data)
- **JDBC Driver** (Connector/J)

---

## 📂 Database Setup
1. Open MySQL and create a database:
   ```sql
   CREATE DATABASE hospital;
Switch to the database:

sql
Copy code
USE hospital;
Create a table:

sql
Copy code
CREATE TABLE patients (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    age INT NOT NULL,
    gender VARCHAR(10) NOT NULL
);
▶️ How to Run
Install and run MySQL Server.

Update your database credentials inside the Java file (DB URL, username, password).

Compile the Java program:

bash
Copy code
javac HospitalManagement.java
Run the program:

bash
Copy code
java HospitalManagement
📋 Example Usage
mathematica
Copy code
====== Hospital Management System ======
1. Add Patient
2. View Patients
3. Exit
Enter your choice: 1
Enter name: John Doe
Enter age: 25
Enter gender: Male
✅ Patient added successfully!

Enter your choice: 2
ID | Name     | Age | Gender
1  | John Doe | 25  | Male
💡 Notes
Patients remain stored even after you exit the program (data is stored in MySQL).

You can view them anytime by selecting option 2 (View Patients).

Make sure MySQL server is running before starting the program.
