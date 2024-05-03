```markdown
# Blockchain Implementation

This is a simple implementation of a blockchain using C programming language. It demonstrates the basic concepts of a blockchain, including adding blocks, verifying the chain, altering blocks, and detecting attempts to tamper with the chain.

## Features

- Add new blocks to the blockchain
- Add multiple random blocks to the blockchain
- Alter a specific block in the blockchain
- Print the entire blockchain
- Verify the integrity of the blockchain
- Detect attempts to tamper with the blockchain

## Prerequisites

- GCC compiler
- OpenSSL library (for SHA-256 hashing)

## Building and Running

1. Compile the program with the OpenSSL library:

```
gcc blockChain2.c -o blockchain -lcrypto
```

2. Run the compiled program:

```
./blockchain
```

## Usage

Upon running the program, you will be presented with a menu of options:

1. Add a new block to the blockchain (manual entry)
2. Add multiple random blocks to the blockchain
3. Alter a specific block in the blockchain
4. Print the entire blockchain
5. Verify the integrity of the blockchain
6. Attempt to tamper with the blockchain (for demonstration purposes)

Follow the on-screen prompts to interact with the blockchain.

## Code Structure

The code consists of the following main functions:

- `addBlock(int data)`: Adds a new block to the blockchain with the specified data.
- `verifyChain()`: Verifies the integrity of the blockchain by checking the hash values of each block.
- `alterNthBlock(int n, int newData)`: Alters the data of the nth block in the blockchain.
- `hackChain()`: Attempts to tamper with the blockchain by modifying block data and hash values.
- `toString(struct block b)`: Converts a block structure to a byte array for hashing.
- `hashPrinter(unsigned char hash[], int length)`: Prints the hash value in hexadecimal format.
- `hashCompare(unsigned char *str1, unsigned char *str2)`: Compares two hash values for equality.
- `printBlock(struct block *b)`: Prints the details of a single block.
- `printAllChain()`: Prints the details of all blocks in the blockchain.

## License

This project is licensed under the [MIT License](LICENSE).
```

This README.md file provides an overview of the blockchain implementation, including its features, prerequisites, instructions for building and running the program, a high-level description of the code structure, and information about licensing.
