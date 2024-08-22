# AES Encryption and Decryption

This project implements a simplified version of the AES (Advanced Encryption Standard) algorithm in Python. The implementation includes both encryption (`eaes`) and decryption (`daes`) functions that operate on 16-byte blocks of data, with a focus on demonstrating the core concepts of AES, such as key expansion, substitution using S-boxes, and matrix manipulation. Test files are included to validate the correctness of the implementation.

## Features

- **AES Encryption (`eaes`)**: Encrypts a message using a given key, applying two rounds of AES transformations.
- **AES Decryption (`daes`)**: Decrypts a message that was encrypted using the `eaes` function, reversing the AES transformations.
- **S-Box and Inverse S-Box**: Utilizes pre-defined S-boxes for byte substitution during encryption and decryption.
- **Matrix Manipulations**: Implements key AES operations, such as shifting rows and mixing columns, through matrix transformations.
- **Unit Testing**: Includes comprehensive unit tests with provided test files to verify the correctness of both encryption and decryption processes.

## Project Structure

- **`daes.py`:** Contains the implementation of the AES encryption and decryption functions, as well as the unit tests for verifying the implementation.
- **Test Files:**
  - **`keys_short.txt`:** A short key file used for testing encryption and decryption.
  - **`keys_long.txt`:** A long key file used for testing encryption and decryption.
  - **`message_short.txt`:** A short message used for encryption and decryption tests.
  - **`message_long.txt`:** A longer message used for encryption and decryption tests.
  - **`cipher_short.txt`:** The expected encrypted output for `message_short.txt`.
  - **`cipher_long.txt`:** The expected encrypted output for `message_long.txt`.

## How to Use

### Encrypt a Message

To encrypt a message, use the `eaes` function, providing the paths to the input message file, key file, and the output file where the encrypted message will be stored.

Example:
```bash
python -c "from daes import eaes; eaes('message_short.txt', 'keys_short.txt', 'encrypted.txt')"
```

### Decrypt a Message  
To decrypt a message, use the daes function, providing the paths to the encrypted message file, key file, and the output file where the decrypted message will be stored.
Example:
```bash
python -c "from daes import daes; daes('cipher_short.txt', 'keys_short.txt', 'decrypted.txt')"

```

### Running Unit Tests 
Unit tests are included to verify the functionality of the encryption and decryption algorithms using the provided test files. You can run the tests using the following command:
Example:
```bash
python daes.py

```
This will execute the unittest framework and run all test cases defined in the script, comparing the results against the provided test files.

## Installation  

1. **Clone the repository**
   ```bash
   git clone https://github.com/omriarie/AES.git
   ```

2. **Navigate to the project directory**
   ```bash
   git clone https://github.com/omriarie/AES
   ```

3. **Run the unit tests to ensure everything is set up correctly**
   ```bash
   python daes.py
   ```


## Contact
For any inquiries or issues, please open an issue on the GitHub repository or contact the maintainers directly:

Omri Arie – omriarie@gmail.com  
Project Link: https://github.com/omriarie/AES
