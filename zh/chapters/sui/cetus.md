# Cetus创建集中流动性资金池教程

在Cetus创建CLMM集中流动性资金池

Cetus是SUI区块链生态里最大的去中心化交易所DEX，使用类似于Uniswap V3的算法构建集中性流动性CLMM协议和一系列附属功能，为DeFi用户提供最佳的交易体验和更高的资金效率。

和传统的AMM不同，Cetus 加入了集中流动性的概念，让流动性提供者可以在定制化价格范围内，策略性地分配其资产。这项创新可以大幅度地减少传统AMM池中流动性利用不足的情况，还可以提高效率，并且为流动性提供者大幅提高费用，与PancakeSwap V3、Uniswap V3类似。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FDsu27RIjT6zrEUEd8YiI%252F1.png%3Falt%3Dmedia%26token%3Dc7f75afa-4708-47dd-9874-be5fc7edc354&width=768&dpr=3&quality=100&sign=cf68ee01&sv=2)


注意：本文仅作为教学演示，所涉及到的资金池和代币均**没有任何实际价值** ，大家也不要进行任何形式的交易。如果因此造成资金损失，PandaTool无法对此负责

## 一、创建集中流动性资金池

在Cetus无法创建AMM资金池，只能创建CLMM资金池。

### 1、连接钱包

连接钱包是所有操作的第一步，老手可以直接忽略。我们打开Cetus的官网：<https://app.cetus.zone/>，点击右上角**连接钱包** 按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FSNul0M5955dgKbwMqRIR%252F2.png%3Falt%3Dmedia%26token%3D70e94ce6-9385-4a3d-9c2b-26c502ab993d&width=768&dpr=3&quality=100&sign=4f96c39&sv=2)

之后会弹出一些钱包让你选择，PandaTool推荐选择Suiet钱包，点击连接即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FihDQ1Xcxl8Ow1Jk5XaXk%252F2-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D515c7ba8-bc65-4875-ba41-8ec19b6e274d&width=768&dpr=3&quality=100&sign=23b3b729&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FcRsOhW6PReXz3mhaXCWk%252F3-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Dfc9c3f2b-ac21-4830-9def-70c4b710778f&width=768&dpr=3&quality=100&sign=d20db4dc&sv=2)

点击连接

连接成功后，我们能在右上角看到钱包地址。之后我们点击左上角的**Earn** 按钮，找到**Pools** ，进行加池操作

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F8emtLcKAsfoEXo9l1n7X%252F4-%25E5%258A%25A0%25E6%25B1%25A0polls.png%3Falt%3Dmedia%26token%3Dad182387-abae-4709-8bdc-c45ff0ff7138&width=768&dpr=3&quality=100&sign=6d8a4891&sv=2)

### 2、找到交易对

当然，除了从首页进入以外，我们也可以直接点击链接进入资金池：<https://app.cetus.zone/pool/list> ，在页面的中间位置点击**Create Pool**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FyoEVB02TtXwVqfCB08WW%252F8-%25E5%2588%259B%25E5%25BB%25BA%25E6%25B1%25A0%25E5%25AD%2590.png%3Falt%3Dmedia%26token%3D74321454-380e-4f59-9f1f-8634bd3a5575&width=768&dpr=3&quality=100&sign=82af9d6f&sv=2)

进入我们进行代币选择页面，左边一般是自己发行的土狗币，右边是SUI

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEPSu45TFSEXkx2Xj5vyO%252F9-%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D7c4c469a-be25-44a2-973e-2602517fe2d8&width=768&dpr=3&quality=100&sign=ce390c90&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FoVaexusav9I9WwZs8xZm%252F10-%25E6%2589%25BE%25E5%2588%25B0%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Da8f2cb99-cd28-4d8e-8d9c-4517601a6078&width=768&dpr=3&quality=100&sign=d44b79ee&sv=2)

当我们通过合约地址找到自己发行的代币之后，点击Import，会有一个风险提示，大意就是说：

> 该代币不在频繁交易列表中。请注意，任何人都可以在 Sui 区块链上以任何名称创建代币，包括创建现有代币的假版本或声称代表没有代币的项目的代币。交易前务必进行自己的研究。

这个提示基本上每个土狗币都有，不用担心也不用在意，直接勾选继续下一步就行了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPrBFsdBuu6Bv491Wlz2X%252F11-%25E9%25A3%258E%25E9%2599%25A9%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3Dedbcd11b-9aee-4c4a-a111-a6882fc1877b&width=768&dpr=3&quality=100&sign=983941e9&sv=2)

