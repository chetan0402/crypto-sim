# Crypto-sim

Crypto_sim/crypto-sim is a Python library for dealing with cryptography(secure encryption and decryption).

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install crypto-sim.

```
pip install crypto-sim
```

## Usage

### To generate a key
```python
from crypto_sim import crypto

crypto.generate_key()
>>> b'KFH1RhgN_JydLaZzAv6QbpQzsET1SQLjjaFz9dR2-To=' #A key will be returned
```
### To save the key in default dir
```python
from crypto_sim import crypto

crypto.save_and_create_key() #A key will be automatically generate and saved
```
### To get the saved key
```python
from crypto_sim import crypto

crypto.get_key()
```
Note:- this only works when the save_and_create_key() is used

### To encrypt a str
```python
from crypto_sim import

key=crypto.generate_key()
plain_message="hi"
encrypted=crypto.encrypt(plain_message,key)
print(encrypted)
```
Output:-
```python
>>> b'gAAAAABe7uOq4PYOSe9usicMgivc0oVJWaWBzBQmbZbICgrG7TfbdxK8bIuXqttaw-rnScJBGd2RUxgSaC3_CTK0NwbJS_THJA=='
```
### To decrypt
First, we will execute the above code and then we will get the key and the encrypted message

After that,
```python
# This full code is after the above code
decrypted=crypto.decrypt(encryption,key)
print(decrypted)
plain_message==decrypted
```
Output:-
```python
>>> hi
>>> True
```

## Links
[CODE](https://github.com/chetan0402/crypto-sim/)

[LICENSE](https://github.com/chetan0402/crypto-sim/blob/master/LICENSE.txt)

[See what's new in the next project](https://github.com/chetan0402/crypto-sim/blob/master/new.txt)
