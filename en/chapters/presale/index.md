# Chapter 5: Presale Tools

This chapter introduces PandaTool's token presale tools, including standard Mint presale, add-pool presale, and donation presale features.

---

## Create Standard Token Mint Presale Tutorial

100% decentralized presale contract creation tutorial

**What is Standard Mint Presale?**

Simply put, it is a presale through the Mint method. The project team transfers a certain amount of tokens to the presale contract address. After the presale is opened, users transfer BNB to the presale contract address, and the presale contract will automatically give tokens to users according to the set ratio.

Note: The prerequisite for creating a presale is that you must first create a token. Without a token, you cannot presale.

### I. Presale Feature Description

  * **No Frontend:** No webpage needed, pure contract support, 100% **decentralized**
  * **Transfer = Presale:** Users transfer BNB to `presale contract` and **automatically** receive tokens
  * **No Claiming:** Users participating in presale do **not need** to manually claim tokens
  * **Custom Functions:** Project team can **modify** presale price and portion quantity through console after presale starts
  * **No Soft/Hard Cap:** No concept of soft or hard cap, only total presale quantity (portions x quantity per portion)

### II. Important Notes

  * During standard token presale, someone may add liquidity pool early
  * Recommend using manual trading enable function to prevent pool trading
  * Do not add presale address to blacklist, otherwise trading is impossible

### III. Standard Mint Presale Creation Tutorial

#### 1. Connect Wallet (Experienced users can skip)

First, open the presale creation website: <https://www.pandatool.org/#/presale/simpleMint>, click connect wallet in the upper right corner

#### 2. Fill in Presale Parameters

After wallet connection is successful, we create the presale through the PandaTool visual page and fill in the corresponding presale parameters:

  * **Presale Name:** Any name, e.g., Presale, Chinese not supported, only English
  * **Presale Token Address:** The token contract address to presale (prerequisite is having a token)
  * **Price Per Portion:** How much to pay per presale portion, minimum price is 0.001 (BNB or ETH)
  * **Quantity Per Portion:** How many tokens in each presale portion
  * **Total Portions:** Total number of portions available for presale (quantity per portion x total portions <= total token supply)
  * **Max Portions Per Transaction:** Maximum portions that can be bought at once
  * **Max Portions Per Wallet:** Maximum portions a single wallet address can buy

After filling in parameters, click Create Contract, a prompt will pop up for you to confirm again

#### 3. Presale Console Operations

After successful creation, we enter the console: <https://www.pandatool.org/#/presale/console>, to see how to operate this presale

  * **Presale Control**
    * **Transfer Ownership**: Transfer contract permissions to others
    * **Enable Presale:** Click and confirm with wallet to enable presale
    * **Withdraw Tokens from Contract:** Can withdraw value coins and tokens from the presale contract

  * **Parameter Control**
    * **Modify Price Per Portion:** Modify presale price, minimum 0.001
    * **Modify Quantity Per Portion:** Modify quantity per portion
    * **Modify Total Portions:** Modify total presale portions based on actual situation
    * **Modify Max Portions Per Mint:** Modify single presale limit as needed
    * **Modify Max Portions Per Wallet:** Modify single wallet presale limit as needed

#### 4. How Does Presale Start and End?

**1) Enable Presale:** In `Presale Console` click **Enable Presale**, there will be two confirmations. First is authorization confirmation, second will ask you to **transfer** enough tokens into the presale contract

**2) End Presale:** If you want to end the presale early, just use the "Withdraw Tokens from Contract" function to withdraw all tokens from the contract, then presale is no longer possible

### IV. FAQ

  * **Why did enabling presale fail?**
    * **Insufficient tokens in wallet:** If your set presale [quantity per portion x total portions = 10000 tokens], but your wallet only has 9000 tokens, it will prompt presale failure
    * **Presale contract not whitelisted:** If the presale contract address is not added to the token whitelist, presale may fail to enable
    * **Token contract has holding limit:** If the previous token contract has maximum holding limit, and your presale quantity exceeds this limit, tokens cannot be transferred to the presale address, causing presale enable failure

  * **After presale is enabled, why do user transfer presales fail?**
    * **Price issue:** If the user's BNB transfer amount is less than the price per portion, it will fail, BNB returned
    * **Gas issue:** If gas fee is set too low, presale may fail
    * **Contract total issue:** If the contract address doesn't have enough tokens for presale, users naturally cannot participate
    * **Portion input error:** Max portions per wallet must be greater than or equal to max portions per transaction
    * **Presale limit reached:** If single transaction or single wallet presale limit is reached, cannot buy more
    * **Presale completed:** If you set total presale portions as 10, and 10 portions have been reached, presale is complete

  * **Can I presale using wBNB or USDT?**
    * Not supported, currently only native token presales are supported. BSC chain uses BNB, Base chain uses ETH

  * **Batch presale and actual portion distribution**
    * **Integer multiple presale:** If 1 portion is 100 tokens, price 0.03 BNB. User transfers 0.06 BNB, receives 200 tokens; user transfers 0.09 BNB, receives 300 tokens, and so on
    * **Non-integer multiple presale:** Same 1 portion 100 tokens, price 0.03 BNB. If user transfers 0.04 BNB, receives 100 tokens, excess 0.01 BNB returned

  * **Is there a max/min limit for presale?**
    * **Minimum limit:** Single address single presale, minimum limit is your set minimum price, below this price cannot presale
    * **Maximum limit:** Both single transaction and single wallet have separate maximum limits