确定交易对之后，我们选择交易费率，也就是我们通常理解的交易滑点

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4Je7w8XSNhr75lCPOPgy%252F12-%25E9%2580%2589%25E6%258B%25A9%25E6%25BB%2591%25E7%2582%25B9.png%3Falt%3Dmedia%26token%3D4804f041-dbbb-4ca3-84fd-4a3aaaa9bf50&width=768&dpr=3&quality=100&sign=94ac6294&sv=2)

一共有4个选择，分别是：0.01%、0.05%、0.25%、1%。这个滑点越大，意味着交易摩擦成本越高，但是也越容易成交。像稳定币，价格波动低的，可以选择0.01%、0.05%。正常的土狗币，推荐选择**0.25%和1%** 。因为土狗币交易不频繁、不稳定，滑点大一点有助于交易顺利完成

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fhjei6ToTDu1YIQmh6sKv%252F13-%25E8%25AE%25BE%25E7%25BD%25AE%25E6%25BB%2591%25E7%2582%25B9.png%3Falt%3Dmedia%26token%3D6b839da5-bd63-439b-a2ba-617067091e35&width=768&dpr=3&quality=100&sign=64d8d5e5&sv=2)

### 3、设置并创建资金池

当我选择一个滑点（0.25%）之后，我们就可以进行下一步配置了

首先需要给一个初始上线价格，这个价格是基于SUI的，即：1个土狗币=多少SUI

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCAfqo6XvO3ilnJv9ltZ8%252F14-%25E8%25AE%25BE%25E7%25BD%25AE%25E4%25BB%25B7%25E6%25A0%25BC.png%3Falt%3Dmedia%26token%3D650ff472-4a65-4256-8b76-c84dad27707c&width=768&dpr=3&quality=100&sign=75f3214d&sv=2)

假设我设置价格为：0.0000001SUI，它的意思就是：代币上线的价格是1Panda=0.0000001SUI。之后我们进入下一步，设置价格范围

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FyLmb5EiYNeGeEh8NCjcq%252F15-%25E4%25BB%25B7%25E6%25A0%25BC%25E8%258C%2583%25E5%259B%25B4.png%3Falt%3Dmedia%26token%3D87c36b8a-2ae5-4744-a9ee-8fef43678d8e&width=768&dpr=3&quality=100&sign=1900788b&sv=2)

如果你不太了解这个价格范围是啥意思，就把**Full Range勾选上** 。

> Full Range：全范围的意思。代币价格波动没有上限和下限，可以根据用户需求随时交易。

之后，我们填写要加池子的金额。例如，我选择加10个SUI，交易所会自动给我配对1亿个左右的Panda，确认数量后，点击n**ewAdd** 按钮即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FYpEa16b3BUUaszTaXPaW%252F16-%25E5%2588%259B%25E5%25BB%25BA%25E4%25BA%25A4%25E6%2598%2593%25E5%25AF%25B9.png%3Falt%3Dmedia%26token%3D11b5b0ef-e3ce-4cd4-83df-f92a91f19066&width=768&dpr=3&quality=100&sign=67f6434a&sv=2)

之后会弹出提示，让你确认创建资金池，我们点击按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCNWBdUtMrBjKcC4gkNSq%252F17-%25E7%25A1%25AE%25E8%25AE%25A4%25E5%25B9%25B6%25E7%2582%25B9%25E5%2587%25BB.png%3Falt%3Dmedia%26token%3D8780c3f2-7a89-4415-95d5-9b60aa867798&width=768&dpr=3&quality=100&sign=7d51f8a7&sv=2)

最后会弹出钱包让你进行确认，点击Approve就可以了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWng2ke4LliaWRBfkz80b%252F18-%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D1fe41363-da37-4400-beab-a471493af20e&width=768&dpr=3&quality=100&sign=774ac13&sv=2)

如果资金池创建成功了，会有下面这个提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F7xKjojLwoWkpbMIyDjyf%252F19-%25E8%25B5%2584%25E9%2587%2591%25E6%25B1%25A0%25E5%2588%259B%25E5%25BB%25BA%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Df587c195-692d-4a46-93aa-7309bb2f9e05&width=768&dpr=3&quality=100&sign=470c5d3b&sv=2)

到这里，资金池创建就完成了，我们试一下交易

### 4、交易代币

