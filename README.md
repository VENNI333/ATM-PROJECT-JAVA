# ATM Project

## Project Overview
This project simulates a simple ATM (Automated Teller Machine) system using Java. The system includes functionalities such as viewing the balance, depositing money, withdrawing money, and viewing a mini-statement of transactions. The project demonstrates object-oriented programming principles, including encapsulation, abstraction, and interface implementation.

---

## Technologies Used
- *Programming Language*: Java
- *IDE*: Any Java-supported IDE (e.g., IntelliJ IDEA, Eclipse, or VS Code)
- *Java Features*: Object-Oriented Programming (OOP), Interface, Collections (HashMap)

---

## Project Structure
The project consists of the following files:

### 1. Atm.java
This class represents the ATM entity with attributes for balance, deposit amount, and withdraw amount.

### 2. AtmOperationInterf.java
This is an interface defining the required ATM operations:
- viewBalance()
- withdrawAmount(double withdrawAmount)
- depositAmount(double depositAmount)
- viewMiniStatement()

### 3. AtmOperationImpl.java
This class implements the AtmOperationInterf interface. It provides logic for handling ATM operations and maintains a mini-statement using a HashMap.

### 4. AtmMain.java
The entry point for the application. It provides a menu-driven interface to interact with the ATM.

---

## Flow of Code Execution

### 1. *Start the Application*
- The program welcomes the user and prompts for the ATM number and PIN.
- If the ATM number and PIN are correct, the main menu is displayed.

### 2. *Main Menu Options*
The user can choose from the following options:

#### a) View Balance
- Calls viewBalance() to display the current balance in the account.

#### b) Withdraw Amount
- Prompts the user to enter an amount to withdraw.
- Validates if the amount is a multiple of 500 and less than or equal to the available balance.
- Updates the balance and adds the transaction to the mini-statement.

#### c) Deposit Amount
- Prompts the user to enter an amount to deposit.
- Updates the balance and adds the transaction to the mini-statement.

#### d) View Mini Statement
- Displays a list of all transactions (deposits and withdrawals).

#### e) Exit
- Exits the application with a thank-you message.

### 3. *Invalid Input Handling*
- If an invalid choice or incorrect credentials are provided, appropriate error messages are displayed.

---

## Example Execution Screenshot (Pseudo)

### Welcome Screen
text
Welcome to ATM Machine!
Enter ATM number: 12345
Enter PIN: 123


### Main Menu
text
1. View Available Balance
2. Withdraw Amount
3. Deposit Amount
4. View Mini Statement
5. Exit
Enter choice: 1


### View Balance
text
Available Balance is: 10000.0


### Withdraw Amount
text
Enter amount to withdraw: 500
Please collect your cash: 500.0
Available Balance is: 9500.0


### Deposit Amount
text
Enter amount to deposit: 2000
2000.0 Deposited Successfully!
Available Balance is: 11500.0


### Mini Statement
text
500.0 = Amount Withdrawn
2000.0 = Amount Deposited


### Exit
text
Collect your ATM Card
Thank you for choosing ATM Machine


---

## How to Run
1. Compile all Java files in the atm package.
2. Run the AtmMain class to start the program.
3. Follow the on-screen instructions to perform operations.

---

## Additional Notes
- Ensure valid input for all operations to avoid unexpected behavior.
- Extend the project by adding features like password reset or account locking after multiple incorrect PIN attempts.

---

## Screenshots
Include screenshots of the running application (if available).