If you have questions or unclear points, please join the official Telegram group: <https://t.me/PandaTool>

---

## Create Token Mint Add-Pool Presale Tutorial

Presale = Add Pool, Automatic LP Distribution, Everyone is a Market Maker

**What is Mint Add-Pool Presale?**

Simply put, it is a presale through the Mint method, and the received BNB is added to the liquidity pool. The project team transfers a certain amount of tokens to the presale contract address. After the presale is opened, users transfer BNB to the presale contract address, and the presale contract will automatically add tokens and BNB together to PancakeSwap to form a liquidity pool, and give LP to users.

The difference from standard presale is that add-pool presale **only gives LP to users**, to establish the foundation for the project's subsequent development.

### I. Mint Add-Pool Presale Feature Description

  * **Add-Pool Presale:** Automatically **adds liquidity** during presale, users can only receive `LP`, not tokens
  * **No Frontend:** No webpage needed, pure contract support, 100% **decentralized**
  * **Transfer = Presale:** Users transfer BNB to `presale contract` and **automatically** receive LP
  * **Custom Functions:** Project team can **modify** presale price and portion quantity through console after presale starts
  * **No Soft/Hard Cap:** No concept of soft or hard cap, only total presale quantity (portions x quantity per portion)

### II. Important Notes

  * Please ensure token **has not** added pool before presale is enabled
  * Standard token contracts **not recommended**
  * Other token contracts should not start trading (if manual launch function exists)
  * After presale creation, please add presale address to token address **whitelist**
  * If your token contract has manual launch function but no whitelist function, do not use
  * **Do not remove pool** during presale. Once pool is removed, subsequent presales may fail

### III. Mint Presale Creation Tutorial

#### 1. Connect Wallet (Experienced users can skip)

First, open the presale creation website: <https://www.pandatool.org/#/presale/mintAddSale>, click connect wallet in the upper right corner

#### 2. Fill in Presale Parameters

After wallet connection is successful, we create the presale through the PandaTool visual page and fill in the corresponding presale parameters:

  * **Presale Name**: Name your presale, English only
  * **Presale Token Address**: Your token contract address to presale (prerequisite is having a token)
  * **Price Per Portion:** Presale price per portion, minimum unit is 0.001
  * **Quantity Per Portion**: How many tokens per portion
  * **Total Portions:** Total number of portions available for presale (quantity per portion x total portions <= total token supply)
  * **Max Portions Per Transaction:** Maximum portions per single presale
  * **Max Portions Per Wallet:** Maximum portions per wallet
  * **Select Exchange:** BSC selects Pancake, Base chain selects Uniswap
  * **Add-Pool Ratio:** Add liquidity according to set ratio (minimum 50%, maximum 100%), excess BNB or ETH goes to marketing wallet

After filling in parameters, click Create Contract, wallet will pop up for confirmation, wait a few seconds, and you'll be notified that presale creation is complete

#### 3. Presale Console Operations

After successful creation, we enter the console: <https://www.pandatool.org/#/presale/console>

  * **Permission Control**
    * **Transfer Ownership**: Transfer contract permissions to others
    * **Enable Trading:** Click button and confirm with wallet to start presale
    * **Withdraw Tokens from Contract:** Can withdraw BNB/ETH and tokens from the presale contract

  * **Parameter Control**
    * **Modify Price Per Portion:** Modify presale price, minimum 0.001
    * **Modify Quantity Per Portion:** Modify quantity per portion
    * **Modify Total Portions:** Modify total presale portions based on actual situation
    * **Modify Max Portions Per Mint:** Modify single presale limit as needed
    * **Modify Max Portions Per Wallet:** Modify single wallet presale limit as needed

  * **Pool Control**
    * **Modify Marketing Wallet:** Marketing wallet defaults to token creation wallet, can be modified as needed
    * **Modify Add-Pool Ratio:** Minimum 50%, maximum 100%, can be modified within this range

#### 4. How Does Presale Start and End?

**1) Add Whitelist:** After presale creation, add the presale contract to your token contract's tax whitelist

**2) Enable Presale:** In `Presale Console` click **Start Trading**, there will be two confirmations. First is authorization confirmation, second will ask you to **transfer** enough tokens into the presale contract

**3) End Presale:** If you want to end the presale early, just use the "Withdraw Tokens from Contract" function to withdraw all tokens from the contract, then presale is no longer possible

### IV. FAQ

  * **How to understand add-pool ratio?**
    * If you select 100%, it means all BNB from each user's presale will be added to the pool as liquidity; if you select 50%, half of the user's presale BNB goes to marketing wallet, half is added to the pool

  * **What is the marketing wallet for?**
    * Marketing wallet defaults to the token creation wallet, mainly to receive users' excess BNB when you select the add-pool mode

