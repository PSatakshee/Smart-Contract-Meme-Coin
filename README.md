# Smart Contract- Meme Coin
This project is a complete solution for managing a token on the Ethereum blockchain. It includes a smart contract written in Solidity for transferring tokens, burning excess supply, and minting new tokens as needed. The front-end is developed using React and integrates with the Ethereum blockchain using Ethers.js.

## Output

Below are some screenshots and outputs from the project to give you an idea of how it works.

### 1. Initial Screen
The initial screen is displayed when the application loads. It prompts the user to connect their MetaMask wallet to interact with the DApp.

![Initial Screen](https://github.com/PSatakshee/Smart-Contract-Meme-Coin/blob/main/Output/Initial%20screen.jpeg)

### 2. Wallet Connected
Once the wallet is connected, the application displays the user's wallet address and contract address. The user can then access the functionalities for transferring, minting, or burning tokens.

![Wallet Connected](https://github.com/PSatakshee/Smart-Contract-Meme-Coin/blob/main/Output/Connected%20to%20wallet.jpeg)

### 3. Token Transferred
After initiating a token transfer, the application shows a token address and the amount transferred. The transaction details are also recorded on the blockchain.

![Token Transferred](https://github.com/PSatakshee/Smart-Contract-Meme-Coin/blob/main/Output/Tokens%20transfered.jpeg)

## ⚠️ Important Update:

This project was initially configured to use the Rinkeby testnet. However, as of 2023, Rinkeby has been deprecated and is no longer active. To ensure continued functionality and testing, you'll need to switch to an active Ethereum testnet like Goerli or Sepolia.

### Why the change?

- Rinkeby is no longer supported, meaning you won't be able to deploy or interact with contracts on that network.
- Goerli and Sepolia are the recommended testnets moving forward, offering better support and a stable environment for testing your smart contracts.


Please update your Hardhat configuration to use Goerli or Sepolia by following the instructions in the ** hardhat.config.js** file section:
```
      module.exports = {
        solidity: "0.8.4",
        defaultNetwork: "goerli",  // Change to "goerli" or "sepolia"
        networks: {
          goerli: {  // Replace with "sepolia" if using Sepolia
            url: "[Your_Alchemy_or_Infura_URL]",
            accounts: ["0x" + "[Your_Private_Key]"],
          },
        },

```
