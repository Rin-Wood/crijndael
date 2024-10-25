# crijndael

`crijndael` is a Python package for decrypting data, using a custom AES-256 decryption algorithm implemented in C.

## Features

- Provides efficient AES-256 decryption functionality, based on C implementation.
- Supports Python 3.6+

## Installation

Install the latest version of `crijndael` from PyPI:

```bash
pip install crijndael
```

## Usage
Here's how to use `crijndael` for decryption:

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
