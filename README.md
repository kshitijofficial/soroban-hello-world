# Soroban Smart Contract Project

This repository contains a project structured for developing Soroban smart contracts. It follows the recommended directory structure for Soroban contracts, making it easy to add, manage, and test multiple contracts within the same workspace.

## Project Structure

```plaintext
.
├── contracts
│   └── hello_world
│       ├── src
│       │   ├── lib.rs
│       │   └── test.rs
│       └── Cargo.toml
├── Cargo.toml
└── README.md
```

- **contracts/**: This directory contains the Soroban smart contracts. Each contract resides in its own subdirectory.
- **hello_world/**: A starter Soroban contract to demonstrate the basic structure.
  - `lib.rs`: The main contract logic.
  - `test.rs`: Unit tests for the contract.
  - `Cargo.toml`: Configuration specific to this contract, including dependencies.
- **Cargo.toml**: The top-level configuration file, setting up the project workspace and managing dependencies across contracts.
- **README.md**: Project documentation (this file).

## Prerequisites

Before running this project, ensure you have the setup ready:

- [Soroban Setup](https://developers.stellar.org/docs/build/smart-contracts/getting-started/setup)

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/kshitijofficial/soroban-hello-world
   ```

2. **Initialize the project**:
   Ensure all dependencies are properly set up by running:
   ```bash
   cargo build
   ```

3. **Add a new Soroban contract**:
   You can add new contracts by creating new subdirectories under `contracts/` and adding the necessary files (`Cargo.toml`, `lib.rs`, etc.).

4. **Running Tests**:
   Each contract comes with its own test suite. Navigate to the contract's directory and run:
   ```bash
   cargo test
   ```

## Example Contract: `hello_world`

The `hello_world` contract serves as a basic example to demonstrate the Soroban smart contract framework. You can find the implementation in `contracts/hello_world/src/lib.rs`. The tests are located in `contracts/hello_world/src/test.rs`.
