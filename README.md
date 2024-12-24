# File Encryption and Decryption Tool

This Python script allows you to securely encrypt and decrypt files using the `cryptography.fernet` module. The script supports both encryption and decryption based on user input.

## Features
- **File Encryption:** Encrypt files to protect sensitive data.
- **File Decryption:** Decrypt previously encrypted files using the same key.

## Prerequisites
- Python 3.6 or above
- `cryptography` library

Install the required library by running:
```bash
pip install cryptography
```

## How to Use

### Step 1: Clone the Repository
```bash
git clone <repository-url>
cd <repository-directory>
```

### Step 2: Run the Script
Run the script using Python:
```bash
python <script_name>.py
```

### Step 3: Choose an Operation
1. **Encryption**
   - Enter the file name with the path to encrypt.
   - The script generates a unique encryption key, which you need to save securely.
   - The encrypted file overwrites the original file.
2. **Decryption**
   - Enter the file name with the path to decrypt.
   - Provide the previously generated encryption key.
   - The decrypted file overwrites the original file.

## Key Points
- The key generated during encryption is essential for decryption. **Save it securely.**
- Ensure that you use the correct key when decrypting files; an incorrect key will result in a failure to decrypt.

## Example
### Encryption:
1. Run the script and select `1` for encryption.
2. Enter the path of the file you want to encrypt.
3. Save the generated encryption key.

Example output:
```
Please enter the Type of operation to perform
1.Encryption
2.Decryption
1
Please enter the file name with path for Encryption
example.txt
Key: mF9c6jAB3LNaTOIG0czniTkix4Cz_xd3NcDgxJ7ZDBs=
File example.txt is encrypted and saved.
```

### Decryption:
1. Run the script and select `2` for decryption.
2. Enter the path of the encrypted file.
3. Enter the encryption key generated during encryption.

Example output:
```
Please enter the Type of operation to perform
1.Encryption
2.Decryption
2
Please enter the file name with path for Decryption
example.txt
Please enter the Key to decrypt
mF9c6jAB3LNaTOIG0czniTkix4Cz_xd3NcDgxJ7ZDBs=
File example.txt decrypted and saved.
```

## File Structure
- `script_name.py`: Python script for encryption and decryption.

## Notes
- The script modifies the file in place, so make sure to keep a backup of the original file if necessary.
- Always store your encryption keys in a secure location. Loss of the key means the data cannot be recovered.


