BloomData Package
The 'BloomData' package is a collection of utility functions designed to make working with data and performing various calculations easier. It includes modules for basic arithmetic operations, generating random phrases, and managing a simple wallet.

Installation
To install the package, you can use pip:
pip install bloomdata

Usage
Arithmetic Operations (bloomdata.py)
The 'bloomdata' module provides functions for performing basic arithmetic operations. For example:
import bloomdata.bloomdata as bd
result = bd.increment(5)
print(result)  # Output: 6

Random Phrase Generator (helper_functions.py)
The 'helper_functions' module includes a function for generating random phrases using adjectives and nouns. Here's how you can use it:
import bloomdata.helper_functions as hf
phrase = hf.random_phrase(['blue', 'large'], ['house', 'tree'])
print(phrase)  # Output: "blue house"

Wallet Management (wallet.py)
The 'wallet' module introduces a 'Wallet' class for managing a simple wallet. You can create a wallet, add funds, spend money, and check the balance:
from bloomdata.wallet import Wallet
my_wallet = Wallet(100)
print(my_wallet.balance)  # Output: 100
my_wallet.spend_cash(30)
print(my_wallet.balance)  # Output: 70

Testing
The package includes a set of pytest tests to ensure the correctness of its functions. You can run the tests using the following command:
pytest

License
This project is licensed under the MIT License. See the LICENSE file for details.
