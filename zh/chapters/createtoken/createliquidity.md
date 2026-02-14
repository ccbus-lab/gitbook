# 创建流动性资金池教程

在BSC、ETH、BASE上创建资金池

## **视频教程**

## **一、资金池概念解读**

流动性资金池，俗语称之为：底池、池子，英文简称LP，是区块链上用来进行兑换交易的代币池。通常来说，就是按照一定的比例将两种代币放到一起组成的池子。

那为什么要创建底池？很简单：**没有池子，不能交易；有了池子，才能实时兑换。**

如果你想学习更多资金池相关的知识，可以阅读以下文章：

  * ✅**流动性资金池概念解读：**<https://academy.ccbus.cc/kn/1056>

  * ✅**流动性池资金运作逻辑：**<https://academy.ccbus.cc/zh_CN/kn/805>


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FNzs9afxxH8qzIfYAK5AU%252FBSC%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%2599%25E7%25A8%258B.jpg%3Falt%3Dmedia%26token%3D8a052046-e7fa-415a-ac94-14e3f93c8149&width=768&dpr=3&quality=100&sign=d4c20fbb&sv=2)

## **二、创建资金池注意事项**

### **1、给路由合约加白名单**

如果代币有特殊的功能，如果手动开盘、持仓限制等，请先将PandaTool的路由合约加到白名单里面，才开始创建。

  * **PandaRouter路由合约地址：**`0x60c8E6DAAfD4D24fEa43E01CE1EC1ecDa3eE1143`

  * X Layer路由地址：`0x6ADCc1B97d84a2F566b443a6215ea0b01D40EBA4`


### **2、确保余额足够**

不管是创建什么类型的资金池，请确钱包内至少有**0.032个BNB** （BSC链的情况下）用于支付创建费用

### **3、V2和V3的区别**

PancakeSwap、Uniswap都有V2和V3两个协议，其实很好区分

  * **V2：** 适用所有类型的代币（标准ERC20、分红/销毁等复杂功能等），默认用V2就可以了

  * **V3：** 仅适用于标准代币（无功能代币），且PandaTool仅支持通过V3创建稳定池


## **三、创建资金池流程**

**步骤1：** 进入PandaTool、连接钱包并切换至对应的区块链

**步骤2：** 选择加池的两种代币

**步骤3：** 填写加池的代币数量

**步骤4：** 授权代币

**步骤5：** 立即创建资金池

### **1、连接钱包**

不管我们是创建代币、创建资金池，还是交易兑换、批量转账，第一步都是要连接钱包。连接钱包是所有DAPP必要的操作，希望大家都能养成这个习惯。不连接钱包，什么都做不了。

此时我们进入到PandaTool创建资金池工具的网页：<https://ccbus.cc/liquidity-control/create-liquidity> 然后在右上角点击连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPbbxvTJpKvA77TCQ9Tqg%252F1.%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D8dd6bd7f-1a0a-48c6-9946-129526d05c60&width=768&dpr=3&quality=100&sign=86bf2953&sv=2)

此时会跳出Metamask或者OKX Web3钱包，点击确认，即可完成连接。钱包连接成功后，会在右上角看到你的钱包地址。

如果你希望在BSC链创建资金池，就将区块链切换到BSC。如果是希望在以太坊上创建资金池，就将区块链切换到ETH即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1w5qQjQSljaqv4Dbi0Tk%252F2.%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Daa876443-0773-451e-90d8-e8643228e373&width=768&dpr=3&quality=100&sign=26ac03ef&sv=2)

### **2、选择代币**

连接钱包后，我们需要选择加池类型和代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZT8rDfyfi6Jtfuj2gjiu%252F3%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Dcb02c7a2-e16f-4009-b50e-0f9111029d9e&width=768&dpr=3&quality=100&sign=763a79b3&sv=2)

  * **加池类型：** 默认用V2，稳定池加V3

  * **底池代币：** 交易对价值代币，如USDT、BNB等

  * **代币地址：** 您创建的代币合约地址


