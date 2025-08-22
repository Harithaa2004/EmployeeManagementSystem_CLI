# Employee Attendance Management System

A **Java CLI (Command-Line Interface)** application to manage employees and track their attendance.
This project demonstrates **Object-Oriented Programming (OOP)** concepts such as encapsulation, inheritance, abstraction, enums, validation, and data handling.

---

##  Features

*  **Employee Management**

  * Add employees (with auto-generated IDs like `E001`, `E002`)
  * List all employees
  * Delete employees

* ⏱ **Attendance Tracking**

  * Record **Check-In** and **Check-Out**
  * Prevent duplicate or invalid check-ins/check-outs
  * Filter attendance by **Employee ID** or **Date**
  * View summary of **working hours** for each employee

* 🛠 **Utility Features**

  * Simple menu-based CLI
  * Data validation
  * Role and Department defined using **Enums**

---

##  Project Structure

```
src/
 ├── app/
 │   ├── Employee.java
 │   ├── EmployeeList.java
 │   ├── Attendance.java
 │   ├── AttendanceList.java
 │   ├── EmployeeManager.java
 │   └── Main.java
```

* **Employee.java** → Defines employee details (ID, name, role, department)
* **EmployeeList.java** → Custom list to manage employees
* **Attendance.java** → Represents a single attendance record
* **AttendanceList.java** → Handles all attendance records and validation
* **EmployeeManager.java** → Coordinates employees + attendance logic
* **Main.java** → CLI entry point with interactive menu

---

### Prerequisites

* Install [Java 17+](https://adoptopenjdk.net/)

### Compile and Run

1. Clone this repository or copy the source files.

2. Open a terminal and navigate to the project folder.

3. Compile all `.java` files:

   ```bash
   javac src/app/*.java -d out
   ```

4. Run the program:

   ```bash
   java -cp out app.Main
   ```

---

##  Sample Menu

```
=== Employee Attendance Management ===
1. Add Employee
2. List Employees
3. Check In
4. Check Out
5. Filter Attendance
6. Delete Employee
7. Working Hours Summary
0. Exit
```

---

##  Example Usage

1. Add employee:

   * Input: First Name, Last Name, Role, Department
   * Auto-ID assigned: `E001`

2. Record Attendance:

   * Choose `Check In` → System records current time
   * Choose `Check Out` → System records end time and calculates duration

3. Filter Attendance:

   * By **Employee ID** → Show all records of one employee
   * By **Date** → Show all employees who worked on that date

---

##  Future Enhancements

* 🔒 Persist data in files (CSV/JSON) or database (SQLite/MySQL)
* 📊 Generate monthly reports
* 🌐 Add a **REST API** with Spring Boot
* 🎨 Create a GUI with JavaFX

---


Developed as a learning project to practice **Java OOP, Collections, and CLI app development**.

---

