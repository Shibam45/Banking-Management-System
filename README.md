# 🏦 Banking Management System

A console-based Banking Management System developed using **Java, JDBC, and MySQL**. This project demonstrates core object-oriented programming concepts and database connectivity through essential banking operations, including user registration, account creation, deposits, withdrawals, fund transfers, and balance inquiries.

## 📌 Project Overview

The Banking Management System allows users to register and log in, open a bank account, and perform basic financial operations through a menu-driven command-line interface.

The application uses Java for business logic and JDBC to interact with a MySQL database, enabling account and user information to be stored and retrieved.

## ✨ Features

- **User Registration:** Register users with their full name, email address, and password.
- **User Authentication:** Log in using registered email credentials.
- **Bank Account Creation:** Create a bank account with an account number, account holder's name, initial balance, and security PIN.
- **Deposit Money:** Credit money to an account after security PIN verification.
- **Withdraw Money:** Debit money from an account while checking the available balance.
- **Fund Transfer:** Transfer money between bank accounts.
- **Balance Inquiry:** Check the current account balance after PIN verification.
- **MySQL Database Integration:** Store and retrieve user and account information.
- **Transaction Consistency:** Use JDBC transaction controls, including commit and rollback, for banking operations.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Java | Core application logic and object-oriented programming |
| JDBC | Database connectivity and SQL execution |
| MySQL | Persistent storage for users and bank accounts |
| MySQL Connector/J | JDBC driver for connecting Java to MySQL |
| IntelliJ IDEA | Development environment |
| Git & GitHub | Version control and project hosting |

## 🏗️ Application Architecture

The application separates its main responsibilities across four Java classes.

| Class | Responsibility |
|---|---|
| `BankingApp.java` | Application entry point, database connection, main menu, and navigation |
| `User.java` | User registration, login, and duplicate-email checks |
| `Accounts.java` | Account creation, account number generation, and account lookup |
| `AccountManager.java` | Deposits, withdrawals, fund transfers, and balance inquiries |

### Application Workflow

1. The application establishes a connection to MySQL through JDBC.
2. The user registers or logs in.
3. A logged-in user can create a bank account if one does not already exist.
4. The application displays a banking menu.
5. The user selects a banking operation and provides the required information.
6. The application executes SQL queries and updates the database.
7. The result of the operation is displayed in the console.

## 📂 Project Structure

```text
Banking-Management-System/
│
├── src/
│   └── BankingManagementSystem/
│       ├── BankingApp.java
│       ├── User.java
│       ├── Accounts.java
│       └── AccountManager.java
│
├── .idea/
├── .gitignore
├── Banking Management System.iml
└── README.md
```

The application starts with the following menu:

```text
*** WELCOME TO BANKING SYSTEM ***

1. Register
2. Login
3. Exit
```

After successful login, users can access the available banking operations.

## 💻 Banking Operations

The logged-in user is presented with the following menu:

```text
1. Debit Money
2. Credit Money
3. Transfer Money
4. Check Balance
5. Log Out
```

- **Debit Money:** Withdraws money after checking the security PIN and available balance.
- **Credit Money:** Adds money to the account after PIN verification.
- **Transfer Money:** Transfers funds from the sender's account to the recipient's account.
- **Check Balance:** Displays the account balance after PIN verification.
- **Log Out:** Returns the user to the main application menu.

## 🧠 Key Concepts Demonstrated

This project provides practical experience with:

- Object-oriented programming and class design
- Constructors, methods, and encapsulation
- Java exception handling
- JDBC database connectivity
- SQL queries and prepared statements
- CRUD-related database operations
- Authentication and input validation
- Database transaction management using commit and rollback
- Separation of application responsibilities across classes

## 🔐 Security Considerations

This is an educational project and is **not intended for real banking transactions**.

Before extending it for production use, consider the following improvements:

- Store passwords using a secure password-hashing algorithm.
- Never hardcode or commit database credentials.
- Validate that transaction amounts are positive and within permitted limits.
- Validate recipient accounts before processing transfers.
- Use database transactions with reliable rollback and cleanup handling.
- Add transaction history and audit logging.
- Improve exception handling and avoid exposing database errors to users.
- Use appropriate authentication, authorization, and account-protection mechanisms.

## 🔮 Future Enhancements

Potential improvements include:

- A graphical user interface using Java Swing or JavaFX.
- Transaction history and account statements.
- Improved input validation and error handling.
- JUnit tests for banking operations.
- Maven-based dependency management.
- Secure password hashing and credential management.
- Support for multiple accounts per user.
- Administrative functionality and reporting.

## 🎯 Learning Outcomes

Through this project, developers can explore how Java applications interact with relational databases and how object-oriented design can organize real-world workflows such as account creation, balance management, and fund transfers.


