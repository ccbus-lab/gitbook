# Chapter 2: EVM Token Creation

This chapter introduces how to create various types of tokens on EVM-compatible chains (such as BSC, ETH, Base, etc.), including standard tokens, dividend tokens, LP dividend tokens, and more.

## Table of Contents

### Basic Tutorials
- [Standard Token Creation Tutorial](standard.md) - Create basic ERC20 tokens
- [Mobile TP Wallet Token Creation Tutorial](tp.md) - Create tokens using TP Wallet
- [Contract Verification Tutorial](verify-and-publish.md) - Contract verification and open source

### Token Types
- [Holder Dividend Token Tutorial](holdreflection.md) - Holder dividend mechanism
- [Multi-function Token Tutorial](simplecontrol.md) - Tokens with control functions
- [314 Protocol Token Tutorial](314.md) - 314 protocol tokens
- [LP Dividend Token Tutorial](lpreflection.md) - LP dividend mechanism
- [LP Dividend + Referral Rewards](lpwithinviter.md) - LP dividend with invitations
- [Black Hole Dividend Token Tutorial](blackhole.md) - Black hole dividend mechanism
- [Holder Compound + Referral Rewards](holdwithinviter.md) - Compound + invitation mechanism
- [LP Burn Token Tutorial](lpburn.md) - LP burn mechanism
- [Holder Power Dividend](holdothers.md) - Power dividend tokens
- [Holder Dividend Tutorial](token-reared.md) - Holder dividend details
- [Mining + Referral Rewards](lpmine.md) - Mining mechanism tokens
- [Custom Token Contracts](stakebuyback.md) - Custom contract features

### Liquidity Management
- [Create Liquidity Pool Tutorial](createliquidity.md) - Add liquidity tutorial
- [Create Stablecoin Pool Tutorial](createv3.md) - V3 stable pools
- [Add/Remove Liquidity Tutorial](lpmanage.md) - Liquidity management
- [Add Pool and Bundle Buy Tutorial](createbuy.md) - Launch with bundled purchases

### Lock and Unlock
- [Create Lock Pool or Lock Token Tutorial](createlock.md) - Lock tutorial
- [Unlock Pool or Token Tutorial](lockmanage.md) - Unlock tutorial

### Trading Tools
- [Token Batch Trading/Market Cap Management Tutorial](swapbot.md) - Market cap management tools

---

## Standard Token Creation Tutorial

Standard tokens are the most basic ERC20 tokens, without complex mechanisms, suitable for beginners.

### Creation Steps

1. **Connect Wallet**: Open PandaTool website, connect MetaMask or other Web3 wallet
2. **Select Chain**: Choose the public chain to create token on (BSC, ETH, Base, etc.)
3. **Fill in Parameters**:
   - Token name
   - Token symbol
   - Total supply
   - Decimals (usually 18)
4. **Create Token**: Confirm parameters and pay fees to create

### Important Notes

- Ensure wallet has enough Gas fees
- Token name and symbol cannot be modified once created
- Recommend testing on testnet first

---

## Holder Dividend Token Tutorial

Holder dividend tokens have a dividend mechanism that automatically distributes rewards to holders.

### Features

- Automatic dividends to token holders
- Dividend currency is the native token
- Configurable dividend ratio

---

## Multi-function Token Tutorial

Multi-function tokens provide more control features, suitable for projects requiring flexible management.

### Feature List

- Trading on/off switch
- Blacklist/Whitelist
- Buy/sell tax rate settings
- Maximum holding limit
- Maximum transaction limit

---

## LP Dividend Token Tutorial

LP dividend tokens distribute part of the transaction tax to liquidity providers.

### Mechanism Description

- Transactions generate tax
- Tax automatically distributed to LP holders
- Incentivizes users to provide liquidity

---

## Create Liquidity Pool Tutorial

Creating a liquidity pool is a necessary step for token trading.

### Operation Steps

1. Prepare tokens and paired currency (such as BNB, USDT)
2. Open DEX (such as PancakeSwap)
3. Select add liquidity
4. Set initial price ratio
5. Confirm addition

### Price Calculation

Initial price = Paired currency amount / Token amount

Example: 1000 USDT + 1000000 tokens = 0.001 USDT/token

---

## Contract Verification Tutorial

Contract verification can increase project transparency and credibility.

### Verification Method

1. Find the contract on blockchain explorer
2. Click "Verify & Publish"
3. Select compiler version
4. Submit source code
5. Wait for verification completion

---

## Token Batch Trading/Market Cap Management Tutorial

Market cap management tools can help project teams maintain token price stability.

### Feature Description

- Batch buy/sell
- Scheduled trading
- Price range maintenance
- Multi-wallet operations
