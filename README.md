# ATM-CONSOLE-BASED-PROJECT
Here’s a README file content template for your ATM console-based project that you can use for uploading to GitHub:

---

# ATM Console Based Project

## Overview

This is a simple **ATM system** built in Python that simulates basic ATM functionality. It allows users to perform essential operations such as withdrawing money, depositing funds, generating and changing PINs, and checking their account balance, all through a command-line interface.

## Features

- **Withdrawal**: Allows users to withdraw a specified amount from their account.
- **Deposit**: Allows users to deposit a specified amount into their account.
- **Pin Generation**: Users can generate a PIN for their account if one doesn't exist.
- **Mini Statement**: Displays a mini statement including user details and account balance.
- **Pin Change**: Users can change their PIN after providing the old one and setting a new PIN.
- **Balance Check**: Users can check their account balance.
- **Exit**: Users can log out from the ATM system.

## Prerequisites

- Python 3.x or higher

## Getting Started

To use this ATM system, follow the instructions below:

### 1. Clone the repository

First, clone this repository to your local machine using Git.

```bash
git clone https://github.com/yourusername/atm-console-project.git
```

### 2. Navigate to the project directory

```bash
cd atm-console-project
```

### 3. Run the program

Ensure you have Python 3.x installed on your system. Then, run the Python script to start the ATM system:

```bash
python atm.py
```

## Data Structure

The ATM system uses a dictionary to store account information. Each account has:

- **Account Number**: A unique identifier for each user.
- **Account Holder Name**: Name of the account holder.
- **Date of Birth**: The date of birth of the account holder (formatted as `DD-MM-YYYY`).
- **Account Balance**: The current balance in the account.
- **Pin**: A unique PIN for the account (stored as `None` if not set).

Example:

```python
accounts = {
    1001: ["rama", "21-03-2024", 10000, 2103],
    1002: ["surekha", "04-06-2024", 20000, 1272],
    1003: ["pravallika", "07-10-2024", 5000, None]
}
```

## Available Operations

1. **Withdrawal**:
    - Prompt: `Enter Account Number`, followed by `Enter Pin`, and `Enter Amount to Withdraw`.
    - The system checks for sufficient funds and processes the withdrawal if conditions are met.

2. **Deposit**:
    - Prompt: `Enter Account Number` and `Enter Amount to Deposit`.
    - The deposit amount is added to the account balance.

3. **Pin Generation**:
    - Prompt: `Enter Pin` and `Confirm Pin`.
    - A PIN is set for the account if one does not exist.

4. **Mini Statement**:
    - Prompt: `Enter Account Number` and `Enter Pin`.
    - Displays the account holder’s details, account number, date of birth, and balance.

5. **Pin Change**:
    - Prompt: `Enter Old Pin`, `Enter New Pin`, and `Confirm New Pin`.
    - The user can change their existing PIN after verifying the old PIN.

6. **Balance Check**:
    - Prompt: `Enter Account Number` and `Enter Pin`.
    - Displays the current balance of the account.

7. **Exit**:
    - Logs the user out of the ATM system with a thank you message.

## Example Interaction

```
**********************
Welcome to ATM
**********************

Choose Your Option
1. Withdrawal
2. Deposit
3. Pin Generation
4. Mini statement
5. Pin Change
6. Balance Check
7. Exit
Enter Your Option: 1

**********************
Enter Account Number: 1001
Enter Pin: 2103
Enter Amount to Withdraw: 5000
Withdraw Successful!
**********************
```

## Notes

- **Pin Generation**: The PIN is generated only if it’s not already set for the account.
- **Pin Verification**: Every sensitive operation requires the correct PIN for validation.
- **Error Handling**: Basic error handling is implemented for invalid account numbers, incorrect PINs, and insufficient funds.

## License

This project is open-source and available under the [MIT License](LICENSE).

 
