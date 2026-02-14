# PumpFun一键捆绑卖出教程

多个地址内的代币一次性全部卖出

### 怎么理解PumpFun一键捆绑卖出这个功能？

我们假设这样一种情况，当你使用PUMP捆绑买入功能在多个地址内买入代币，或者拉盘刷量期间操作多个地址买入代币后，想将这些地址里面的代币全部卖出，应该怎么办？

传统的方式就是三种：

  * **第一种：** 手动卖。不断地切换钱包操作。这样不仅慢，而且机器人会泡在你的前面，不合适

  * **第二种：** 机器人卖。通过我们的机器人可以自动化卖出，省去了手动操作的麻烦，但是速度跟不上

  * **第三种：** 归集后卖。将代币归集到一个地址后统一卖出。听起来比较合适，但也是麻烦，多了一步归集的操作


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbDgCYoCEDBMjAFi6aSsC%252FPUMP%25E6%258D%2586%25E7%25BB%2591%25E5%258D%2596%25E5%2587%25BA.jpg%3Falt%3Dmedia%26token%3D125a0cc4-f200-482c-b97a-e8bdfe275e56&width=768&dpr=3&quality=100&sign=6cba8ce2&sv=2)

基于此，我们开发了一键捆绑卖出的功能，导入钱包私钥后，即可**一次性将所有钱包内的相关代币全部卖出。** 目前一次最多支持15个地址，如果钱包比较多，可以多导入几次。

### PUMP一键捆绑卖出教程

#### 1、配置卖出参数

我们打开PandaTool的一键卖出工具：<https://solana.pandatool.org/sellpump> ，或者在官网导航栏找到捆绑卖出的按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F0e5Do2qKWFjFvpPmIawl%252F1-%25E6%258D%2586%25E7%25BB%2591%25E5%258D%2596%25E5%2587%25BA.png%3Falt%3Dmedia%26token%3D0f31af3e-37d6-4531-a38e-24be72a9341b&width=768&dpr=3&quality=100&sign=a50cdd77&sv=2)

进入到捆绑卖出页面后，我们填写相关的参数

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fgigz1W2U0msc8BQRPp9M%252F5-%25E5%258D%2596%25E5%2587%25BA%25E5%258F%2582%25E6%2595%25B0.png%3Falt%3Dmedia%26token%3D99d33768-2bbc-4398-a08c-eb35e54b1d76&width=768&dpr=3&quality=100&sign=2655dee5&sv=2)

  * **pump代币：** 输入pump代币合约地址，点击查询

  * **代币名称：** 查询后自动识别，无需填写

  * **代币简称：** 查询后自动识别，无需填写

  * **Jito捆绑小费：** 默认是0.001sol。如果捆绑失败，可尝试提高Jito小费（4个地址以内不需要，4个地址以上需要）

  * **捆绑钱包设置：** 请注意,链接钱包不参与捆绑卖出,所有费用由第一个导入的地址支付!


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbpglD1pYk6zaiW7S9kFP%252F6-%25E5%25AF%25BC%25E5%2585%25A5%25E7%25A7%2581%25E9%2592%25A5.png%3Falt%3Dmedia%26token%3Dc40d0765-79d2-4a59-9a2f-a7e907b2496d&width=768&dpr=3&quality=100&sign=b8d6222b&sv=2)

导入钱包后，我们点击刷新余额，大概就是这样一个页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1BJrZ7L7JpNDXIRmCZO9%252F7-%25E5%258D%2596%25E5%2587%25BA%25E9%2585%258D%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Df813cbf6-1a72-4aa6-bfd8-912755188e50&width=768&dpr=3&quality=100&sign=9cd924a0&sv=2)

从这张截图中我们发现一个问题：第一个钱包尾号为wnnt的地址，钱包内的Sol余额比较少（必须大于0.3个sol），无法支付卖出费用。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FxFzE8FSs5a9TjWVASLZh%252F8-%25E5%25AF%25B9%25E8%25B0%2583%25E4%25BD%258D%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3D63227f06-4d7f-4039-b9bc-ff34c27e1373&width=768&dpr=3&quality=100&sign=eedefc52&sv=2)

因此，我们需要转一些sol给第一个钱包地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQyOHaL8AOXPoq9H8ZnUr%252F8-2%25E4%25BD%2599%25E9%25A2%259D%25E5%25A4%259F%25E4%25BA%2586.png%3Falt%3Dmedia%26token%3D8f3e6d47-8f77-40b2-95e9-fa203e5bbbe0&width=768&dpr=3&quality=100&sign=78da0558&sv=2)

搞定后，在确认其他地方也没有问题后，我们点击立即卖出

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FoRjd9JwnszKBKiRphKgp%252F9-%25E7%25AB%258B%25E5%258D%25B3%25E5%258D%2596%25E5%2587%25BA.png%3Falt%3Dmedia%26token%3D60c5621e-db1f-4ad3-9376-06f0f54adb25&width=768&dpr=3&quality=100&sign=7c9c83ff&sv=2)


☝当仅导入四个地址时, 无需 使用Jito捆绑功能,成功率较高,推荐使用!

☝最多支持15个地址捆绑卖出,当超过四个地址时,需要使用 Jito的捆绑功能。

☝由于网络环境、Jito节点等复杂影响,该功能可能出现失败。尽快确认。

☝为提高成功率,在弹出钱包后,请尽快确认。

☝若捆绑失败,无任何费用,请尝试更换RPC节点,并考虑在链上活跃度较低的时段再次尝试。

#### 2、确定钱包卖出

当我们点击**立即卖出，** 平台的前端会自动执行，将地址内的代币全部卖出。注意，是全部卖出，不可以指定数量哦

等待15~30秒，如果还没有成功，大概率就是失败了，需要重新提交。

如果卖出成功，会出现以下提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fl0qIiVkC1EtII20e8kM3%252F11-%25E5%258D%2596%25E5%2587%25BA%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Df4adff65-333e-4758-b381-46ddbd320aee&width=768&dpr=3&quality=100&sign=1a331249&sv=2)

之后我们点击刷新余额，就能看到余额为0了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVrYIE3AdZCQdwwJH7ZCT%252F12-%25E5%2588%25B7%25E6%2596%25B0%25E4%25BD%2599%25E9%25A2%259D.png%3Falt%3Dmedia%26token%3D1788f66b-ad6d-48c3-9340-ed0f2cb3ebdf&width=768&dpr=3&quality=100&sign=c07bcb14&sv=2)

### 疑问解答

  1. **一键捆绑卖出需要收费吗？**

     * **答：** 每个地址收费0.01sol，这部分费用全部由第一个钱包出

  2. **一键捆绑卖出是卖出钱包内的所有代币吗？**

     * **答：** 捆绑卖出是卖出你选择的那个PUMP的币，没有选择的币是不受影响的

  3. **卖出失败是怎么回事？**

     * **答：** 正常4个地址以内，应该不会失败。超过4个地址之后，需要用Jito捆绑。捆绑的话可能会失败，这个时候需要刷新后重试，并增加Jito费用


如何您还有其他问题，都可以进入Telegram电报群找志愿者解答： <https://t.me/pandatool>
