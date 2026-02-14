# DeDust加池子(创建流动性)教程

在DeDust上创建AMM资金池

[DeDust](https://dedust.io/)是构建在TON上的去中心化交易所，采用创新的 DeDust 协议 2.0。它注重用户体验、gas 效率和可扩展性，同时开发了跨链桥产品，让用户可以在TON与ETH两条链之间进行无缝对接。

## 为什么选择DeDust

DeDust虽然成立时间不是非常久，但是增长速度很快、用户覆盖度也在迅速上升。据统计，截止到6月22日，DeDust的TVL超过3亿美元，是TON链上排名第一的应用，比第二名STON整整高出6000万美元。

DeDust 通过以下几个独特功能对 TON 区块链上的 DeFi 进行了创新：

  * **资产概念** ：超越传统的单一资产类型，使用允许无缝集成和交换各种资产类型的抽象层，包括来自其他链的原生币和代币。

  * **Vault 系统** ：一组管理不同资产类型的合约，简化交易并实现高效的多跳交换。

  * **池类型** ：提供AMM资金池和稳定币资金池，满足不同资产波动性和交易策略的需求。

  * **工厂合约** ：负责创建池和金库，集中合约管理。

  * **流动性存款合约** ：临时管理流动性存款，提高交易效率。


## DeDust加池子教程

### 1、连接钱包

首先，我们打开DeDust的官网：<https://dedust.io/>，点击右上角`Wallets`，根据提示再点击`Connect Wallet`连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FYrXL5gOWB3Fu7boh0iqb%252F%25E6%2589%25BE%25E5%2588%25B0walets.png%3Falt%3Dmedia%26token%3Dc3222040-6094-43a1-9b3d-2f6f136e8897&width=768&dpr=3&quality=100&sign=c553118b&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVG0Lb8XKK7uLr7L9Prk0%252F%25E9%2580%2589%25E6%258B%25A9connect%2520wallet.png%3Falt%3Dmedia%26token%3D54cf5d56-fbfe-4302-b085-4efb7e8f4c00&width=768&dpr=3&quality=100&sign=57e82615&sv=2)

此时会弹出一列钱包让你选择，如果你安装了`Tonkeeper`，就选择这个（[Tonkeeper安装教程](/ton/tonkeeper)）。如果你安装了OpenMask，就选择OpenMask。一般来说，我们会推荐大家使用Tonkeeper

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fuqsw2UKql9y7q7tze9d7%252F%25E9%2580%2589%25E6%258B%25A9Tonkeeper.png%3Falt%3Dmedia%26token%3Dede88d4d-5edb-4588-89ea-c49984ee2cd5&width=768&dpr=3&quality=100&sign=31621bc5&sv=2)

选择Tonkeeper

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F8ir6i6eWu6jPDofMGKuK%252F%25E9%2580%2589%25E6%258B%25A9%25E6%25B5%258F%25E8%25A7%2588%25E5%2599%25A8%25E6%258F%2592%25E4%25BB%25B6.png%3Falt%3Dmedia%26token%3D472af7c4-6008-4090-9737-918c826622f5&width=768&dpr=3&quality=100&sign=6222bd00&sv=2)

选择浏览器插件版本

然后会弹出钱包插件，点击`连接钱包`即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FuSZ6sCEQO0nPd00JAjvK%252F%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D1d99a95d-efa8-4c7f-971e-0a7cc17bb542&width=768&dpr=3&quality=100&sign=8c4d48cd&sv=2)

连接成功之后，右上角会出现你的钱包地址，如下图

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FRl19lfMDDV1gqKuLnTMZ%252F%25E6%2598%25BE%25E7%25A4%25BA%25E9%2592%25B1%25E5%258C%2585%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D4bdd5db9-9c11-401f-8dbd-bcee0d3fe4c3&width=768&dpr=3&quality=100&sign=f754b117&sv=2)

