
# Aptos Escrow

A decentralized escrow smart contract built on the Aptos blockchain. This project ensures secure transactions between parties without requiring trust by leveraging the security and efficiency of Aptos smart contracts.

## Features

-   Trustless escrow system using Move smart contracts
    
-   Secure fund locking and automated dispute resolution
    
-   Supports multiple participants and conditional releases
    
-   Transparent and auditable transactions
    
-   Low transaction fees and high-speed execution on Aptos
    

## Prerequisites

Ensure you have the following installed before setting up the project:

-   Aptos CLI
    
-   [Move CLI](https://github.com/move-language/move)
    
-   Node.js (for frontend integration if applicable)
    
-   Rust (for Move contract compilation)
    

## Installation

Clone the repository and set up the environment:

```
git clone https://github.com/nhan8573/aptos-escrow.git
cd aptos-escrow
```

## Deploying Smart Contracts

1.  Create an Aptos account (if not already created):
    
    ```
    aptos account create --network testnet
    ```
    
2.  Fund your account using the Aptos faucet.
    
3.  Deploy the smart contract:
    
    ```
    aptos move publish --named-address escrow=your_address --network testnet
    ```
    

## Usage

-   **Initialize an Escrow:** A seller locks funds into the escrow smart contract.
    
-   **Buyer Confirms Receipt:** The buyer verifies they have received the service/product.
    
-   **Dispute Resolution:** If a dispute occurs, an arbitrator can step in based on predefined rules.
    
-   **Release Funds:** Once conditions are met, funds are automatically released.
    

## API Reference

To interact with the smart contract programmatically, use the Aptos SDK:

```
import { AptosClient } from 'aptos';
const client = new AptosClient('https://fullnode.testnet.aptoslabs.com');
```

## Contributing

1.  Fork the repository.
    
2.  Create a new branch.
    
3.  Commit your changes.
    
4.  Submit a pull request.
    

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For any questions, feel free to open an issue or reach out to `your_email@example.com`.
