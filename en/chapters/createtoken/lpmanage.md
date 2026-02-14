# 增加/移除流动性资金池教程

在BSC链上加池子、撤池子的教程

如果您已经在Pancake薄饼或者Uniswap创建了一个流动性资金池，该如何看到自己的池子呢？通过我们的[流动性控制台](https://www.pandatool.org/#/LPmanage?lang=zh-CN)查看，如下图所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZimxZmqUS9Zb0YrLFAYn%252F1.%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%259F%25A5%25E7%259C%258B.png%3Falt%3Dmedia%26token%3D5f5e70b0-f9c8-48bf-bde7-f14382c944cb&width=768&dpr=3&quality=100&sign=adffa847&sv=2)

接下来可以有两个操作：添加流动性和移除流动性。

  * **添加流动性：** 继续向底池内添加代币，让池子越来越大

  * **移除流动性：** 将池子资金取出，使交易无法继续进行


不管是添加流动性，亦或者移除流动性，都是在对已经有的流动性资金池进行管理。这个管理，主要是基于PandaTool开发的流动性控制台实现。

如果您想了解该如何添加或者移除流动性池，可以阅读下面的教程：

### **1、打开PandaTool并连接钱包**

首先，我们进入PandaTool的流动性控制台 <https://www.pandatool.org/#/LPmanage?lang=zh-CN> ，然后右上角连接钱包，并选择对应的区块链

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fy0DUp8sxi7JYbHr3tH9I%252F2%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Dd2794b8f-42a3-4c2d-a28c-253b41137062&width=768&dpr=3&quality=100&sign=c2ff32d9&sv=2)

成功链接钱包后，刷新一下，就会自动查询到当前钱包的流动性情况，如下图

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZimxZmqUS9Zb0YrLFAYn%252F1.%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%259F%25A5%25E7%259C%258B.png%3Falt%3Dmedia%26token%3D5f5e70b0-f9c8-48bf-bde7-f14382c944cb&width=768&dpr=3&quality=100&sign=adffa847&sv=2)

### **2、添加流动性**

添加流动性，我们也可以称之为：增加流动性。指的是，当您创建流动性资金池之后，觉得池子太小，可供交易的金额不大，此时通过增加流动性功能，将更多的代币注入池子中，从而加大资金池

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQrC8UCYbX0A91pSSDi1t%252F3%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%258C%2589%25E9%2592%25AE.png%3Falt%3Dmedia%26token%3D18c57c2e-56fb-4659-9be4-31d83d2fb4f4&width=768&dpr=3&quality=100&sign=a2d686aa&sv=2)

我们点击`添加流动性`按钮后，可以进入到具体的添加页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZLKWzIVetudcHZTQ9D2E%252F4%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E8%25AF%25A6%25E6%2583%2585.png%3Falt%3Dmedia%26token%3Ddb727a3e-41f9-4b65-a7b0-cba033512bcc&width=768&dpr=3&quality=100&sign=57d215ba&sv=2)

  * **加池数量：** 填入您要注入资金池的代币数量（基础代币与报价代币）

  * **授权：** 分别授权基础代币和报价代币，点击授权并钱包确认

  * **立即加池：** 确认好入池数量和授权后，点击`立即加池`按钮


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEFaIiy9IUYTyCPwXMYBG%252F5%25E7%25AB%258B%25E5%258D%25B3%25E5%258A%25A0%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D19039ab6-5f89-4854-aa05-5e19abedcbb0&width=768&dpr=3&quality=100&sign=57b33189&sv=2)

如果加池成功，网站会有相关提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FKppE0FCWayr9XflyJTQr%252F6%25E5%258A%25A0%25E6%25B1%25A0%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D598624ea-2400-4384-8ee1-0f9127b2ceb6&width=768&dpr=3&quality=100&sign=1966e94b&sv=2)

### **3、移除流动性**

移除流动性，我们也称之为：撤池子，就是将流动性资金池内的代币撤出。撤出可以分比例撤出，也可以全部撤出。如果将流动性全部撤出，意味着该代币将无法交易。撤出的代币归操作钱包所有，即谁撤的归谁。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Ff0QkEuoyOCqWpg1DLMJC%252F7%25E6%2592%25A4%25E5%2587%25BA%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D0c831ebf-5b80-448a-ad6d-e62eda9c733f&width=768&dpr=3&quality=100&sign=aa763552&sv=2)

点击撤出流动性的按钮后，我们可以看到具体的详情

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FUdvW2wQNhtuilWbv7NLt%252F8%25E7%25A7%25BB%25E9%2599%25A4%25E8%25AF%25A6%25E6%2583%2585.png%3Falt%3Dmedia%26token%3D7457b196-7054-408f-84f8-5cf920842fb4&width=768&dpr=3&quality=100&sign=bd7d6543&sv=2)

  * **移除百分比：** 选择您要撤出的流动性比例，从0~100%

  * **移除LP数量：** 这些LP数量将会被销毁掉，数量是自动计算的

  * **预计获取数量：** 您预计可以获得的代币数量（包括基础代币与报价代币）

  * **接收钱包：** 接收代币的钱包，默认这个钱包是操作钱包，当然也可以选择其他钱包

  * **Lp代币授权：** 移除流动性前需要将Lp授权给路由合约，以便其进行撤池操作


