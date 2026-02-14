# Chapter 4: Practical Info

This chapter contains practical information for cryptocurrency development and usage, including wallet installation, network configuration, test token acquisition, and more.

## Table of Contents

- [MetaMask Installation Tutorial](metamask.md) - MetaMask wallet installation and configuration
- [OKX Web3 Wallet Token Creation Tutorial](okx.md) - Create tokens using OKX Web3 Wallet
- [Public Chain Configuration Parameters](parameter.md) - Network configuration parameters for various chains
- [Test Token Faucet Collection](faucet.md) - Test token acquisition channels for various chains
- [Exchange Router Contracts](jiao-yi-suo-lu-you-router.md) - DEX router contract addresses
- [Mainstream Token Contract Addresses](smart-contract.md) - Contract address collection for mainstream tokens
- [Token and LP On-chain Unlock Tutorial](unlock.md) - On-chain unlock operation guide

---

## MetaMask Installation Tutorial

*Prerequisite: Must be able to access international websites

### I. Browser Installation

Install Google Chrome on your computer. Download links:

  * Google Chrome Windows 64-bit: https://www.chromedownloads.net/chrome64win/
  * Google Chrome Windows 32-bit: https://www.chromedownloads.net/chrome32win/
  * Google Chrome Mac version: https://www.chromedownloads.net/chrome64osx/

Or use software manager to download Chrome stable version

### II. Configure MetaMask Wallet

**1. Install MetaMask Wallet Plugin**

Open the Google Chrome Web Store <https://chrome.google.com/webstore>, find MetaMask wallet, and install it. After successful addition, pin the icon to the top of the Google Chrome browser.

### III. Configure BSC Network

MetaMask defaults to the Ethereum network, so you need to configure the BSC network yourself. Click "Add Network" and you can see the default BSC option, just add it directly.

*If you need to use BSC testnet, configure the BSC testnet network:

- Network Name (custom): bsc-testnet
- New RPC URL: https://data-seed-prebsc-1-s3.binance.org:8545/
- Chain ID: 97
- Symbol (optional): BNB
- Testnet Explorer: https://testnet.bscscan.com

Note: When creating a wallet, please keep your mnemonic phrase and private key hidden. These should never be leaked or lost, they are extremely important.

---

## Test Token Faucet Collection

### BNB Test Tokens

  * Official Faucet: <https://testnet.bnbchain.org/faucet-smart> (0.3 BNB)
  * **Cross-chain Exchange**: <https://bridge.pandatool.org/> (Recommended)
  * triangleplatform Faucet: <https://faucet.triangleplatform.com/bnbsmartchain/testnet> (0.001)

### Sepolia ETH Test Tokens

  * Alchemy Faucet: <https://www.alchemy.com/faucets/ethereum-sepolia> (0.1 ETH)
  * **Cross-chain Exchange**: <https://bridge.pandatool.org/> (Recommended)
  * Google Cloud Faucet: <https://cloud.google.com/application/web3/faucet/ethereum/sepolia> (0.05 ETH)

### Base ETH Test Tokens

  * **Cross-chain Exchange**: <https://bridge.pandatool.org/> (Recommended)
  * Alchemy Faucet: <https://www.alchemy.com/faucets/base-sepolia> (0.1 ETH)

### Holesky ETH Test Tokens

  * **Cross-chain Exchange**: <https://bridge.pandatool.org/> (Recommended)
  * Stakely Faucet: <https://stakely.io/faucet/ethereum-holesky-testnet-eth> (0.1 ETH)

### TRON Test Tokens TRX

  * **Cross-chain Exchange**: <https://bridge.pandatool.org/> (Recommended)

### Solana Test Tokens SOL

  * **Cross-chain Exchange**: <https://bridge.pandatool.org/> (Recommended)

---

## Public Chain Configuration Parameters

This section provides network configuration parameters for major public chains, including Chain ID, RPC nodes, explorer addresses, and other information.

---

## Mainstream Token Contract Addresses

This section provides a collection of contract addresses for mainstream tokens on various public chains, convenient for developers to query and use.

---

## Exchange Router Contracts

This section provides router contract addresses for various decentralized exchanges, used for token trading and liquidity management.

---

## Token and LP On-chain Unlock Tutorial

This section introduces how to unlock locked tokens or LP tokens on-chain.
