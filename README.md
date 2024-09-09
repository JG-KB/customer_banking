# Banking Account Program

This project is a simple banking account simulation that allows users to create savings and certificate of deposit (CD) accounts, calculate interest, and update account balances accordingly. The program uses an `Account` class and two functions: `create_savings_account` and `create_cd_account`. The user can input initial balances, interest rates, and account maturity periods to simulate how interest accrues over time.

## Features

- **Account Class**: This class handles the core properties of an account, including the balance and interest.
- **Savings Account Functionality**: The program calculates interest for a savings account based on the user's input and updates the balance.
- **CD Account Functionality**: Similar to the savings account, but for a Certificate of Deposit (CD), where the interest earned is calculated and added to the balance.
- **User Input**: Users are prompted to provide the initial balance, interest rate, and maturity period (in months) for both the savings and CD accounts.
- **Formatted Output**: The final balances and interest earned are displayed with two decimal places and thousand separators.

## Requirements

- Python 3.10 or later

## Files Included

1. **`account.py`**: Contains the `Account` class used to manage account balances and interest.
2. **`savings_account.py`**: Defines the `create_savings_account` function, which calculates interest for a savings account.
3. **`cd_account.py`**: Defines the `create_cd_account` function, which calculates interest for a CD account.
4. **`customer_banking.py`**: The main script that prompts the user for input, calls the account functions, and prints the results.

## Installation

1. Clone the repository to your local machine:

   `git clone https://github.com/your-username/banking-account-program.git`

2. Navigate to the project directory:

   `cd banking-account-program`

## Usage

1. Run the `customer_banking.py` script:

   `python customer_banking.py`

2. You will be prompted to enter the following details for both the savings and CD accounts:

   - Initial account balance
   - Interest rate (annual percentage rate)
   - Maturity period (in months)

3. The program will calculate the interest earned and update the account balances. It will then display:

   - The interest earned
   - The updated account balance with interest

## Example Interaction:

Enter the savings account balance: 500000  
Enter the savings account interest rate: 5  
Enter the savings account maturity in months: 12  
The interest earned on the savings account is: 25,000.00  
The updated savings account balance with interest earned is: 525,000.00  

Enter the CD account balance: 1000000  
Enter the CD account interest rate: 10  
Enter the CD account maturity in months: 12  
The interest earned on the CD account is: 100,000.00  
The updated CD account balance with interest earned is: 1,100,000.00  


## Functions

### `Account` Class

- `__init__(self, balance, interest)`: Initializes an account with a given balance and interest.
- `set_balance(self, balance)`: Updates the balance of the account.
- `set_interest(self, interest)`: Updates the interest for the account.

### `create_savings_account(balance, interest_rate, months)`

- **Args**:
  - `balance (float)`: The initial balance of the savings account.
  - `interest_rate (float)`: The annual interest rate for the savings account.
  - `months (int)`: The duration in months for which the interest is calculated.
- **Returns**:
  - The updated balance after adding the interest earned.
  - The interest earned during the period.

### `create_cd_account(balance, interest_rate, months)`

- **Args**:
  - `balance (float)`: The initial balance of the CD account.
  - `interest_rate (float)`: The annual interest rate for the CD account.
  - `months (int)`: The duration in months for which the interest is calculated.
- **Returns**:
  - The updated balance after adding the interest earned.
  - The interest earned during the period.
