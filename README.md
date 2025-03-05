# bank_management
This Java project is a Bank Management System that simulates basic banking operations like deposits, withdrawals, and balance checking using Object-Oriented Programming (OOP) principles.
Goal of the Project
This Java project simulates a banking system using Object-Oriented Programming (OOP) principles. It allows users to:

Create accounts (Savings or Checking)
Deposit money
Withdraw money
Check balance
It uses OOP concepts like abstraction, inheritance, encapsulation, and polymorphism to create a structured and scalable banking system.

Code Explanation
1. Abstract Class: BankAccount
Represents a generic bank account.
Contains:
accountNumber, accountHolder, and balance as protected attributes.
An abstract deposit() and withdraw() method (to be implemented in subclasses).
A method displayBalance() to show the current balance.
getAccountNumber() to fetch an account using the account number.
2. Subclass: SavingsAccount
Inherits from BankAccount.
Has an additional attribute interestRate.
Implements:
deposit(): Increases balance.
withdraw(): Allows withdrawal only if sufficient balance.
3. Subclass: CheckingAccount
Inherits from BankAccount.
Has an attribute overdraftLimit (allows withdrawal beyond balance).
Implements:
deposit(): Increases balance.
withdraw(): Allows overdraft withdrawal up to the limit.
4. Bank Class
Manages multiple bank accounts.
Stores accounts in an ArrayList<BankAccount>.
Methods:
addAccount(): Adds a new account.
findAccount(): Finds an account by account number.
5. BankSystem (Main Class)
Provides a menu-driven system for users.
Uses Scanner for input.
Allows users to:
Create an account (Savings or Checking).
Deposit money.
Withdraw money.
Check balance.
Exit the system.
OOP Principles Used
✅ Encapsulation – Private attributes, public methods.
✅ Abstraction – BankAccount is an abstract class.
✅ Inheritance – SavingsAccount and CheckingAccount extend BankAccount.
✅ Polymorphism – Different implementations of deposit() and withdraw() in subclasses.
