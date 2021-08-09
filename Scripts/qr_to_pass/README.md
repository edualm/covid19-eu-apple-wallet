#   `qr_to_pass`

Based on [vacdec](https://github.com/hannob/vacdec).

Generates a pass from a QR code image.

#   Setup

You will need the python pillow, pyzbar, cbor2 and base45 packages. Additionally, you need zbar. For Mac OS X, it can be installed via `brew install zbar`, on Debian systems via `apt install libzbar0`. [Source](https://pypi.org/project/pyzbar/)

You can install them via your distribution or via pip:

```
pip install base45 cbor2 pillow pyzbar
```