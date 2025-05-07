
---

# UAP - Universal Authenticated Python Encryptor

[![Made for Termux](https://img.shields.io/badge/Made%20for-Termux-blue?style=flat-square&logo=termux)](https://termux.dev)
[![Shell Script](https://img.shields.io/badge/Bash-Script-green?style=flat-square&logo=gnubash)](https://www.gnu.org/software/bash/)
[![Encryption](https://img.shields.io/badge/Encryption-AES--256--CBC-critical?style=flat-square&logo=openssl)](https://www.openssl.org/)
[![Python](https://img.shields.io/badge/Runtime-Python3-yellow?style=flat-square&logo=python)](https://www.python.org)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)](./LICENSE)

**UAP** is a CLI utility that encrypts Python scripts using strong encryption, generating an executable launcher script. Perfect for distributing tools while keeping the source protected.

---

## Features

- AES-256-CBC encryption with password-based key
- Auto-generates `.sh` launcher that decrypts & runs your code
- Safe, temporary execution with automatic cleanup
- Designed for Termux, but runs on any Linux system

---

## Installation

### Requirements

- `wget`
- `dpkg`

### Steps to Install

```bash
# 1. Download the latest .deb package
wget https://github.com/xbyit/UAP/releases/download/Download/uap-pkg.deb

# 2. Install the package
dpkg -i uap-pkg.deb

# 3. Done! Use it via:
uap -e yourscript.py -p yourpasswor

```
---

Usage

# Encrypt a Python script
```bash
uap -e script.py -p mypassword
```
# Run the encrypted file
```
uap -r script.UAP -p mypassword
```
This will create:

script.UAP: the encrypted file

script.sh: a launcher you can share with others

---

# Author

Made with passion by xbyit

Telegram: @xbyit

GitHub: xbyit
