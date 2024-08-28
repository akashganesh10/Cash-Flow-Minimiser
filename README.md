# Cash Flow Minimizer

## Introduction

**Cash Flow Minimizer** is a C program designed to minimize the number of financial transactions among multiple banks. This system helps to reduce the complexity and cost associated with inter-bank transactions, especially when banks use different modes of payment. A world bank is considered as an intermediary to facilitate transactions between banks that have no common payment modes.

## Features

- **Bank Management**: Allows the user to input multiple banks with different payment modes.
- **Transaction Handling**: Minimizes the number of transactions needed to settle all debts among banks.
- **Payment Mode Matching**: Ensures that transactions are made using common payment modes between banks.
- **World Bank Intermediary**: Acts as a mediator when no common payment mode exists between two banks.

## How It Works

1. **Bank Information Input**: The user inputs the number of banks, each bank's name, and the payment modes they support.
2. **Transaction Input**: The user inputs the number of transactions, followed by details of each transaction (debtor bank, creditor bank, and amount).
3. **Transaction Minimization**: The program processes the input and reduces the number of transactions needed by finding the minimum cash flow among the banks.
4. **Output**: The minimized transactions are displayed, specifying the amount each bank needs to pay or receive and the payment mode used.

## Prerequisites

- C compiler (GCC or any other C compiler)
- Basic understanding of C programming language

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/akashganesh10/cash-flow-minimizer.git
    ```

2. **Compile the Program**:
    ```bash
    gcc cash_flow_minimizer.c -o cash_flow_minimizer
    ```

3. **Run the Program**:
    ```bash
    ./cash_flow_minimizer
    ```

## Usage

1. **Input the Number of Banks**: Provide the number of banks participating in the transactions.
2. **Enter Bank Details**: For each bank, enter the bank's name, the number of payment modes it supports, and the payment modes themselves.
3. **Enter Transaction Details**: Provide the number of transactions followed by the debtor bank, creditor bank, and the transaction amount for each.
4. **Get Results**: The program will display the minimized transactions required to settle the debts among banks.

## Example

Suppose there are 3 banks, with the following payment modes:

- **Bank A**: Credit, Debit
- **Bank B**: UPI, NetBanking
- **Bank C**: Credit, UPI

And the transactions are:

1. Bank A owes Bank B Rs 1000
2. Bank B owes Bank C Rs 2000
3. Bank C owes Bank A Rs 500

The program will minimize these transactions, and the output could be:

```
Bank A pays Rs 500 to Bank C via Credit
Bank B pays Rs 1000 to Bank A via UPI
Bank B pays Rs 1000 to Bank C via UPI
```

## Contributing

Feel free to fork this project, make improvements, and submit a pull request. All contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- This project is inspired by the need to optimize and minimize inter-bank transactions for efficiency.

## Contact

For any questions or feedback, feel free to reach out via ag8163@srmist.edu.in.
