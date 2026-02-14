# 标准代币创建教程

干净合约、方便上手、无税无功能、Ave检测全绿

BSC链代币创建教程视频

## 1、功能解释

标准代币指的是**没有任何功能** 、机制的代币合约，代币创建之后默认会丢弃权限，所以也没有任何权限，是一个纯粹的、干净的、标准的合约。

根据以下步骤，您可以在可支持的任意一条链上，创建一个标准合约代币。以BSC为例。

  * 注意：没有安装小狐狸钱包的不能发币，请先安装小狐狸钱包插件，教程：<https://help.pandatool.org/practical-information/metamask>


## 2、连接钱包

使用浏览器或者钱包打开网址：<https://pandatool.org/#/coinrelease/standard>，点击右上角，将小狐狸钱包切换到币安主网（BSC）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVUub3Wn4ECqYrLMq8Qws%252F%25E5%25BE%25AE%25E4%25BF%25A1%25E6%2588%25AA%25E5%259B%25BE_20240117222904.png%3Falt%3Dmedia%26token%3D94b76302-e2e3-4e7b-a355-1667a3bb250e&width=768&dpr=3&quality=100&sign=2eed8679&sv=2)

## 3、填写代币参数

在打开的页面，依次填写代币信息。假设我们创建一个代币叫——“PandaTool”，应该进行如下填写：

  * **代币名称：** PandaTool（代币全称，支持中文、英文以及中英混合文字）

  * **代币符号：** Panda（代币简称，支持中文、英文以及中英混合文字）

  * **发行量：** 10000（代币数量）

  * **精度：** 18（小数点后的位数）

  * **收币地址：** 创建代币后接受代币的地址（代币给到谁）


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F00XgkypTY9k7fpZ10c9f%252F%25E5%258F%2591%25E5%25B8%2581%25E9%25A1%25B5%25E9%259D%25A2.png%3Falt%3Dmedia%26token%3D50128578-74ca-4dea-b1a9-a237e0c11d00&width=768&dpr=3&quality=100&sign=e62262af&sv=2)

## 4、创建合约

确认填写的参数无误后，点击“创建合约”。在打开的页面，将源代码和构造参数复制下来，以防万一：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FTFR3lWoHBLVj1Y92cZ9F%252F%25E5%25BC%2580%25E6%25BA%2590%25E5%258F%2582%25E6%2595%25B0.png%3Falt%3Dmedia%26token%3Dfd493f29-c78e-47ed-841a-714b7fd16980&width=768&dpr=3&quality=100&sign=110a0dd6&sv=2)

开源参数复制

复制之后，再次点击“创建合约”。此时小狐狸钱包会要求你支gas费，点击确认，等待几十秒，合约就创建完成了。

此时，我们点击`控制台`，就能看到自己创建的合约了，代币也已经发送到创建者的钱包地址里。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FSrKWiAByxiFAtc83zlUS%252F%25E8%25BF%259B%25E5%2585%25A5%25E6%258E%25A7%25E5%2588%25B6%25E5%258F%25B0.png%3Falt%3Dmedia%26token%3D3737044f-5d5a-44e7-8bde-5082eb157c2d&width=768&dpr=3&quality=100&sign=b13425bc&sv=2)

进入控制台

## 5、添加流动性

代币创建完成之后，只能转账，还不能交易。要想使代币可以交易，需要创建一个流动性资金池才可以。

### **1）进入PandaTool并连接钱包**

我们进入到PandaTool创建资金池工具的网页：<https://www.pandatool.org/#/createliquidity?lang=zh-CN> 然后在右上角点击连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPbbxvTJpKvA77TCQ9Tqg%252F1.%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D8dd6bd7f-1a0a-48c6-9946-129526d05c60&width=768&dpr=4&quality=100&sign=86bf2953&sv=2)

此时会跳出Metamask或者OKX Web3钱包，点击确认，即可完成连接。钱包连接成功后，会在右上角看到你的钱包地址。

