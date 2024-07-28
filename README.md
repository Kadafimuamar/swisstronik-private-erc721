# swisstronik-private-erc721

This project sets up a Hardhat environment to deploy and interact with an ERC-721 (NFT) contract and makes it private, on the Swisstronik testnet. Follow the steps below to get started.

## Prerequisites

Ensure you have the following installed:
- Node.js
- npm

## Faucet

https://faucet.testnet.swisstronik.com/

## Setup Instructions

1. Clone the repository:
    ```sh
    git clone https://github.com/kadafimuamar/swisstronik-private-erc721.git
    cd swisstronik-private-erc721
    ```

2. Run

    ```bash
    npm install --save-dev @nomicfoundation/hardhat-toolbox
    npm install dotenv
    npm install @swisstronik/utils
    npm install @openzeppelin/contracts
    ```

## Create File .env for Private Key (Keep Safe for this)

1. 

```bash
    PRIVATE_KEY=YOUR-PRIVATE-KEY
```

## Running

1. Compile

 ```bash
    npx hardhat compile
```

2. Deploy Private erc-721

 ```bash
    npx hardhat run scripts/deploy.js --network swisstronik
```

3. Minting Private erc-721

 ```bash
    npx hardhat run scripts/mint.js --network swisstronik
```


3. Follow the prompts to enter your private key and NFT details.


## Notes

- The contract address will be saved in `contract.txt`.
- The transaction hash for the minting process will be printed in the terminal.
