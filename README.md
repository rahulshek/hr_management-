# 🏢 HR Management System

A command-line based Human Resource Management System built with Python and SQLite. It provides role-based access for **Super Admins**, **HR Managers**, and **Employees** to manage day-to-day HR operations like employee records, attendance, leave, payroll, and reporting.

---

## ✨ Features

### 🔐 Role-Based Access Control
- **Super Admin** – Full system access including user and HR management
- **HR Manager** – Manage employees, attendance, leaves, payroll, and reports
- **Employee** – View personal info, mark attendance, apply for leave, and view payslips

### 👥 Employee Management
- Add, update, and view employee records
- Search employees by ID or department

### 📅 Attendance Tracking
- Mark daily attendance (check-in / check-out)
- View attendance history

### 🏖️ Leave Management
- Apply for leave with reason and dates
- Approve or reject leave requests (HR/Admin)
- View leave history and status

### 💰 Payroll & Salary
- Generate payslips for employees
- Apply salary increments
- View salary reports

### 📊 Reports & Export
- Generate employee reports
- Generate salary reports
- Export data to CSV

### 📝 System Logging
- All key actions are logged to `system_log.txt` for audit purposes

---

## 📁 Project Structure

```
hr_management_system/
│
├── main.py                  # Application entry point & login
│
├── database/
│   ├── connection.py        # SQLite database connection
│   └── setup.py             # Table creation & DB initialization
│
├── models/
│   ├── employee_model.py    # Employee data model
│   ├── attendance_model.py  # Attendance data model
│   └── leave_model.py       # Leave data model
│
├── services/
│   ├── auth_service.py      # Login & authentication logic
│   ├── employee_service.py  # Employee CRUD operations
│   ├── attendance_service.py# Attendance operations
│   ├── leave_service.py     # Leave management logic
│   ├── payroll_service.py   # Payroll & payslip generation
│   └── increment_service.py # Salary increment logic
│
├── menus/
│   ├── superadmin_menu.py   # Super Admin CLI menu
│   ├── hr_menu.py           # HR Manager CLI menu
│   └── employee_menu.py     # Employee CLI menu
│
├── reports/
│   ├── employee_reports.py  # Employee report generation
│   └── salary_reports.py    # Salary report generation
│
├── utils/
│   ├── export_csv.py        # CSV export utility
│   └── logger.py            # System logging utility
│
└── .gitignore
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.x

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/rahulshek/hr_management-.git
   cd hr_management-
   ```

2. **Run the application**
   ```bash
   python main.py
   ```

3. **Login** with your credentials. The system will route you to the appropriate menu based on your role.

---

## 🛠️ Tech Stack

| Technology | Purpose            |
|------------|--------------------|
| Python     | Core language       |
| SQLite     | Database            |
| CSV        | Data export         |

---

## 📌 Notes

- The SQLite database (`hr_system.db`) is auto-created on first run.
- Default credentials must be set up via the Super Admin on initial setup.
- All actions are logged in `system_log.txt`.

---

## 👤 Author

**Rahul Shekh**

---

## 📄 License

This project is for educational purposes.
