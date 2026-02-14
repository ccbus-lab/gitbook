# 第四章：实用信息

本章包含加密货币开发和使用过程中的实用信息，包括钱包安装、网络配置、测试币获取等内容。

## 目录

- [小狐狸插件安装教程](metamask.html) - MetaMask钱包安装与配置
- [欧易OKX Web3钱包发币教程](okx.html) - 使用OKX Web3钱包发币
- [公链配置参数](parameter.html) - 各公链网络配置参数
- [测试币水龙头大全](faucet.html) - 各链测试币获取渠道
- [交易所路由Router合约](jiao-yi-suo-lu-you-router.html) - DEX路由合约地址
- [主流币合约地址](smart-contract.html) - 主流代币合约地址汇总
- [代币与LP链上解锁教程](unlock.html) - 链上解锁操作指南

---

## 小狐狸插件安装教程

*前置条件：一定要会科学上网

### 一、浏览器安装

电脑安装谷歌浏览器，下载链接如下：

  * Google Chrome windows 64位：https://www.chromedownloads.net/chrome64win/
  * Google Chrome windows 32位：https://www.chromedownloads.net/chrome32win/
  * Google Chrome mac版：https://www.chromedownloads.net/chrome64osx/

或者使用360软件管家下载chrome稳定版

### 二、配置MetaMask钱包

**1.安装小狐狸钱包插件**

打开谷歌应用商店 <https://chrome.google.com/webstore?hl=zh-CN>，找到MetaMask钱包，进行安装。添加成功之后，将图标固定在谷歌浏览器上方。

### 三、配置币安链网络

MetaMask是默认以太坊网络的，因此要自己配置一个币安链网络，点击"添加网络"，可以看到有默认币安链的选项，直接添加即可。

*如果要用币安测试链，需要配置币安测试链网络：

- 网络名称（自定义）：bsc-testnet
- 新增RPC URL：https://data-seed-prebsc-1-s3.binance.org:8545/
- 链ID：97
- 符号（选填）：BNB
- 测试链浏览器：https://testnet.bscscan.com

注意：生成钱包时请隐藏好自己的助记词和私钥，这是绝对不可以泄露和丢失的，非常重要

---

## 测试币水龙头大全

### BNB测试币

  * 官方水龙头：<https://testnet.bnbchain.org/faucet-smart>（0.3BNB）
  * **跨链兑换**：<https://bridge.ccbus.cc/>（推荐使用）
  * triangleplatform水龙头：<https://faucet.triangleplatform.com/bnbsmartchain/testnet>（0.001个）

### Sepolia ETH测试币

  * Alchemy水龙头：<https://www.alchemy.com/faucets/ethereum-sepolia>（0.1ETH）
  * **跨链兑换**：<https://bridge.ccbus.cc/>（推荐使用）
  * 谷歌云水龙头：<https://cloud.google.com/application/web3/faucet/ethereum/sepolia>（0.05ETH）

### Base ETH测试币

  * **跨链兑换**：<https://bridge.ccbus.cc/>（推荐使用）
  * Alchemy水龙头：<https://www.alchemy.com/faucets/base-sepolia>（0.1ETH）

### Holesky ETH测试币

  * **跨链兑换**：<https://bridge.ccbus.cc/>（推荐使用）
  * Stakely水龙头：<https://stakely.io/faucet/ethereum-holesky-testnet-eth>（0.1ETH）

### TRON 测试币TRX

  * **跨链兑换**：<https://bridge.ccbus.cc/>（推荐使用）

### Solana测试币SOL

  * **跨链兑换**：<https://bridge.ccbus.cc/>（推荐使用）

---

## 公链配置参数

本节提供各主流公链的网络配置参数，包括链ID、RPC节点、浏览器地址等信息。

---

## 主流币合约地址

本节提供各公链上主流代币的合约地址汇总，方便开发者查询和使用。

---

## 交易所路由Router合约

本节提供各去中心化交易所的路由合约地址，用于代币交易和流动性管理。

---

## 代币与LP链上解锁教程

本节介绍如何在链上解锁已锁定的代币或LP代币。
