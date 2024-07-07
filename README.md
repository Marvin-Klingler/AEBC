# AEBC: Advanced Encryption Block Cipher

## Overview

AEBC (Advanced Encryption Block Cipher) is a data encryption program developed as a Matura project for the Kantonsschule Zofingen. Concept invented by Alican Karatasli. 
The program utilizes a unique 9x9 block cipher to provide robust encryption for sensitive data. AEBC is designed to offer strong security features suitable for academic and practical applications.

## Features

- **9x9 Block Cipher**: Uses a custom 9x9 block cipher for encryption and decryption processes.
- **High Security**: Provides a high level of security due to its unique and complex encryption algorithm.
- **User-Friendly Interface**: Command-line interface for easy interaction with the program.
- **Cross-Platform**: Compatible with major operating systems including Windows, macOS, and Linux.

## Table of Contents

- [Installation](#installation)
- [Encryption Process](#encryption-process)
- [Decryption Process](#decryption-process)

## Installation

### Prerequisites

- Python 3.6 or higher
- Git

### Steps

1. Clone the repository:
    ```sh
    git clone https://github.com/Marvin-Klingler/AEBC.git
    ```
2. Navigate to the project directory:
    ```sh
    cd AEBC
    ```
3. Launch main file:
   ```sh
   python AEBC.py
   ```

## Encryption Process

The encryption process in AEBC involves the following steps:

1. **Input Handling**: The plaintext data is read from the specified input file.
2. **Block Formation**: The plaintext is divided into 9x9 blocks. If the final block is incomplete, padding is applied.
3. **Key Scheduling**: The encryption key is processed to generate subkeys used in the cipher rounds.
4. **Cipher Rounds**: Each 9x9 block undergoes multiple rounds of substitution and permutation based on the subkeys.
  - **Substitution Box**: Bytes are swapped out with a predefined list.
  - **Displacement**: Bytes in a box are shuffled in a pattern based on subkey.
  - **Transposition**: Blocks are shuffled in a pattern based on subkey.
  - **Key Infusion**: Bytes are modified with key.
6. **Output Handling**: The encrypted data is written to the specified output file.

## Decryption Process

The decryption process mirrors the encryption process and includes the following steps:

1. **Input Handling**: The encrypted data is read from the specified input file.
2. **Block Formation**: The ciphertext is divided into 9x9 blocks.
3. **Key Scheduling**: The decryption key is processed to regenerate the subkeys.
4. **Inverse Cipher Rounds**: Each 9x9 block undergoes the same processes used in the encryption method in reeversed order.
6. **Output Handling**: The decrypted data is written to the specified output file, with padding removed if necessary.

---

**Note**: AEBC was created as part of a school project and is intended for educational purposes. While the encryption algorithm is designed to be secure, it may not be suitable for all real-world applications without further validation and testing.