确定好移除比例和接收钱包后，我们点`击确认撤池`按钮，此时会跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4BMj8XHco4Al1wU46lNA%252F9%25E7%25A1%25AE%25E8%25AE%25A4%25E6%2592%25A4%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D20860cbe-5806-4d8c-b458-47353350ffda&width=768&dpr=3&quality=100&sign=c484e78f&sv=2)

等待几秒钟，会提示您撤池成功

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGOqR9GQDzDoKPoL8UtkE%252F10%25E6%2592%25A4%25E6%25B1%25A0%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Dce1f89a1-bd03-4b69-b561-8ea2eca82c8b&width=768&dpr=3&quality=100&sign=da54526b&sv=2)

### **4、锁住流动性（锁池）**

锁池，顾名思义就是将流动性锁住，使得加池的人不能撤出流动性，从而保证了项目方撤池跑路的风险。如果您希望进行锁池操作，可以点击`锁池`按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6r1ScvHBatFoOfXrMQ5Z%252F1%25E9%2594%2581%25E6%25B1%25A0%25E6%258C%2589%25E9%2592%25AE.png%3Falt%3Dmedia%26token%3D9985bc84-0d24-48a3-ab8b-d4150e696468&width=768&dpr=3&quality=100&sign=76b35bfe&sv=2)

点击锁池之后，会跳出一个页面，让您填写相关的锁池参数

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1D66h3GEswzG0OIj8Gnt%252F2%25E9%2594%2581%25E6%25B1%25A0%25E8%25AF%25A6%25E6%2583%2585.png%3Falt%3Dmedia%26token%3D5fd0c0a2-a7bf-41f7-9046-c11cafb6798d&width=768&dpr=3&quality=100&sign=971378fc&sv=2)

  * **锁池百分比** ：这个百分比指的是您占有的池子比例的百分比，而非所有流动性的百分比

  * **锁池数量：** 由百分比自动计算出LP的数量

  * **解锁日期：** 根据您当地的时区来设定解锁日期，到期前不可取出LP

  * **锁池标题：** 随便起个名字就行，不是必须要填的

  * **LP代币授权：** 在撤池前需要进行授权


**关于百分比：** 假设池子都是您一个人加的， 那么这个百分比=池子的百分比。如果池子是多个人加的，就需要另外算的。比如，您本身占有池子份额的20%。那么您即便选择100%，整个池子也只是锁了20%的流动性而已。如果您选择20%，那么整个池子也就是锁了4%的流动性。

LP授权之后，点击确认锁池，等待几秒钟，就可以完成了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWryatRNMp8JdO9afKzhB%252F3%25E7%25A1%25AE%25E8%25AE%25A4%25E9%2594%2581%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D41a5079a-72da-4c97-9928-e1486cd516e9&width=768&dpr=3&quality=100&sign=4362947c&sv=2)

锁池之后，我们去哪里看呢？可以在[锁仓控制台](https://www.pandatool.org/#/lockList?lang=zh-CN)里查询我们的锁信息。进入锁仓控制台 → <https://www.pandatool.org/#/lockList?lang=zh-CN>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQtM54U3DdMdOVyZ9vmMf%252F4%25E9%2594%2581%25E4%25BB%2593%25E6%258E%25A7%25E5%2588%25B6%25E5%258F%25B0.png%3Falt%3Dmedia%26token%3D267347e5-4df6-4696-b6bd-00de9a982578&width=768&dpr=3&quality=100&sign=7eec453b&sv=2)

至此，整个关于添加流动性、移除流动性和锁定流动性的教程就算是结束了。和创建流动性相比，增加或者撤出池子的流程还是比较简单的。

接下来，我们看一些疑问

### **5、疑问解答**

**为什么加池/撤池会失败？**

  * 答：主要是两个原因。第一，确认一下钱包是否有足够的原生代币。如果是在BSC链，钱包内至少有**0.011BNB** 才可以成功。如果余额没有问题，我们再看第二个原因，确认一下是否将路由地址加入白名单。特别是功能性代币（如带有交易限制、持仓限制等），需要将路由地址加入白名单才可以完成添加或移除流动性的操作

  * BSC链路由地址：`0x60c8E6DAAfD4D24fEa43E01CE1EC1ecDa3eE1143`


**锁池后代币还能交易吗？**

  * 答：没有问题，锁池只是为了让项目方不能撤池子，不会影响代币的交易。


**锁池可以提前取出LP吗？**

  * 答：不可以，必须严格遵循锁池的时间。到期之前，任何人无法取回LP


**锁池后可以在Ave查询出来吗？**

  * 答：可以，锁池后，Ave会显示出Pinksales的锁标志


**移除/添加/锁池会收取费用吗？**

  * 答：是的，添加流动性、移除流动性和锁池，都是按次收费，每次0.01BNB


如何您还有其他问题，都可以进入Telegram电报群找志愿者解答： <https://t.me/pandatool>