钱包连接成功后，接下来我们进行加池操作

### 2、创建流动性

点击页面的`Pools`，或者直接打开页面：<https://dedust.io/pools> ，点击Creat Tool（创建池）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCaQdMDDp1CfWBlgBwsXV%252F%25E7%2582%25B9%25E5%2587%25BBpools.png%3Falt%3Dmedia%26token%3D084ed40b-0036-4be9-b5ea-91c52a396649&width=768&dpr=3&quality=100&sign=2bdbf048&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F7MU3fRmORDxleHVnl440%252F%25E5%2588%259B%25E5%25BB%25BA%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D64ab96b5-5634-4d79-856b-edff80cfc50e&width=768&dpr=3&quality=100&sign=ee2f49ce&sv=2)

创建池

然后在打开的页面中输入你要加池的TON的数量，以及你要加池的`代币地址`与数量

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGjeFDMQ9tzQoLWBvwUsZ%252F%25E8%25BE%2593%25E5%2585%25A5%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F%25E4%25B8%258E%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Ded29a3fa-d3cb-4e88-9b0d-a7cbbab11a6f&width=768&dpr=3&quality=100&sign=5ed18f2e&sv=2)

输入TON数量

输入合约地址并查找代币，并将其输入

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FFHLwz3V0SZtvtyHvPXLh%252F%25E8%25BE%2593%25E5%2585%25A5%25E4%25BB%25A3%25E5%25B8%2581%25E5%2590%2588%25E7%25BA%25A6%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3Dc16b4e20-0c94-4d8f-9bb3-8a8d6e4d14eb&width=768&dpr=3&quality=100&sign=2e54e55a&sv=2)

输入合约地址查找代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F2PwOOIz9jTdSCgEh7vp8%252F%25E6%259F%25A5%25E6%2589%25BE%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D7a31a922-c5f7-4a17-a6f8-ce1bbf327ba6&width=768&dpr=3&quality=100&sign=c876f838&sv=2)

查找并输入代币

之后，我们点击Connect PANDA，进行代币的授权

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Ffj3rZC6XQPmUrsT3NKWt%252F%25E6%258E%2588%25E6%259D%2583%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D6cc6a413-5e98-4e03-b782-4b9122cd563f&width=768&dpr=3&quality=100&sign=369ed73c&sv=2)

点击授权

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FpGuGT7d8KAysYAQCTlJ2%252F%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D1d037c5d-cd2d-43ac-8b69-111ed34e3af9&width=768&dpr=3&quality=100&sign=abc2afde&sv=2)

钱包确认授权

如果钱包确认后，仍然一直在转圈，且超过1分钟，那可能是网卡了。这个时候看一下钱包，如果已经确认支付了费用，那应该就是完成了，此时刷新一下页面就可以了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVVN0kSNpPIlpauuxiGCb%252F%25E5%2588%259B%25E5%25BB%25BApair.png%3Falt%3Dmedia%26token%3D4ee15c40-2150-41e6-bded-d394e9bfb2ef&width=768&dpr=3&quality=100&sign=8a0f1eee&sv=2)

所有的参数填写无误后，我们点击 Create Pair，钱包确认后，就算是创建成功了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FiAWJM3t3aQunL2wNbq1a%252Fpair%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D7485259c-8719-460d-be3d-2d6337e99022&width=768&dpr=3&quality=100&sign=38d426ab&sv=2)

## DeDust加池子注意事项

**1、DeDust上面能看到代币头像吗？**

  * 答：可以的，只要链上有头像，钱包能看到头像，DeDust上就有头像


**2、DeDust创建流动性需要收费吗？**

  * **答：** 在DeDust创建池子，授权的时候需要支付0.1TON，创池子(Creat Pair)的时候需要支出0.5TON左右，所以累积差不多要支出0.6TON左右


如有不明白或者不清楚的地方，请加入官方电报群：<https://t.me/PandaTool>
