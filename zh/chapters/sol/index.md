# 第七章：Solana工具

本章介绍Solana链上的代币创建和管理工具，包括发币、加池、市值管理等功能。

## 目录

### 钱包与准备
- [幻影钱包Phantom安装教程](phantom.html) - Phantom钱包安装配置
- [批量生成钱包地址](createwallet.html) - 批量创建Solana钱包
- [Solana靓号钱包地址生成教程](vanityaddress.html) - 生成自定义前缀地址

### 代币创建
- [一键发币教程](standard.html) - 标准SPL代币创建
- [创建税率代币(Token2022)教程](create2022.html) - Token2022代币
- [创建靓号代币教程](createvanitytoken.html) - 自定义代币地址
- [代币克隆教程](clonetoken.html) - 克隆已有代币
- [更新代币资料](upload.html) - 修改代币元数据

### 代币管理
- [权限管理(增发、冻结、弃权)](control.html) - 代币权限控制
- [销毁代币、烧池教程](burn.html) - 代币销毁操作
- [提取手续费教程](taxclaim.html) - 提取税率代币手续费
- [租金回收教程](rent.html) - 回收账户租金

### 流动性池
- [创建流动资金池教程](createpool.html) - 创建AMM池
- [CPMM加池子教程](raydium.html) - Raydium CPMM池
- [创建Raydium CLMM稳定池教程](clmm.html) - CLMM集中流动性
- [DLMM稳定池创建教程](meteora.html) - Meteora DLMM池
- [Market ID查询教程](findmarket.html) - 查询市场ID
- [市场ID低成本创建教程](market.html) - 低成本创建Market
- [添加/移除流动性教程](managepool.html) - 流动性管理
- [烧池子教程](burnlp.html) - 销毁LP代币

### Pump.fun相关
- [发币与捆绑买入教程](createpump.html) - Pump.fun发币
- [一键发币与捆绑买入教程](createbonk.html) - 捆绑买入
- [一键捆绑卖出教程](sellpump.html) - 批量卖出
- [Pump.fun市值管理机器人教程](swapbotpump.html) - Pump市值管理

### 批量工具
- [批量空投教程](batch-transfer.html) - 代币批量转账
- [批量归集教程](gather.html) - 代币归集
- [代币快照教程](snapshottoken.html) - 持币地址快照
- [新地址买入工具教程](newbuy.html) - 新钱包买入

### 市值管理
- [市值管理机器人教程](swapbot.html) - 基础市值管理
- [批量交易/市值管理教程](swapbotbonk.html) - 高级市值管理
- [创建预售、私募教程](createmint.html) - 预售功能

---

## 幻影钱包Phantom安装教程

Phantom是Solana生态最流行的钱包，支持Chrome、Firefox、Edge等浏览器。

### 安装步骤

1. 访问 <https://phantom.app/>
2. 下载并安装浏览器插件
3. 创建新钱包或导入已有钱包
4. 妥善保管助记词

---

## 一键发币教程

在Solana上创建标准SPL代币。

### 创建参数

- 代币名称
- 代币符号
- 精度（推荐9）
- 发行总量
- Logo图片

### 注意事项

- 需要少量SOL作为Gas费和账户租金
- 代币资料存储在链上，需要额外SOL

---

## 创建税率代币(Token2022)教程

Token2022是Solana新一代代币标准，支持转账税率功能。

### 功能特点

- 内置转账税率
- 税率可配置
- 白名单免税

---

## 创建流动资金池教程

在Raydium创建代币交易池。

### 准备工作

1. 创建Market ID（OpenBook）
2. 准备代币和SOL
3. 设置初始价格

### 创建步骤

1. 选择代币对
2. 设置初始流动性
3. 确认创建

---

## 市值管理机器人教程

自动化市值管理工具，帮助维护代币价格。

### 功能说明

- 自动买卖
- 价格区间设置
- 多钱包轮换
- 交易频率控制

---

## 批量空投教程

将代币批量发送给多个地址。

### 使用方法

1. 准备接收地址列表
2. 设置每个地址的数量
3. 确认并执行批量转账

### 费用说明

每笔转账需要少量SOL作为Gas费
