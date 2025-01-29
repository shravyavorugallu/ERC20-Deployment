# ERC20 Token Deployment Instructions

## Prerequisites
- A web browser with [MetaMask](https://metamask.io/) installed
- Testnet funds (Goerli or Sepolia) – [Get testnet ETH here](https://goerlifaucet.com/)
- An [Etherscan](https://etherscan.io/) account with an API key

## Deployment Steps

### 1. Setup Remix
1. Open [Remix Ethereum](https://remix.ethereum.org/).
2. Create a new workspace from the upper-left menu.
3. Choose the OpenZeppelin ERC20 template and select 'Mintable'.

### 2. Modify and Compile the Contract
1. In the folder menu, open `contracts/MyToken.sol`.
2. Modify the token name and symbol in the `constructor` function.
3. Click the Solidity logo on the left sidebar.
4. Select `MyToken.sol` and compile it.

### 3. Deploy the Contract
1. Click the Ethereum logo on the left sidebar.
2. In the environment menu, choose **Injected Provider - MetaMask** and connect your wallet.
3. Ensure you have testnet ETH in your wallet.
4. In the deployment menu, select `MyToken.sol`.
5. Paste your wallet address next to the orange **Deploy** button.
6. Click **Deploy** and confirm the transaction in MetaMask.
7. Once confirmed, click the **Etherscan hyperlink** in the output console and save the contract address.

### 4. Mint Tokens
1. In Remix, expand the deployed contract instance.
2. Under `mint`, enter an address and the amount of tokens to mint.
3. Execute the mint function and confirm the transaction in MetaMask.

### 5. Verify the Contract on Etherscan
1. Download the **Etherscan plugin** from the bottom-left plug icon in Remix.
2. Create an account and API key at [Etherscan](https://etherscan.io/).
3. In Remix, click the **Etherscan icon** on the left sidebar.
4. Select `MyToken.sol` and input the deployed contract address.
5. Enter your API key and wallet address as the initial owner.
6. Click **Verify**. The contract should be verified on testnet Etherscan within 2 minutes.

## Conclusion
Once verified, you can interact with your contract directly on Etherscan, enabling public access to its functions. 🎉