If you have questions or unclear points, please join the official Telegram group: <https://t.me/PandaTool>

---

## Create Token Mint Donation Presale Tutorial

Presale = Add Pool, Automatic LP Distribution, Everyone is a Market Maker

**What is Mint Donation Presale?**

Simply put, it is a presale through the Mint method, and the received BNB is donated to celebrity wallets. Specifically, the project team transfers a certain amount of tokens to the presale contract address. After the presale is opened, users transfer BNB to the presale contract address, and the presale contract will automatically give a portion of tokens or BNB to celebrity wallets according to the set ratio, such as Vitalik's wallet address, convenient for subsequent promotion.

Different from standard presale and add-pool presale, donation presale leverages celebrity marketing, proactively adding wallet addresses like Vitalik's to the project, creating new narratives for the project, facilitating subsequent promotion.

### I. Mint Donation Presale Feature Description

  * **Donation Presale:** Give BNB or tokens to celebrity wallets during presale
  * **No Frontend:** No webpage needed, pure contract support, 100% **decentralized**
  * **Transfer = Presale:** Users transfer BNB to `presale contract` and **automatically** receive tokens
  * **Custom Functions:** Project team can **modify** presale price and portion quantity through console after presale starts
  * **No Soft/Hard Cap:** No concept of soft or hard cap, only total presale quantity (portions x quantity per portion)

### II. Important Notes

  * Vitalik may dump later, be aware of the risk
  * Standard token contracts **not recommended** for presale, as someone may add pool during presale
  * Other token contracts should not start trading (if manual launch function exists)

### III. Donation Presale Creation Tutorial

#### 1. Connect Wallet (Experienced users can skip)

First, open the donation presale creation website: <https://www.pandatool.org/#/presale/mintDonate>, click connect wallet in the upper right corner

#### 2. Fill in Presale Parameters

After wallet connection is successful, we create the presale through the PandaTool visual page and fill in the corresponding presale parameters:

  * **Presale Name**: Name your presale, English only
  * **Presale Token Address**: Your token contract address to presale (prerequisite is having a token)
  * **Price Per Portion:** Presale price per portion, minimum unit is 0.001
  * **Quantity Per Portion**: How many tokens per portion
  * **Total Portions:** Total number of portions available for presale (quantity per portion x total portions <= total token supply)
  * **Max Portions Per Transaction:** Maximum portions per single presale
  * **Max Portions Per Wallet:** Maximum portions per wallet
  * **Donate BNB/ETH Ratio:** What ratio (0~100) of presale BNB/ETH to donate to an address
  * **BNB/ETH Receiving Address:** Which address to donate BNB/ETH to (usually celebrity wallet)
  * **Donate Token Ratio:** What ratio (0~100) of presale tokens to donate to an address
  * **Token Receiving Address:** Which address to donate tokens to (usually celebrity wallet)

Vitalik's wallet address: 0xd8da6bf26964af9d7eed9e03e53415d37aa96045

After filling in parameters, click Create Contract, wallet will pop up for confirmation, wait a few seconds, and you'll be notified that presale creation is complete

#### 3. Presale Console Operations

After successful creation, we enter the console: <https://www.pandatool.org/#/presale/console>

  * **Permission Control**
    * **Transfer Ownership**: Transfer contract permissions to others
    * **Enable Trading:** Click button and confirm with wallet to start presale
    * **Withdraw Tokens from Contract:** Can withdraw BNB/ETH and tokens from the presale contract

  * **Parameter Control**
    * **Modify Price Per Portion:** Modify presale price, minimum 0.001
    * **Modify Quantity Per Portion:** Modify quantity per portion
    * **Modify Total Portions:** Modify total presale portions based on actual situation
    * **Modify Max Portions Per Mint:** Modify single presale limit as needed
    * **Modify Max Portions Per Wallet:** Modify single wallet presale limit as needed

  * **Donation Control**
    * **Modify BNB/ETH Receiving Wallet:** Reset the wallet address receiving donations
    * **Modify BNB/ETH Donation Ratio:** Reset the donation ratio
    * **Modify Token Receiving Wallet:** Reset the wallet address receiving donations
    * **Modify Token Donation Ratio:** Reset the donation ratio

#### 4. How Does Presale Start and End?

**1) Add Whitelist:** After presale creation, add the presale contract to your token contract's tax whitelist

**2) Enable Presale:** In `Presale Console` click **Start Trading**, there will be two confirmations. First is authorization confirmation, second will ask you to **transfer** enough tokens into the presale contract

**3) End Presale:** If you want to end the presale early, just use the "Withdraw Tokens from Contract" function to withdraw all tokens from the contract, then presale is no longer possible

### IV. FAQ

  * **What is the donation ratio range?**
    * Minimum 0% donation, maximum 100% donation

  * **What's the difference between donating BNB and donating tokens?**
    * **Donate BNB/ETH:** Project team receives less BNB/ETH
    * **Donate Tokens:** Users receive fewer tokens

If you have questions or unclear points, please join the official Telegram group: <https://t.me/PandaTool>
