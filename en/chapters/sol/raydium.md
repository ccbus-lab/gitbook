# Raydium CPMM加池子教程

Sol链上最大DEX

CPMM是Raydium最新推出的一个流动性产品，具有以下特点：

  * **新的做市逻辑：** 采用了新的 CPMM 做市模式，有别于之前V2的AMM

  * **不需要市场ID：** CPMM不再需要Openbook市场ID，可省去一笔ID创建费用

  * **创池成本更低：** CPMM的池子创建收费0.2sol，是原先AMM池子的一半

  * **支持度不够：** 例如PEPE机器人等尚不支持CPMM版本，只有我们的市值机器人支持

  * **交易问题 ：** 加了CPMM池子之后，偶尔可能会遇到无法交易的问题


### 1、加池子

我们打开Raydium的官网：<https://raydium.io/liquidity-pools/>，点击右边的`创建`按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6WDax2cGwL3nfF3tT2YM%252F%25E5%2588%259B%25E5%25BB%25BA%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D6b0b3519-3781-464c-845b-476924b2a0e8&width=768&dpr=3&quality=100&sign=77ae3982&sv=2)

打开之后，选择**标准AMM池** ，然后继续下一步

  * 集中池创建麻烦，且价格不能波动太大，所以一般我们推荐创建标准AMM池


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F5k4P6N0Sl51S4e092l8l%252F%25E6%25A0%2587%25E5%2587%2586AMM%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3De69cc612-9a56-439a-ad75-8f0616d40008&width=768&dpr=3&quality=100&sign=37561b70&sv=2)

### 2、确定价格和比例

在新的页面，我们需要填写相应的代币与数量，进行流动性创建

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6KnkbCStHVgrr3mZew4B%252F%25E4%25BB%25A3%25E5%25B8%2581%25E6%2595%25B0%25E9%2587%258F%25E4%25B8%258Esol%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3Dda6f30d7-f139-4fee-8cce-d9800dfbe7f0&width=768&dpr=3&quality=100&sign=b3a719a&sv=2)

  * **代币数量：** 你要添加到池子里面的代币数量（你发行的代币）

  * **Sol数量：** 你的交易对代币（报价代币）

  * **开盘时间：** 代币开始交易的时间。这个时间之前，池子无法交易（UTC时间，与北京时间有8个小时时差）

  * **开盘价格：** 也就是代币初始价格，取决于你的代币数量与Sol数量。例如，我初始放入1亿枚代币和1个sol进入池子，那么我的开盘价格就是：0.00000001sol，换算成USDT就是0.00000182U


例如我填好的，类似于下面这样：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9pAHjRwBs3WTNzWpkWTV%252F%25E5%25BC%2580%25E7%259B%2598%25E6%2597%25B6%25E9%2597%25B4.png%3Falt%3Dmedia%26token%3D4277bae9-bc6b-4cab-86e8-14e5d67055fa&width=768&dpr=3&quality=100&sign=473368f1&sv=2)

关于开盘时间这一块，在设置的时候，Raydium很人性化的给予了自动转换时区的功能，UTC时间与北京时间自动转换，所以设置起来就比较方便了，例如下面这样

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3xlE48Jt5OR19IP11nyY%252F%25E6%2597%25B6%25E9%2597%25B4%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Da5b2a29f-5996-42cb-b848-962a30f3ef03&width=768&dpr=3&quality=100&sign=ecb32644&sv=2)

确定好没问题之后，点击初始化流动性，钱包确认支付费用就可以了。（注：加池手续费大概0.2sol左右）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FBrFiZays0USC6APTy5NE%252Fsol%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D5f5b599b-8250-4b7c-a5da-1c4acf454417&width=768&dpr=3&quality=100&sign=a5068b2b&sv=2)

池子创建成功后，会有个提示给你，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FftiqeDrAALn7p53AUnb4%252F%25E6%25B1%25A0%25E5%25AD%2590%25E5%2588%259B%25E5%25BB%25BA%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D342670d1-a14a-46f4-9ce2-41c4adb5620c&width=768&dpr=3&quality=100&sign=1528c51f&sv=2)

### 4、撤池子

池子加好之后怎么撤呢？这里也和大家说一下

我们打开Raydium，找到`我的投资组合`，页面链接：<https://raydium.io/portfolio/> 选择标准流动池，就能看到自己的池子了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FpcHa3LHnubNQKBpzRgzg%252F%25E6%2592%25A4%25E6%25B1%25A0%25E5%25AD%2590%25E6%258C%2589%25E9%2592%25AE.png%3Falt%3Dmedia%26token%3D79e5476c-11ef-4f40-95b0-71a837740cb6&width=768&dpr=3&quality=100&sign=b2c4a29d&sv=2)

  * 注：如果你设置了开盘时间，那要等到开盘后，才能看到池子


此时，如果你想撤池子，选择那个“-”按钮就可以了，如下所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FeDxvdect4BFgWgf0iIXs%252F%25E6%2592%25A4%25E6%25B1%25A0%25E5%25AD%2590%25E6%25AF%2594%25E4%25BE%258B.png%3Falt%3Dmedia%26token%3Dc2319054-5152-424a-859e-75d252f1d6df&width=768&dpr=3&quality=100&sign=63b42c63&sv=2)

选择你要撤池子的比例，点击`移除流动性`，然后钱包确认，就可以了

### 5、相关问题

**1）** CPMM**有什么优点/缺点？**

  * 答：CPMM的优点就是不用创建市场ID，省了笔钱。缺点就是一些狙击机器人不支持V3，没法用


**2）加了** CPMM**池子后能**`**锁池**`**吗？**

  * 答：同样可以烧池子


**3）代币没有关闭冻结权限，怎么办？**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FwBe30g7Vb7UHSnTXqtqj%252F%25E5%25BE%25AE%25E4%25BF%25A1%25E6%2588%25AA%25E5%259B%25BE_20240528170459.png%3Falt%3Dmedia%26token%3Dd2570cbb-cc7f-4d56-b625-bc16c48a5014&width=768&dpr=3&quality=100&sign=7d17091f&sv=2)

  * 答：需要去权限管理工具那里关闭冻结权限：<https://solana.pandatool.org/control>，方可继续操作。如果还是有提示，可能是raydium有缓存，需要更换网络或者刷新重试


**4）“应用程序错误：发生了客户端异常”应该怎么解决**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4qFu0DrwwkUGePeN74qq%252F%25E5%25BE%25AE%25E4%25BF%25A1%25E6%2588%25AA%25E5%259B%25BE_20241001101529.png%3Falt%3Dmedia%26token%3Dd547b151-9262-4afd-9573-153c9ab7f47e&width=768&dpr=3&quality=100&sign=1523fb6e&sv=2)

  * 答：出现这个问题的原因主要是在谷歌浏览器开启翻译导致的，只要将翻译关闭，重新刷新试一下，这个问题就不会出现了


以上就是关于Raydium CPMM加池子/撤池子的全部教程了，如果有任何问题，请进入我们的电报群：<https://t.me/pandatool>，找志愿者解答，谢谢
