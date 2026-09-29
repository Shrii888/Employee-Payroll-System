# Employee Payroll System

A Python-based **Employee Payroll System** built as a menu-driven application to manage employee records, calculate salaries, generate payslips, search employees, and save payroll data using JSON.

## 📌 Project Overview

This project demonstrates how Python can be used to automate basic employee payroll management.

The system stores employee information in a JSON file and provides functions for:

- Adding employees
- Updating an employee's name
- Calculating gross and net salary
- Generating payslips
- Searching employee records
- Saving payroll data
- Running the system through a menu-driven interface

## 🖼️ Project Preview

The notebook includes a project infographic showing the main features and workflow of the Employee Payroll System.

## ✨ Features

### 1. Add Employee

The system collects:

- Employee ID
- Employee Name
- Department
- Basic Salary
- Allowances
- Deductions

Each employee is stored as a dictionary inside the `employees` list.

The system also checks for duplicate Employee IDs and prevents negative salary-related values.

### 2. Save Payroll Records

Employee records are saved in:

```text
payroll.json
```

The project uses Python's built-in `json` module.

Records are saved using:

```python
json.dump(employees, file, indent=4)
```

The program also attempts to load existing records when it starts. If `payroll.json` does not exist, an empty employee list is created.

### 3. Update Employee Name

The project includes an `update_employee()` function that allows an employee's name to be corrected using their Employee ID.

This was useful for handling incorrect employee information without creating a duplicate employee record.

### 4. Calculate Salary

Salary is calculated using:

**Gross Salary = Basic Salary + Allowances**

**Net Salary = Gross Salary - Deductions**

The calculated values are stored in the employee record as:

```text
gross_salary
net_salary
```

### 5. Generate Payslip

The `generate_payslip()` function creates a formatted payslip containing:

- Employee ID
- Name
- Department
- Basic Salary
- Allowances
- Gross Salary
- Deductions
- Net Salary

The function also calculates and stores gross and net salary before displaying the payslip.

### 6. Search Employee

Employees can be searched using their Employee ID.

The search function displays employee details and, when available, gross and net salary.

### 7. Menu-Driven System

The final application is controlled through a simple menu:

```text
========================================
       EMPLOYEE PAYROLL SYSTEM
========================================

1. Add Employee
2. Calculate Salary
3. Generate Payslip
4. Search Employee
5. Save Payroll Data
6. Exit
```

The menu continues running until the user selects **Exit**.

## 🛠️ Technologies Used

- **Python**
- **JSON**
- **File Handling**
- **Functions**
- **Lists**
- **Dictionaries**
- **Loops**
- **Conditional Statements**
- **Input Handling**

## 📂 Project Structure

```text
Employee-Payroll-System/
│
├── Project_4_Employee.ipynb
├── payroll.json
├── README.md
└── project-image.png
```

> The exact image filename can be changed to match the image stored in the project folder.

## 🔄 Project Workflow

```text
Start
  ↓
Load payroll.json
  ↓
Display Employee Payroll Menu
  ↓
Choose an Operation
  ↓
Add / Calculate / Payslip / Search
  ↓
Update Employee Records
  ↓
Save Data to payroll.json
  ↓
Continue or Exit
```

## 💾 Sample Employee Record

The stored JSON structure follows this format:

```json
{
    "employee_id": 1005,
    "name": "Nancy Singh",
    "department": "Auditing",
    "basic_salary": 25000.0,
    "allowances": 4500.0,
    "deductions": 2000.0,
    "gross_salary": 29500.0,
    "net_salary": 27500.0
}
```

## 🧮 Salary Calculation Example

Suppose an employee has:

```text
Basic Salary = ₹25,000
Allowances   = ₹4,500
Deductions   = ₹2,000
```

Then:

```text
Gross Salary = ₹25,000 + ₹4,500
             = ₹29,500

Net Salary   = ₹29,500 - ₹2,000
             = ₹27,500
```

## 🎯 Learning Outcomes

Through this project, I practiced:

- Working with JSON data
- Reading and writing files
- Creating reusable Python functions
- Working with lists and dictionaries
- Searching records using loops
- Performing salary calculations
- Updating stored records
- Building formatted console output
- Creating a menu-driven Python application
- Managing persistent employee data

## 💼 Business Use Case

A payroll system helps an organization maintain employee salary information in a structured way.

This project demonstrates the basic logic behind:

- Employee record management
- Salary computation
- Payslip generation
- Employee lookup
- Payroll data storage

It is a learning project rather than a production payroll system, but it demonstrates how Python can automate repetitive payroll-related tasks.

## 🚀 Future Improvements

Possible future enhancements include:

- Update complete employee records
- Delete employee records
- More robust input validation
- Tax and PF calculations
- Attendance-based salary calculation
- Monthly payroll reports
- Export payslips to PDF
- GUI using Tkinter
- Database integration using MySQL

## 👩‍💻 Author

**Shrii**
Shriya Verma


Aspiring Data Analyst  | Data Analytics with Generative AI | August Batch
Python | SQL | Excel | Power BI

