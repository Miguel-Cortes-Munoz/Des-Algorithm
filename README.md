# DES Encryption and Decryption Tool

This C++ program implements the **Data Encryption Standard (DES)** algorithm for encrypting and decrypting 64-bit blocks of data using a 64-bit key (16 hex characters). It allows the user to input a key and a plaintext or ciphertext in hexadecimal format and returns the encrypted or decrypted result.

##  About DES

DES is a symmetric-key algorithm for the encryption of digital data. It operates on 64-bit blocks and uses a 56-bit key (plus 8 parity bits) across 16 rounds of Feistel-based processing with key-dependent substitutions and permutations. This implementation follows the standard DES specification including:

- Initial and Final Permutations (IP/FP)
- 16 Feistel rounds using:
  - Expansion (E table)
  - S-box substitutions (8 groups)
  - Permutation (P table)
- Subkey generation using PC-1, PC-2, and left rotations

---

##  Made By

**Miguel Cortes Muñoz**  
Completed for self-study and experimentation with classic symmetric encryption.

---

##  How to Use
### Compile

Use any standard C++ compiler (C++11 or later):

```bash
g++ -o des_tool des.cpp

Run

./des_tool
Sample Input/Output
You will be prompted to select an operation and enter key and data in hexadecimal format.

Choose operation (1 for Encryption, 2 for Decryption): 1
Enter the key in hexadecimal (16 characters):
133457799BBCDFF1
Enter the input text in hexadecimal:
0123456789ABCDEF
Encrypted output (Hex): 85E813540F0AB405
