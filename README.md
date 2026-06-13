# Cash Register Lab

## Description

This project implements a Cash Register using Object-Oriented Programming (OOP) principles in Python.

The application simulates the behavior of a cash register used in an e-commerce environment. It allows users to:

* Add items to a register
* Track purchase totals
* Apply percentage discounts
* Void the most recent transaction
* Maintain a list of purchased items

## Features

### CashRegister Class

#### Attributes

* `discount` - Percentage discount applied to purchases
* `total` - Running total of all items added
* `items` - List containing all purchased items
* `previous_transactions` - Stores information about previous transactions

#### Methods

##### add_item(item, price, quantity=1)

Adds an item to the register.

Example:

```python
register.add_item("apple", 0.99)
register.add_item("book", 5.00, 3)
```

##### apply_discount()

Applies the configured discount to the current total.

Example:

```python
register = CashRegister(20)
register.apply_discount()
```

##### void_last_transaction()

Removes the most recent transaction and updates the total accordingly.

Example:

```python
register.void_last_transaction()
```

## Project Structure

```text
oop-p2-cash-register-lab/
│
├── lib/
│   ├── cash_register.py
│   └── testing/
│
├── README.md
├── Pipfile
└── pytest.ini
```

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd oop-p2-cash-register-lab
```

Install dependencies:

```bash
pipenv install
```

or

```bash
python3 -m pip install pytest
```

## Running Tests

Run all tests:

```bash
python3 -m pytest
```

Expected result:

```text
14 passed
```

## Technologies Used

* Python 3
* Pytest
* Object-Oriented Programming (OOP)

## Author

Thomas Buko

## License

This project was created for educational purposes as part of the Moringa School Software Engineering Program.
