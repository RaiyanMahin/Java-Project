# Banking Application

A simple Java console-based banking application with Object-Oriented Programming (OOP) principles.

## Overview

The application allows users to perform various banking operations, such as creating accounts, displaying account details, updating balances, depositing and withdrawing amounts, and searching for accounts. It employs OOP concepts such as encapsulation, abstraction, inheritance, and polymorphism.

## Usage

1. Compile and run the `Main` class. 
2. Follow the on-screen menu to perform banking operations.

## File Link
- [Main Java File](https://github.com/RaiyanMahin/WSD_Coding_Challenge/blob/main/WSD_Coding_Challenge/src/Main.java)

## Structure

### Main Class

The main class `Main` serves as the entry point for the application. It contains a `BankingApplication` inner class and handles user interactions through a menu system.

### BankingApplication Class

This class manages a list of `Account` objects and provides methods for creating, displaying, updating, and deleting accounts. It also handles deposit and withdrawal operations.

#### Methods

- `createAccount()`: Creates a new account based on user input.
- `displayAllAccounts()`: Displays details of all accounts.
- `updateAccountBalance(int accountNumber)`: Updates the balance of a specific account.
- `deleteAccount(int accountNumber)`: Deletes a specific account.
- `depositAmount(int accountNumber)`: Deposits an amount into a specific account.
- `withdrawAmount(int accountNumber)`: Withdraws an amount from a specific account.
- `searchAccount(int accountNumber)`: Searches for an account based on the account number.
- `isPossibleWithdraw(int accountNumber, int amount)`: Checks if a withdrawal is possible for a specific account and amount.
- `isAccountExist(int accountNumber)`: Checks if a given account number exists in the list of accounts.
- `isAccountNumberUnique(int accountNumber)`: Checks if a given account number is unique among existing accounts.

### Account Class

An abstract class representing a generic account. It contains common properties such as name, account number, creation date, and balance. It also declares abstract methods for displaying account details and updating the balance.

#### Methods

- `display()`: Abstract method to display account details.
- `updateBalance(int amount)`: Abstract method to update the account balance.

### SavingsAccount, SalaryAccount, CurrentAccount Classes

These classes inherit from the `Account` class and represent specific types of accounts. They provide concrete implementations of the abstract methods and include additional details for their respective account types.

## OOP Concepts

- **Encapsulation**: Achieved by using private access modifiers for fields and methods within classes.
- **Abstraction**: Implemented through the abstract `Account` class, providing a blueprint for specific account types.
- **Inheritance**: Utilized by the specific account types (`SavingsAccount`, `SalaryAccount`, `CurrentAccount`) inheriting common properties and methods from the `Account` class.
- **Polymorphism**: Demonstrated through the use of abstract methods (`display` and `updateBalance`) in the `Account` class, which are implemented differently in each specific account type.

## Sample Output

-[# Check this File](https://github.com/RaiyanMahin/WSD_Coding_Challenge/blob/main/Sample%20Output%20of%20BankingApplication.pdf)

Feel free to explore and extend the application for additional features and improvements.

