# XRPL APY Calculator

## Introduction

This Python script calculates the Average Pool Yearly Percentage (APY) and Average Wallet APY for a given wallet address on the XRPL (XRP Ledger). It utilizes the xrpl library to interact with the ledger and perform the necessary calculations.

## Installation

To install the required dependencies, run the following command:

```
pip install xrpl
```

## Usage

The script defines several functions to calculate APY for a wallet address. Here's an example usage:

```python
from xrpl_apy_calculator import calculate_apy, get_deposit_events, get_transaction_history, get_balance

# Example usage
wallet_address = "r9cZA1mLK5R5Am25ArFby8XbriRay7UFg"
total_pool_apy, average_wallet_apy = calculate_apy(wallet_address)
print("Total Pool APY:", total_pool_apy)
print("Average Wallet APY:", average_wallet_apy)
```

## Functionality

- `calculate_apy(wallet_address, ledger_index='validated')`: Calculates the total pool APY and average wallet APY for the given wallet address.
- `get_deposit_events(wallet_address, client, ledger_index)`: Retrieves deposit events for the wallet address from the XRPL ledger.
- `get_transaction_history(wallet_address, client, ledger_index)`: Fetches the transaction history for the wallet address.
- `get_balance(wallet_address, client, ledger_index)`: Queries the balance of the wallet address on the XRPL ledger.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or bug fixes.

## License

This project is licensed under the MIT License.# XRPLAMMAPY
APY check per wallet address
