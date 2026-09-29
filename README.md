# 🏦 Bank Management System – Java

This is a **Bank Management System** developed using **Java and Object-Oriented Programming (OOP)** concepts.
The system allows users to create and manage bank accounts, perform financial transactions, request loans, calculate interest, and store account information in a file.

This project was developed as part of the **Object Oriented Programming II: Java (CSE 201)** course at the **University of Asia Pacific**.

---

## 📌 Project Overview

The Bank Management System provides a simple console-based banking environment where users can:

* Create a bank account
* Login using account number and password
* Deposit money
* Withdraw money
* Transfer money between accounts
* Request a loan
* Check account balance
* Calculate interest for deposit accounts
* Close an account
* Save and load account information from a file

The system supports two types of accounts: **Current Account** and **Deposit Account**.

---

## 🛠️ Technologies Used

* Java
* Object-Oriented Programming (OOP)
* Java Collections
* File Handling
* Exception Handling
* `ArrayList`
* `Scanner`
* `FileWriter`

---

## 📂 Project Structure

```text
BankManagementSystem/
│
├── BankSystem.java
├── BankAccount.java
├── CurrentAccount.java
├── DepositAccount.java
├── text.txt
└── README.md
```

---

## 🎯 Main Features

### 👤 Account Management

* Create a new bank account
* Select Current or Deposit account
* Set account number and password
* Prevent duplicate account numbers
* Login and logout
* Close an existing account

### 💰 Banking Transactions

* Deposit money
* Withdraw money
* Transfer money to another account
* Check current balance

The `BankAccount` class contains the common banking operations such as deposit, withdrawal, transfer, and loan functionality.

### 🏦 Loan Management

Users can request a loan through their account.

The requested loan amount is added to the loan information and account balance.

### 📈 Interest Calculation

Interest calculation is available for **Deposit Accounts**.

The system uses a fixed **5% interest rate** and calculates interest based on the account balance and number of years.

### 💾 File Storage

Account information is saved in a text file so that the data can be loaded again when the program starts.

The system uses `text.txt` for storing account information.

---

## 🧩 OOP Concepts Used

### 1. Abstraction

`BankAccount` is an **abstract class** that contains common properties and methods for different types of bank accounts.

```java
public abstract class BankAccount
```

It defines common operations such as:

* Deposit
* Withdraw
* Transfer
* Loan request
* Interest calculation

### 2. Inheritance

Two classes inherit from the `BankAccount` class:

```text
BankAccount
   │
   ├── CurrentAccount
   │
   └── DepositAccount
```

Both classes override the `getAccountType()` method.

### 3. Polymorphism

The system uses a `BankAccount` reference to work with both `CurrentAccount` and `DepositAccount` objects.

```java
BankAccount acc = null;
```

The appropriate account object is created based on the selected account type.

### 4. Encapsulation

Important account information such as:

* Name
* Account Number
* Password
* Balance
* Loan

is maintained inside the `BankAccount` class using private/protected access modifiers and getter methods.

---

## 📚 Classes

### `BankSystem`

The main class of the application.

Responsibilities include:

* Starting the application
* Creating accounts
* Login
* Account menu
* Saving accounts
* Loading accounts from file

### `BankAccount`

An abstract base class containing common banking operations.

Main methods include:

* `deposit()`
* `withdraw()`
* `transfer()`
* `requestLoan()`
* `calculateInterest()`
* `checkPassword()`
* `saveToFile()`

### `CurrentAccount`

A child class of `BankAccount` designed for current account holders.

It does not support interest calculation.

### `DepositAccount`

A child class of `BankAccount` designed for deposit account holders.

It supports interest calculation.

---

## 🔄 Account Menu

After successful login, users can access the following options:

```text
1. Deposit
2. Withdraw
3. Transfer
4. Request Loan
5. Check Balance
6. Interest Calculation
7. Close Account
8. Logout
```

---

## 💻 How to Run

### Step 1: Install Java

Make sure Java/JDK is installed on your computer.

### Step 2: Open the Project

Open the project in an IDE such as:

* IntelliJ IDEA
* Eclipse
* NetBeans

### Step 3: Compile the Java Files

Make sure the following classes are available:

```text
BankSystem.java
BankAccount.java
CurrentAccount.java
DepositAccount.java
```

### Step 4: Run the Main Class

Run:

```text
BankSystem.java
```

The console will display:

```text
=== Bank System ===
1. Create Account
2. Login
3. Exit
```

---

## 📸 Project Output

The project demonstrates the following operations:

* Create and login to a Current Account
* Deposit and check balance
* Logout
* Create and login to a Deposit Account
* Withdraw and check balance
* Request a loan
* Calculate deposit interest
* Close an account
* Save account information to a file

These outputs are documented in the project report.

---

## 👥 Project Team

**Group: 06**
**Section: C2**
**Semester: 2nd Year, 1st Semester**

### Members

* **Pial Ahmed Shosi**
* **Rafi Ahammed Rajon**
* **Faria Bente Faruk**

Department of Computer Science & Engineering
University of Asia Pacific

---

## 🎓 Course Information

**Course:** Object Oriented Programming II: Java
**Course Code:** CSE 201
**Department:** Computer Science & Engineering
**University:** University of Asia Pacific

---

## 📌 Future Improvements

Possible future improvements include:

* Graphical User Interface (GUI)
* Database integration
* Improved password security
* Transaction history interface
* More account types
* Online banking functionality
* Better input validation

---

## 👩‍💻 Author

**Faria Bente Faruk**
CSE Undergraduate | Java Developer | Student

---

⭐ Thank you for visiting our Bank Management System project!
