# Solana代币快照教程

对Solana代币进行快照的教程

### **什么是代币快照？**

代币**快照** ，通俗点说，就是在区块链上“拍一张照”——记录某一时刻（或某个区块高度）、某个代币的所有持仓地址，以及每个地址的持仓数量。

### **为什么要对代币进行快照？**

  1. **空投 / 分发奖励：** 按快照上的持币量发放代币或 NFT，防止在发放前有人临时买入套现。 

  2. **治理投票：** 确定在某一时刻谁有投票资格及其投票权重（基于当时持币量）。 

  3. **数据分析与合规审计：** 统计持币分布、识别大户/交易所/燃烧地址、评估去中心化程度。 

  4. **迁移/空转准备：** 项目从旧合约迁移到新合约时，用快照保证老用户权益完整转移。


可以说，快照能保证“按某一时刻谁持有多少来发放权益”的公平性与可溯源性。

### **如何对代币进行快照？**

为了满足用户对于代币快照的需求，PandaTool开发了针对于Solana代币的快照工具，任何人只需要几个简单的步骤，就可以快速进行代币快照，以获取代币持仓信息。

#### **1、打开PandaTool**

首先，我们打开PandaTool的代币快照工具：<https://solana.pandatool.org/snapshotToken>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FlsVFVF9d37oDi3HiHKgy%252F1%25E6%2589%25BE%25E5%2588%25B0%25E5%25BF%25AB%25E7%2585%25A7%25E5%25B7%25A5%25E5%2585%25B7.png%3Falt%3Dmedia%26token%3Db7db6efe-d072-4c2f-a835-01f6634fad21&width=768&dpr=3&quality=100&sign=6e5b8800&sv=2)

#### **2、输入代币合约地址**

之后，我们在输入框填入要抓取的代币合约地址，如：XsDoVfqeBukxuZHWhdvWHBhgEHjGNst4MLodqsJHzoB，点击**搜索**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FeQIkb2p2K76YTnDKTI9q%252F2%25E5%2590%2588%25E7%25BA%25A6%25E5%259C%25B0%25E5%259D%2580%252B%25E6%2590%259C%25E7%25B4%25A2.png%3Falt%3Dmedia%26token%3D9c2ccb0a-d46c-447b-8bd9-be37031dc7d8&width=768&dpr=3&quality=100&sign=c1963908&sv=2)

#### **3、筛选快照数据**

搜索之后，就可以看到代币的名称、符号以及持币人数等等。接下来，就要筛选一下快照的数据了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FddAsNZJ6BBOuzO0pFkKi%252F3%25E6%2595%25B0%25E6%258D%25AE%25E7%25AD%259B%25E9%2580%2589.png%3Falt%3Dmedia%26token%3Dbd113ada-2f63-4bee-bbec-a00ffba79853&width=768&dpr=3&quality=100&sign=29ca1564&sv=2)

  * **持仓地址筛选：** TOP100的意思，就是快照前100持币者的地址

  * **自定义最低代币持有量：** 筛选出持有这个数量以上的地址。假设您填写100，意味着持币数量少于100的地址将**不会** 被快照


#### **4、快照导出**

当我们设定好筛选的数据后，再选择导出格式：

  * **CSV：** 类似于Excel表格，可以在批量转账的时候用来上传识别地址。

  * **TXT：** 文本格式，便于查看与复制


如果您拿到快照数据是为了进行批量空投，就选择CSV格式导出。如果您拿到快照数据是为了看一下，那么TXT格式比较合适。

确定好格式后，我们点击“立即快照”按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FiLU2ZVFQaRbO3tzKD4nH%252F4%25E7%25AB%258B%25E5%258D%25B3%25E5%25AF%25BC%25E5%2587%25BA.png%3Falt%3Dmedia%26token%3Dc2c5ae9d-d47e-4f56-8799-48bea270004b&width=768&dpr=3&quality=100&sign=e0cdfb8e&sv=2)

之后，浏览器会提示您下载一个文档，这个就是您导出的快照数据

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FDm9z9SB8DX4Nv6bsTP4I%252F5%25E5%25AF%25BC%25E5%2587%25BA%25E6%2595%25B0%25E6%258D%25AE.png%3Falt%3Dmedia%26token%3D23dc852d-d879-4d4e-a087-844794bc4b3d&width=768&dpr=3&quality=100&sign=120307b&sv=2)

接下来就能看到一些快照数据了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FocqqZB3eAzJgzMAxqW6M%252F6%25E5%25BF%25AB%25E7%2585%25A7%25E6%2595%25B0%25E6%258D%25AE-csv.jpg%3Falt%3Dmedia%26token%3D29bad67c-2b9e-409b-999f-2eea01fb107e&width=768&dpr=3&quality=100&sign=33306033&sv=2)

### **代币快照注意事项**

**1、PandaTool的代币快照工具需要收费吗？**

  * **答：** 不收费，该工具是免费使用的


**2、快照的数据准确吗？**

  * **答：** 代币快照的数据是基于某一个区块高度或者时间的，过了这个时间，数据可能就会有变化。


**3、代币快照支持BSC链、ETH链吗？**

  * **答：** 支持的，可以在这里操作 <https://pandatool.org/#/contractCheck/snapshotToken?lang=zh-CN>


当然，如果您对代币快照这个工具还有哪些问题，可以直接在Telegram群里咨询志愿者：<https://t.me/pandatool>
