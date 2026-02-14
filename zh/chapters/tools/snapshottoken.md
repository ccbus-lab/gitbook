# 代币快照教程

快速获取BSC链代币的持仓数据

### **什么是代币快照？**

代币**快照** ，通俗点说，就是在区块链上“拍一张照”——记录某一时刻（或某个区块高度）、某个代币的所有持仓地址，以及每个地址的持仓数量。

### **为什么要对代币进行快照？**

  1. **空投 / 分发奖励：** 按快照上的持币量发放代币或 NFT，防止在发放前有人临时买入套现。

  2. **治理投票：** 确定在某一时刻谁有投票资格及其投票权重（基于当时持币量）。

  3. **数据分析与合规审计：** 统计持币分布、识别大户/交易所/燃烧地址、评估去中心化程度。

  4. **迁移/空转准备：** 项目从旧合约迁移到新合约时，用快照保证老用户权益完整转移。


可以说，快照能保证“按某一时刻谁持有多少来发放权益”的公平性与可溯源性。

### **代币快照支持哪些区块链？**

目前PandaTool开发了针对多链的代币快照工具，支持包括：BSC、ETH、Base、Polygon、Arbitrum等EVMs链，以及针对Solana代币的快照工具

  * Solana代币快照：<https://solana.ccbus.cc/snapshotToken>


### **如何对代币进行快照？**

为了满足用户对于代币快照的需求，PandaTool开发了针对于BSC、ETH等区块链代币的快照工具，任何人只需要几个简单的步骤，就可以快速进行代币快照，以获取代币持仓信息。

**1、打开PandaTool**

首先，我们打开PandaTool的代币快照工具：<https://ccbus.cc/contract-inspector>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGjkVs6T5ZVyOpIZxaQg8%252F1%25E6%2589%25BE%25E5%2588%25B0%25E5%25B7%25A5%25E5%2585%25B7.png%3Falt%3Dmedia%26token%3Df1442089-07c3-4c9a-bdbf-66fa80cb5548&width=768&dpr=3&quality=100&sign=899fd11b&sv=2)

**2、选择链并输入代币**

接下来，您需要输入要快照的代币合约地址，并且选择区块链。例如我要抓取/快照BSC链USDT的持币地址，我就选择BSC，并且输入USDT的合约地址：0x55d398326f99059fF775485246999027B3197955，然后点击`**搜索**`按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F5JdXgRYD6kGVp8XqMHos%252F2%25E9%2593%25BE%25E4%25B8%258E%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D9e127272-866f-46b1-987c-8a10ebffc5c1&width=768&dpr=3&quality=100&sign=ab6b1a19&sv=2)

**3、筛选快照数据**

搜索之后，我们就能看到基本的代币数据了。接下来，要对这些数据进行筛选

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F7986LevKZRPmQbqkZ8vb%252F3%25E7%25AD%259B%25E9%2580%2589.png%3Falt%3Dmedia%26token%3Da1a1dd20-de74-4661-a4f6-da77d6deced7&width=768&dpr=3&quality=100&sign=fa7d4fdd&sv=2)

  * **持仓地址筛选：** TOP100的意思，就是快照前100持币者的地址。TOP500就是前500的持仓地址，以此类推

  * **自定义最低代币持有量：** 筛选出持有这个数量以上的地址。假设您填写100，意味着持币数量少于100的地址将**不会** 被快照


**4、快照导出**

当我们设定好筛选的数据后，再选择导出格式：

  * **CSV：** 类似于Excel表格，可以在批量转账的时候用来上传识别地址。

  * **TXT：** 文本格式，便于查看与复制


如果您拿到快照数据是为了进行批量空投，就选择CSV格式导出。如果您拿到快照数据是为了看一下，那么TXT格式比较合适。

确定好格式后，我们点击“立即快照”按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FSerCNAPRQaeIgYZuo4hh%252F4%25E5%25AF%25BC%25E5%2587%25BA.png%3Falt%3Dmedia%26token%3Dc9a43ac6-5650-48d2-b260-4c8614496f7e&width=768&dpr=3&quality=100&sign=d572295f&sv=2)

之后，浏览器会提示您下载一个文档，这个就是您导出的快照数据

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjBgCPcxgYG6sruWt1g9F%252F5%25E4%25BF%259D%25E5%25AD%2598.png%3Falt%3Dmedia%26token%3D975899df-1c4b-4116-bb89-9bc701f6666a&width=768&dpr=3&quality=100&sign=f0ef452&sv=2)

接下来就能看到一些快照数据了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6ZLeoLkDRBIia1qVVGNW%252Ftxt%25E6%25A0%25BC%25E5%25BC%258F%25E7%259A%2584%25E6%2595%25B0%25E6%258D%25AE.png%3Falt%3Dmedia%26token%3Da14e20f4-112e-4bb5-9666-da6f8e4f93de&width=768&dpr=3&quality=100&sign=4a89d93c&sv=2)

### **代币快照注意事项**

**1、PandaTool的代币快照工具需要收费吗？**

  * **答：** 不收费，该工具是免费使用的


**2、快照的数据准确吗？**

  * **答：** 代币快照的数据是基于某一个区块高度或者时间的，过了这个时间，数据可能就会有变化。


**3、代币快照支持Solana区块链吗？**

  * **答：** 支持的，可以在这里操作：<https://solana.ccbus.cc/snapshotToken>


当然，如果您对代币快照这个工具还有哪些问题，可以直接在Telegram群里咨询志愿者：<https://t.me/pandatool>
