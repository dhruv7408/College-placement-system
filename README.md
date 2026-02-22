#  College Placement Management System

This is a console-based **College Placement Management System** built using **C++ and MySQL**.
The goal of this project is to simplify and automate the campus placement process by managing students, companies, job postings, and applications in one centralized system.

Instead of handling placements manually using spreadsheets or paperwork, this system organizes everything through a structured database and a C++ backend.

---

##  Why I Built This

As a Computer Science student, I wanted to build something practical that reflects a real-world college placement workflow.

This project helped me understand:

* How backend systems interact with databases
* How relational database design works
* How to apply OOP concepts in a real project
* How to manage real-world constraints like eligibility and duplicate applications

## What This System Can Do

### For Students

* Register student details
* View available job drives
* Apply for jobs (based on CGPA eligibility)
* Track application status
* View placement updates

### For Admin / Placement Cell

* Add and manage companies
* Create placement drives
* View applicants for each job
* Update application status (Shortlisted / Selected / Rejected)
* Record final placements

##  Technologies Used

* **C++**

  * Object-Oriented Programming
  * Inheritance & Polymorphism
  * Smart Pointers
  * Exception Handling
* **MySQL**

  * Relational Database Design
  * Foreign Keys & Constraints
  * ENUM for status control
* **MySQL Connector/C++**

  * Secure database connectivity
  * Prepared statements (to prevent SQL injection)
    
## 🗄 Database Design

The system uses the following tables:

* `students`
* `companies`
* `jobs`
* `applications`
* `placements`

Relationships are properly defined using:

* Primary Keys
* Foreign Keys with `ON DELETE CASCADE`
* Unique constraints to prevent duplicate job applications


## How to Run the Project

### Install Requirements

* MySQL Server
* MySQL Connector/C++
* C++ Compiler (g++ / MinGW / MSVC)

###  Setup Database

Run the provided SQL script:

```sql
SOURCE database.sql;
```

###  Update Database Password

In the `DatabaseConfig` class, replace:

```cpp
const string PASSWORD = "your_password";
```

with your actual MySQL password.

### 4️⃣ Compile & Run

Windows:

```bash
g++ main.cpp -o placement_system.exe -lmysqlcppconn
placement_system.exe
```

##  Possible Future Improvements

* Add login authentication for admin & students
* Build a GUI version using Qt
* Convert it into a web-based system
* Add analytics dashboard
* Export reports in CSV/PDF


##  What This Project Demonstrates

* Real-world backend logic implementation
* Strong understanding of OOP in C++
* Clean relational database design
* CRUD operations using prepared statements
* Handling real placement workflow logic

##  About Me

Built by **Dhruv Gupta**
B.Tech Computer Science Student

This project is part of my learning journey toward backend/software development roles .

