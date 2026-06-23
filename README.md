![Python](https://img.shields.io/badge/python-3.x-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Maintenance](https://img.shields.io/badge/maintained-yes-brightgreen.svg)
![Stars](https://img.shields.io/github/stars/Wa3tE4/Gmail-Brute?style=social)
![Forks](https://img.shields.io/github/forks/Wa3tE4/Gmail-Brute?style=social)
![Issues](https://img.shields.io/github/issues/Wa3tE4/Gmail-Brute)

# Gmail SMTP Authentication Tester

A simple Python script that attempts SMTP authentication against a Gmail account using passwords supplied from a wordlist.

## Features

* Connects to Gmail's SMTP server using TLS
* Supports an included password list
* Supports custom password lists
* Displays authentication results in real time
* Lightweight and easy to modify

## Requirements

* Python 3.x
* Internet connection
* A password list file (`Passwords.txt` or a custom file)

## Installation

Clone the repository:

```bash
git clone https://github.com/Wa3te4/Gmail_Brute.git
cd project-name
```

No external dependencies are required. The script uses Python's built-in `smtplib` module.

## Usage

Run the script:

```bash
python main.py
```

You will be prompted to:

1. Enter a Gmail address.
2. Choose between:

   * The built-in password list (`Passwords.txt`)
   * A custom password list file
3. The script will begin attempting SMTP authentication and display the results.

## Project Structure

```text
.
├── main.py
├── Passwords.txt
└── README.md
```

## Configuration

To use a custom password list, provide the full path or filename when prompted.

Example:

```text
wordlists/common-passwords.txt
```

## Notes

* The script uses Gmail's SMTP endpoint:
  `smtp.gmail.com:587`
* TLS encryption is enabled before authentication attempts.
* Password lists are read line-by-line to reduce memory usage.

## License

This project is provided for educational and research purposes only.
