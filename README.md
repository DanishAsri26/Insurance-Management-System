# 🛡️ Insurance Management System (Python)

This is a comprehensive, console-based application built in Python for managing an insurance system. It supports multiple user roles (Admin, Agent, and Customer) and utilizes an SQLite database to handle policy data, user accounts, and transactions.

The system is designed with a clear object-oriented approach, making the codebase modular, scalable, and easy to maintain.

## ✨ Features

The system offers distinct functionalities based on the logged-in user role:

### 1. 🔑 User Management & Roles
* **Three distinct roles:** Admin, Agent, and Customer.
* Secure login and registration for each user type.
* Role-based access control (e.g., only Agents can add new policies, only Admins can manage agents).

### 2. 📝 Policy Management (Admin/Agent)
* **Add/Create Policies:** Agents can register new insurance policies with details like policy ID, type, premium, and coverage.
* **View Policies:** Agents and Customers can view policy details.
* **Search/Filter:** Efficiently search for policies based on various criteria.

### 3. 👤 Customer Management
* Customers can view their owned policies, check premium status, and update their personal information.

### 4. 📊 Database Backend
* Uses **SQLite** for reliable and lightweight data storage.
* The system initializes the database and required tables automatically upon first run.

## 📁 Project Structure

The project is divided into logical components based on responsibility and user roles:

| File Name | Description |
| :--- | :--- |
| `main.py` | **The entry point of the application.** Contains the main menu and handles user role selection and login/registration flow. |
| `admin.py` | Logic and functions specific to the **Admin** role (e.g., managing agents, system reports). |
| `agent.py` | Logic and functions specific to the **Agent** role (e.g., adding/modifying policies, managing customer records). |
| `customer.py` | Logic and functions specific to the **Customer** role (e.g., viewing policies, updating profile). |
| `Insurance_class.py` | Defines the **data models** (classes) for Policy, Customer, Agent, and Admin, enforcing object-oriented principles. |
| `database_setup.py` | **Database initialization script.** Handles connecting to SQLite and creating all necessary tables (Users, Policies, etc.). |

## 🛠️ Prerequisites

To run this application, you need the following:

* **Python:** Version 3.x (Recommended)
* **Python Libraries:**
    * `sqlite3` (usually included with Python standard library)
    * Any other standard libraries used for date/time or specific console formatting (check source code if dependencies were added).

## 🚀 How to Run the System

### 1. Clone the Repository

```bash
git clone [https://github.com/YourUsername/RepoName.git](https://github.com/YourUsername/RepoName.git)
cd RepoName
