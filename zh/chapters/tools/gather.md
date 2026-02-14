# 代币批量归集工具

一键批量归集EVM链的代币

批量归集工具指的是，可以将钱包内的代币一次性归集到一个地址，也就是我们常说的**多对一转账。** 归集完的钱包地址就可以直接丢弃掉，方便钱包的管理与整合。

接下来，将给大家演示，该如何使用PandaTool平台的批量归集工具


批量归集工具免费使用

### 一、连接钱包

首先，我们需要打开批量归集工具：<https://ccbus.cc/toolset/gather> ，进入之后，会让你切换到币安链

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F19IM1hfKWxCHvNg03t8V%252F1-%25E5%2588%2587%25E6%258D%25A2%25E9%2593%25BE.png%3Falt%3Dmedia%26token%3D956f26c4-531a-40c4-9d6e-b4bb07b2112c&width=768&dpr=3&quality=100&sign=91213a4d&sv=2)

将链切换到币安链，并连接钱包后，就能够看到整个批量归集的页面了。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FO8TPq21h3vAxEB80nbIw%252F%25E6%2589%25B9%25E9%2587%258F%25E5%25BD%2592%25E9%259B%2586.png%3Falt%3Dmedia%26token%3D17cbb1e2-de70-4b03-a5cb-270f82199a75&width=768&dpr=3&quality=100&sign=8898e9f4&sv=2)

需要注意的是，批量归集以前是需要购买会员才能使用，现在不需要了

### 二、配置归集参数

进入归集页面之后，我们需要按照下图顺序和要求，填写并配置相关信息，同时导入要`归集`的钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnZRvnbfGW4y5B8VjwJEp%252F4-%25E9%2585%258D%25E7%25BD%25AE%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3Ddfd4b163-b115-4547-b849-c9b173852530&width=768&dpr=3&quality=100&sign=eef6115e&sv=2)

**1、选择链**

  * 目前支持BSC、Arb、Base、ETH等多种EVM链的代币归集


**2、接收地址**

  * 输入接收代币的钱包地址


**3、归集代币**

  * 归集原生代币：如果归集BNB、ETH这种原生代币，不需要输入合约地址

  * 归集其他代币：如果归集的是其他代币，则需要填入代币合约地址


**4、导入钱包**

  * 导入需要归集的钱包私钥


**5、刷新余额**

  * 在导入钱包之后，需要刷新各钱包内的代币余额

  * 在每一次**完成归集后** ，也需要筛选钱包内的代币余额

  * 在每一次**切换了链之后** ，也需要刷新钱包内的代币余额


**6、选择归集方式**

  * **发送全部：** 将钱包内某个`指定代币`全部归集到指定的钱包地址

  * **归集数量：** 可以自定义要归集的代币数量，如果部分钱包数量不足，将跳过

  * **保留余额：** 在钱包内保留固定余额的代币，其余的归集出去。如果余额不够，将跳过


**7、核对归集信息**

  * 确认好要归集的信息无误


### 三、执行归集

如下图所示，当所有的信息填写完成后，我们点击归集按钮，即可开始执行归集

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEkirK6XxBlV05TithDzo%252F5-%25E6%2589%25A7%25E8%25A1%258C%25E5%25BD%2592%25E9%259B%2586.png%3Falt%3Dmedia%26token%3D4c07cd82-4731-4ca7-a821-9854fdaef333&width=768&dpr=3&quality=100&sign=f3dde2f3&sv=2)

不管执行结果是成功还是失败，都会给你展示出来。如果遇到失败的情况，可以点击地址栏的`执行`按钮，再次执行归集

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FJIbUgOjgHvk1wGdKjIxy%252F6-%25E7%2582%25B9%25E5%2587%25BB%25E6%2589%25A7%25E8%25A1%258C.png%3Falt%3Dmedia%26token%3D1561bd70-d71b-4f23-bd00-c0ffde989894&width=768&dpr=3&quality=100&sign=be204c15&sv=2)

### 四、批量归集疑问解答

**1、为什么归集会失败？**

  * 如果要归集的地址内的gas余额不足，也有可能会失败

  * 如果此时链刚好延迟了，也会导致部分钱包失败


**2、归集需要收费吗？**

  * PandaTool的批量归集产品是**不收费** 的，除了**gas** 以外，您不会额外支出其他费用


**3、为什么归集后没有返回结果？**

  * 可能是链卡住了，耐心等待几秒钟，就会有结果返回的


有任何关于批量归集的的问题，可以在电报群联系志愿者：<https://t.me/pandatool>
