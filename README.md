# crijndael

`crijndael` is a Python package for encrypting/decrypting data, using the AES-256 algorithm implemented in C.

## Features

- Provides efficient AES-256 encrypting/decryption functionality, based on C implementation.
- Supports Python 3.6+

## Installation

Install the latest version of `crijndael` from PyPI:

```bash
pip install crijndael
```

## Usage
```python
import crijndael

data = b'...'
key = b'...'
iv = b'...'
blocksize = 256
keysize = 256
mode = 0
# 0 - CBC, 1 - ECB

dec = crijndael.decrypt(data, key, iv, blocksize, keysize, mode)
enc = crijndael.encrypt(data, key, iv, blocksize, keysize, mode)