如果你希望在BSC链创建资金池，就将区块链切换到BSC。如果是希望在以太坊上创建资金池，就将区块链切换到ETH即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1w5qQjQSljaqv4Dbi0Tk%252F2.%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Daa876443-0773-451e-90d8-e8643228e373&width=768&dpr=4&quality=100&sign=26ac03ef&sv=2)

### **2）选择代币**

连接钱包后，我们需要选择加池类型和代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZT8rDfyfi6Jtfuj2gjiu%252F3%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Dcb02c7a2-e16f-4009-b50e-0f9111029d9e&width=768&dpr=4&quality=100&sign=763a79b3&sv=2)

  * **加池类型：** 默认用V2，稳定池加V3

  * **底池代币：** 交易对价值代币，如USDT、BNB等

  * **代币地址：** 您创建的代币合约地址


填写好之后，点击`**查询代币**`，正常来说会提示你：**代币正常，请填写加池数量**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOGrX5fvZTzORDK0dCJoc%252F4%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D5b86d10f-a099-423c-9c5a-3b10cbd5db74&width=768&dpr=4&quality=100&sign=cc26fa49&sv=2)

### **3）填写加池数量**

确定好两种代币后，接下来就是填写代币数量了（加池数量不能超过自己钱包里的数量）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhSAXnwjXJmMKZk7CpF4M%252F5%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F2.png%3Falt%3Dmedia%26token%3D1c72c1bb-7067-430b-962d-e29629f038be&width=768&dpr=4&quality=100&sign=dd7453e&sv=2)

  * **Panda：** 我创建的代币，填写10000枚，表示将10000个Panda代币放入资金池中

  * **USDT：** 我选择的价值嗲比，填写10000，表示将10000个USDT放入资金池中


**预估价格：** Panda代币的初始价格是1USDT（用10000除以10000得到价格是1）。如果Panda放1000个，USDT放10000个，那么预估初始价格就是10U，以此类推

### **4）代币授权**

当我们确定好加池的代币和数量之后，就需要钱包授权了。也就是说，你要将代币授权给路由合约，然后路由合约会帮助你完成加池操作。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGeMSQ6p44y64PFQG5fqt%252F6%25E4%25BB%25A3%25E5%25B8%2581%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3Db5b2fa56-45ea-4bc1-9248-9e70c1e52ed6&width=768&dpr=4&quality=100&sign=69773d02&sv=2)

我们需要分别对两种代币进行授权（如果是BNB或者ETH，则无需授权），此时会跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fl3i0OVoKNWffqozv82tY%252F7%25E6%258E%2588%25E6%259D%2583%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3D5ec2687f-4bb1-44a1-9871-ae8c80242a8c&width=768&dpr=4&quality=100&sign=a2195cc2&sv=2)

当两种代币都授权成功后，会看到以下提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLKkMqMVD4wCBNKM9nM1w%252F8%25E5%25B7%25B2%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D8d3da2d0-d36c-4996-8dbd-22f886141257&width=768&dpr=4&quality=100&sign=e7da7db8&sv=2)

### **5）创建资金池**

代币授权完成后，就是创建资金池了。点击“立即加池”按钮，跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FE0nEZBS7LZZrNXaJY62g%252F10%25E5%258A%25A0%25E6%25B1%25A0%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3Dcffe5b72-d29f-4e7b-acd0-311e2794d90b&width=768&dpr=4&quality=100&sign=997908b5&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FguRrJDgzgmpDwW7YPUAc%252F9%25E7%25AB%258B%25E5%258D%25B3%25E5%258A%25A0%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D20531d92-8579-4058-bee5-c1d71ed4fd9b&width=768&dpr=4&quality=100&sign=cc14d5c9&sv=2)

钱包确认后等待几秒钟，即可完成创建资金池的操作

## 注意事项

  * 代币创建完成后，默认是开源的，无需手动开源。

  * 代币名称支持中文、英文以及中英混合文字

  * 如果您要在测试网添加USDT交易对，请使用PandaTool官方发布的测试USDT做资金池，合约地址：0x66e972502a34a625828c544a1914e8d8cc2a9de5


如果您有任何关于发币的问题，均可以在Telegram群里咨询我们的志愿者：<https://t.me/pandatool>