我们回到Cntus的官网首页：<https://app.cetus.zone/> ，在交易对那里输入Panda的合约地址，进行一笔500万的代币卖出

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F8W6fnABebaBZE8ocLTrL%252F20-%25E5%258D%2596%25E5%2587%25BA%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Dc0d2a158-5b72-44da-aeaf-cafd0cd8df65&width=768&dpr=3&quality=100&sign=eee5e899&sv=2)

点击Swap，钱包确认后，即可完成交易

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FRfagn9wfzHcCifB26zx8%252F21-%25E7%25A1%25AE%25E8%25AE%25A4%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3D9e9e51b1-efa7-4eb0-b2e9-b7ef08e83863&width=768&dpr=3&quality=100&sign=49f75bc4&sv=2)

确认交易

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FmxhycdBsXbJ5sD2l5YgG%252F22-%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4%25E6%2594%25AF%25E5%2587%25BA.png%3Falt%3Dmedia%26token%3D67507a35-1f38-4761-8d0f-2a7757befb52&width=768&dpr=3&quality=100&sign=40a0da9f&sv=2)

钱包确认交易

等待几秒钟，页面会有提示，就说明交易成功了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjYFtzPaSAsy2bvWr2CXm%252F23-%25E4%25BA%25A4%25E6%2598%2593%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D68607593-c86b-43ca-9f0b-46f602c25126&width=768&dpr=3&quality=100&sign=b9f9ccba&sv=2)

## 二、增加与撤出流动性资金池

池子创建成功后，接下来我们看怎么增加流动性与撤出流动性，即所谓的：加池子与撤池子。

首先我们要做的是找到自己的流动性，在Cetus的流动性管理页面，点击**我的仓位，** 找到自己的流动性：[**https://app.cetus.zone/pool/position** ](https://app.cetus.zone/pool/position)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F5PpK4wyFowI4zUHbbJPK%252F24-%25E6%2588%2591%25E7%259A%2584%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Def54438c-eed4-444d-a652-96c4405610cb&width=768&dpr=3&quality=100&sign=5be6b7f3&sv=2)

之后我们点击最右边的小按钮，这个按钮不太好找，请注意下图位置

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGQ9hP16yqy7Fhy4me455%252F25%25E5%25B0%258F%25E6%258C%2589%25E9%2592%25AE.png%3Falt%3Dmedia%26token%3D985842eb-ea08-4b18-89b0-832bea4fc8fe&width=768&dpr=3&quality=100&sign=bfee7ddb&sv=2)

然后就会进入到一个流动性操作的页面，具体内容如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FSnoL30fulGQElCzuHS1C%252F26-%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%2593%258D%25E4%25BD%259C.png%3Falt%3Dmedia%26token%3D70e0225e-8d33-4b25-9ec2-2afdda6b9220&width=768&dpr=3&quality=100&sign=49e6e485&sv=2)

如果我们要增加流动性，就在增加的页面输入金额，比如这样

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FUt62VUMXlotwSmYNMtlp%252F27-%25E5%25A2%259E%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Da42372dd-b0f5-4d63-b432-544577527a25&width=768&dpr=3&quality=100&sign=aa9eaa41&sv=2)

如果要移除流动性，就在移除的页面输入数量，并确认移除比例即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fzj3lMvyjB16OW3vl9lIP%252F28-%25E7%25A7%25BB%25E9%2599%25A4%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D70505150-6797-4301-9671-b777530a6ae1&width=768&dpr=3&quality=100&sign=2131d67c&sv=2)

其他的操作都是一样，点击按钮，钱包授权确认，即可完成操作

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCHm4eG5j280tYYLkgEmC%252F29-%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D4ff9c415-67b3-45bb-83a8-f1c08850f174&width=768&dpr=3&quality=100&sign=a208b526&sv=2)

到这里，整个关于Cetus的流动性教程就全部结束了，接下来解答一些疑问

## 三、疑问解答

**1、创建资金池的过程中不弹出钱包怎么办？**

  * 答：如果在页面操作时间过久，就会这样，可以刷新页面重试。或者查看一下钱包是否锁住，如果上锁了，把钱包解锁后刷新页面就可以了


**2、Cetus创建池子要收费吗？**

  * 答：根据实际操作经验来看，在Cetus创建池子不收取费用


**3、为什么池子创建成功后，在流动性管理那里找不到我的仓位？**

  * 答：池子创建成功后，等待几分钟，才能看到。如果很长时间找不到自己的池子，可以刷新页面，看看网络是否有问题


如有大家还有不明白或者不清楚的地方，请加入官方电报Telegram群：<https://t.me/PandaTool>
