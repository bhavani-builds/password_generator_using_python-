# 🔐 PyPassword Generator

A simple command-line tool built with Python that generates strong, randomized passwords based on your chosen mix of letters, numbers, and symbols.

## Features

- 🔀 Generates passwords with a custom number of letters, numbers, and symbols
- 🎲 Randomly shuffles characters for unpredictable, secure output
- 🖥️ Simple, beginner-friendly command-line interface
- 🐍 Pure Python — no external dependencies required

## Demo

```
Welcome to the PyPassword Generator!
How many letters would you like in your password?
8
How many symbols would you like?
2
How many numbers would you like?
2

Your password is: jR%Tn0qYa#z5
```

## Getting Started

### Prerequisites

- Python 3.x installed on your machine

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/bhavani-builds/pypassword-generator.git
   cd pypassword-generator
   ```

2. Run the script:
   ```bash
   python task.py
   ```

### Usage

When you run the script, you'll be prompted to enter:

| Prompt | Description |
|---|---|
| Number of letters | How many letters (a–z, A–Z) to include |
| Number of symbols | How many symbols (`!#$%&()*+`) to include |
| Number of numbers | How many digits (0–9) to include |

The script will then generate a password using your chosen combination, shuffle the characters randomly, and print the final result.

## How It Works

1. Three character pools are defined: `letters`, `numbers`, and `symbols`.
2. The user specifies how many characters from each pool to include.
3. Random characters are picked from each pool and added to a list.
4. The list is shuffled using `random.shuffle()` to randomize character order.
5. The shuffled list is joined into a final password string and printed.

## Project Structure

```
pypassword-generator/
│
├── task.py        # Main script
└── README.md      # Project documentation
```

## Possible Improvements

- [ ] Remove debug `print()` statements showing the password list before/after shuffling
- [ ] Add input validation (e.g., reject negative numbers or non-numeric input)
- [ ] Use `random.SystemRandom()` or the `secrets` module for cryptographically secure password generation
- [ ] Add an option to copy the password directly to the clipboard
- [ ] Add a minimum total password length requirement

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgements

Inspired by the "100 Days of Code: The Complete Python Pro Bootcamp" password generator project.
