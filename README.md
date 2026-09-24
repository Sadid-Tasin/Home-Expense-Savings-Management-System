# Home Expense & Savings Management System

## Project Overview

**Home Expense & Savings Management System** is a console-based C programming project designed to manage and analyze household expenses.

The system provides predefined household expense categories, a monthly expense calculator, a yearly savings calculator, login security, and password management.

The main purpose of this project is to demonstrate how basic C programming concepts can be combined to create a practical expense-management application.

---

## Main Objectives

* Display different categories of household expenses.
* Provide predefined information about house rent, food, utilities, and household items.
* Calculate total monthly expenses.
* Calculate per-person monthly expenses.
* Calculate yearly savings.
* Track extra costs and savings throughout the year.
* Provide a basic login authentication system.
* Allow the user to change the account password.
* Protect the system with a maximum login-attempt limit.

---

## Main Features

### 1. Secure Login System

The program starts with a login panel.

The user must provide the correct username and password to access the system.

The program allows a maximum of **3 login attempts**. If all attempts fail, the program automatically locks and exits.

---

### 2. Monthly Home Expense Categories

The system contains four major expense categories:

#### House Rent

* Monthly Rent
* Advance Payment
* Maintenance Charge
* Security and Maid Charge

#### Food

* Groceries
* Vegetable/Meat Purchase
* Monthly Food Storage
* Special Items

#### Utilities

* Electricity
* Gas
* Water
* Internet

#### Household Items

* Cleaning Items
* Kitchen Items
* Home Repair & Maintenance
* Water Cleaner & WASA Bill

These categories are displayed through separate functions such as `HouseRent()`, `Food()`, `Utilities()` and `Household()`.

---

## 3. Monthly Expense Calculator

The user can enter any number of expense types.

For each expense, the program takes:

* Expense name
* Expense amount

It then calculates the total expense.

The user can also enter the number of family members, after which the system calculates the expense per person.

### Calculation

```text
Total Expense = Sum of all entered expenses

Per Person Expense = Total Expense / Number of Members
```

The calculator is implemented through the `calculate()` function.

---

## 4. Yearly Savings Calculator

The system can calculate savings over a full 12-month period.

The user enters:

* Fixed monthly cost
* Running cost for each month
* Fixed monthly saving amount

The system compares the running cost with the fixed cost.

If the running cost is higher, the difference is treated as an extra cost/loan.

If the running cost is lower, the difference is treated as saved profit.

The program then calculates the final yearly saving after adjusting the extra costs and savings.

### Final Saving Formula

```text
Yearly Saving = Monthly Saving × 12

Final Saving =
(Yearly Saving + Profit) - Loan + Advance
```

The project uses a fixed **1000 taka advance** for urgent needs in the calculation.

---

## 5. Password Management

The Settings section allows the user to change the existing password.

The program first asks for the old password.

If the old password is correct, the user can enter a new password.

If the old password is incorrect, the password remains unchanged.

After successfully changing the password, the system requires the user to log in again.

---

## Program Flow

```text
Start
  ↓
Login
  ↓
Username & Password Verification
  ↓
Main Program Menu
  ├── Monthly Home Expense Categories
  ├── Per Person Expense Calculator
  ├── Yearly Savings Calculator
  ├── Settings
  │     └── Change Password
  └── Exit
```

---

## Programming Concepts Used

* C Functions
* `if-else`
* `switch-case`
* `for` loop
* `while` loop
* Arrays
* Character/String handling
* User input/output
* Arithmetic operations
* Function-based program organization
* Basic authentication logic

---

## Technologies

**Language:** C

**Type:** Console Application

**Main Concepts:** Functions, Loops, Conditions, Arrays, Strings, Switch Case

---

## Learning Outcomes

Through this project, the following concepts were practiced:

* Breaking a large program into functions.
* Taking and processing user input.
* Using loops and conditional statements.
* Working with arrays and strings.
* Performing financial calculations.
* Implementing a basic authentication system.
* Designing a menu-driven console application.

---

## Project Type

**Academic / Beginner C Programming Project**

The project demonstrates how fundamental programming concepts can be used to build a practical household expense and savings management system.
