
# infosys-springboard
Python OOP demonstrating Encapsulation, Inheritance, Polymorphism, Abstraction using Bank Accounts.

## Files
- `bank_oop.py` – Main Python file with:
  - `Account` (base class)
  - `SavingsAccount` (inherits from Account)
  - `PremiumAccount` (inherits from SavingsAccount)
## How to Run
1. Install Python (if not already installed).
2. Download or clone this repository.
3. Run the file:
4. Check the console output to see deposits, withdrawals, interest, and credit limit behavior.

## OOP Concepts Used
- **Encapsulation** – Balance and account details stored in protected attributes.
- **Inheritance** – SavingsAccount and PremiumAccount extend the base Account.
- **Polymorphism** – `withdraw()` behaves differently in each account type.
- **Abstraction** – Methods like `add_interest()` and `get_balance()` hide internal details.
