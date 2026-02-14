# Chapter 7: Solana Tools

This chapter introduces token creation and management tools on the Solana chain, including token creation, pool addition, market cap management, and other features.

## Table of Contents

### Wallet & Preparation
- [Phantom Wallet Installation Tutorial](phantom.md) - Phantom wallet installation and configuration
- [Batch Generate Wallet Addresses](createwallet.md) - Batch create Solana wallets
- [Solana Vanity Wallet Address Generation Tutorial](vanityaddress.md) - Generate custom prefix addresses

### Token Creation
- [One-Click Token Creation Tutorial](standard.md) - Standard SPL token creation
- [Create Tax Token (Token2022) Tutorial](create2022.md) - Token2022 tokens
- [Create Vanity Token Tutorial](createvanitytoken.md) - Custom token addresses
- [Token Clone Tutorial](clonetoken.md) - Clone existing tokens
- [Update Token Info](upload.md) - Modify token metadata

### Token Management
- [Permission Management (Mint, Freeze, Revoke)](control.md) - Token permission control
- [Burn Token, Burn Pool Tutorial](burn.md) - Token burn operations
- [Extract Fee Tutorial](taxclaim.md) - Extract tax token fees
- [Rent Recovery Tutorial](rent.md) - Recover account rent

### Liquidity Pools
- [Create Liquidity Pool Tutorial](createpool.md) - Create AMM pools
- [CPMM Add Pool Tutorial](raydium.md) - Raydium CPMM pools
- [Create Raydium CLMM Stable Pool Tutorial](clmm.md) - CLMM concentrated liquidity
- [DLMM Stable Pool Creation Tutorial](meteora.md) - Meteora DLMM pools
- [Market ID Query Tutorial](findmarket.md) - Query market IDs
- [Low-Cost Market ID Creation Tutorial](market.md) - Create Market at low cost
- [Add/Remove Liquidity Tutorial](managepool.md) - Liquidity management
- [Burn Pool Tutorial](burnlp.md) - Burn LP tokens

### Pump.fun Related
- [Token Creation and Bundle Buy Tutorial](createpump.md) - Pump.fun token creation
- [One-Click Token Creation and Bundle Buy Tutorial](createbonk.md) - Bundle buy
- [One-Click Bundle Sell Tutorial](sellpump.md) - Batch sell
- [Pump.fun Market Cap Management Bot Tutorial](swapbotpump.md) - Pump market cap management

### Batch Tools
- [Batch Airdrop Tutorial](batch-transfer.md) - Token batch transfer
- [Batch Collection Tutorial](gather.md) - Token collection
- [Token Snapshot Tutorial](snapshottoken.md) - Holder address snapshot
- [New Address Buy Tool Tutorial](newbuy.md) - New wallet purchases

### Market Cap Management
- [Market Cap Management Bot Tutorial](swapbot.md) - Basic market cap management
- [Batch Trading/Market Cap Management Tutorial](swapbotbonk.md) - Advanced market cap management
- [Create Presale, Private Sale Tutorial](createmint.md) - Presale features

---

## Phantom Wallet Installation Tutorial

Phantom is the most popular wallet in the Solana ecosystem, supporting Chrome, Firefox, Edge, and other browsers.

### Installation Steps

1. Visit <https://phantom.app/>
2. Download and install the browser plugin
3. Create new wallet or import existing wallet
4. Safely store mnemonic phrase

---

## One-Click Token Creation Tutorial

Create standard SPL tokens on Solana.

### Creation Parameters

- Token name
- Token symbol
- Decimals (recommended 9)
- Total supply
- Logo image

### Important Notes

- Requires small amount of SOL for Gas fees and account rent
- Token info stored on-chain requires additional SOL

---

## Create Tax Token (Token2022) Tutorial

Token2022 is Solana's new generation token standard, supporting transfer tax functionality.

### Features

- Built-in transfer tax
- Configurable tax rate
- Whitelist tax exemption

---

## Create Liquidity Pool Tutorial

Create token trading pools on Raydium.

### Preparation

1. Create Market ID (OpenBook)
2. Prepare tokens and SOL
3. Set initial price

### Creation Steps

1. Select token pair
2. Set initial liquidity
3. Confirm creation

---

## Market Cap Management Bot Tutorial

Automated market cap management tool to help maintain token price.

### Feature Description

- Automatic buy/sell
- Price range setting
- Multi-wallet rotation
- Trading frequency control

---

## Batch Airdrop Tutorial

Batch send tokens to multiple addresses.

### Usage Method

1. Prepare recipient address list
2. Set quantity for each address
3. Confirm and execute batch transfer

### Fee Description

Each transfer requires small amount of SOL for Gas fees