填写好之后，点击`**查询代币**`，正常来说会提示你：**代币正常，请填写加池数量**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOGrX5fvZTzORDK0dCJoc%252F4%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D5b86d10f-a099-423c-9c5a-3b10cbd5db74&width=768&dpr=3&quality=100&sign=cc26fa49&sv=2)

### **3、填写加池数量**

确定好两种代币后，接下来就是填写代币数量了（加池数量不能超过自己钱包里的数量）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhSAXnwjXJmMKZk7CpF4M%252F5%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F2.png%3Falt%3Dmedia%26token%3D1c72c1bb-7067-430b-962d-e29629f038be&width=768&dpr=3&quality=100&sign=dd7453e&sv=2)

  * **Panda：** 我创建的代币，填写10000枚，表示将10000个Panda代币放入资金池中

  * **USDT：** 我选择的价值嗲比，填写10000，表示将10000个USDT放入资金池中


**预估价格：** Panda代币的初始价格是1USDT（用10000除以10000得到价格是1）。如果Panda放1000个，USDT放10000个，那么预估初始价格就是10U，以此类推

### **4、代币授权**

当我们确定好加池的代币和数量之后，就需要钱包授权了。也就是说，你要将代币授权给路由合约，然后路由合约会帮助你完成加池操作。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGeMSQ6p44y64PFQG5fqt%252F6%25E4%25BB%25A3%25E5%25B8%2581%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3Db5b2fa56-45ea-4bc1-9248-9e70c1e52ed6&width=768&dpr=3&quality=100&sign=69773d02&sv=2)

我们需要分别对两种代币进行授权（如果是BNB或者ETH，则无需授权），此时会跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fl3i0OVoKNWffqozv82tY%252F7%25E6%258E%2588%25E6%259D%2583%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3D5ec2687f-4bb1-44a1-9871-ae8c80242a8c&width=768&dpr=3&quality=100&sign=a2195cc2&sv=2)

当两种代币都授权成功后，会看到以下提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLKkMqMVD4wCBNKM9nM1w%252F8%25E5%25B7%25B2%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D8d3da2d0-d36c-4996-8dbd-22f886141257&width=768&dpr=3&quality=100&sign=e7da7db8&sv=2)

### **5、创建资金池**

代币授权完成后，就是创建资金池了。点击“立即加池”按钮，跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FguRrJDgzgmpDwW7YPUAc%252F9%25E7%25AB%258B%25E5%258D%25B3%25E5%258A%25A0%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D20531d92-8579-4058-bee5-c1d71ed4fd9b&width=768&dpr=3&quality=100&sign=cc14d5c9&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FE0nEZBS7LZZrNXaJY62g%252F10%25E5%258A%25A0%25E6%25B1%25A0%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3Dcffe5b72-d29f-4e7b-acd0-311e2794d90b&width=768&dpr=3&quality=100&sign=997908b5&sv=2)

钱包确认后等待几秒钟，即可完成创建资金池的操作

## **四、疑问解答**

**1、为什么加池会失败？**

  * **答：** 两个原因。首先确认一下自己钱包内的BNB/ETH数量是否足够，BSC链加池至少需要0.03个BNB。如果余额充足，那么再看下有没有**将路由地址加入白名单** 。

  * 路由地址：`0x60c8E6DAAfD4D24fEa43E01CE1EC1ecDa3eE1143`


**2、创建BNB交易对的池子，用户可以用USDT买币吗？**

  * **答：** 当然可以。创建USDT的资金池，用户也能用BNB购买代币，都是相通的。


**3、对于加池数量有要求吗？**

  * **答：** 没有要求。可以根据你的代币经济学和价格需求，添加适当比例的代币。一般来说，我们要求池子尽量大于300U或1个BNB。


**4、预估价格会变吗？**

  * **答：** 预估价格只是你的代币初始价格，即上线价格。后续随着不断交易，价格会不断变化。


**5、V2和V3有什么区别？**

  * **答：** 带功能/机制的币，只能加V2。目前V3的池子只支持标准币（主要做稳定池），大家不要加错了


如果您有任何关于创建资金池的问题，均可以在Telegram群里咨询我们的志愿者：<https://t.me/pandatool>
