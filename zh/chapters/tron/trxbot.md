# 波场Tron市值管理机器人使用教程

一篇文章学会使用波场市值管理机器人

Tron市值管理机器人，简单来说就是基于波场链开发的自动交易、批量交易的机器人系统，可以按照设定好的目标价格进行买卖

## 一、注意事项

1、 机器人为`单路由`模式：即，TRX的池子，只能用TRX交易。USDT的池子，只能用USDCT交易

2、 机器人目前只支持Sunswap V2 ，不支持Sunwap V1或者V3池子，也不支持Sunpump

3、 刚开盘项目价格不稳定，往往需要`提高滑点`才能交易成功

4、交易失败的大部分原因都是这几种：余额不够（查看参数是否填写错误）、没有按照流程操作（比如没查池子就开始交易）、矿工费较低（可以增加矿工费）、池子或者交易对的选择错误

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FgNfsbX09Z9DjvMcjwkor%252F15-%25E4%25BA%25A4%25E6%2598%2593%25E6%2589%2580.png%3Falt%3Dmedia%26token%3De8b2e5ce-f192-45b1-aa8a-ef0e48f017c8&width=768&dpr=3&quality=100&sign=922de8df&sv=2)

## 二、TRX市值管理使用教程

### 1.钱包连接并购买会员

打开市值管理机器人页面：<https://tron.ccbus.cc/trx>，右上角连接钱包（如果没有安装TronLink钱包，可以看 → [波宝钱包安装教程](/tron/tronlink)）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FojcKjtb8oWusPsYXVoRp%252F1-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Df8770cf8-53f0-4860-a644-8f7a4d1a47c4&width=768&dpr=3&quality=100&sign=80fd34eb&sv=2)

链接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4Cagz5iWy1vCZFhhZ1mH%252F2-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Da45b1413-8aa7-4fe5-9585-4d577b0b84ad&width=768&dpr=3&quality=100&sign=728d6b8c&sv=2)

点击连接

连接成功后，就可以在右上角看到自己的钱包地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FMYMDQ1EyFPnMT5AWx90U%252F3-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D5fdd1b1c-abad-4208-a593-6ea2e5e7c413&width=768&dpr=3&quality=100&sign=f6681a27&sv=2)

之后我们点击左侧的购买会员按钮，先进行会员购买，之后才能使用机器人

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FX8hJF1BnoOvO8IIjqygu%252F4-%25E8%25B4%25AD%25E4%25B9%25B0%25E4%25BC%259A%25E5%2591%2598.png%3Falt%3Dmedia%26token%3Db2bfa3e0-678b-4a62-ac2f-d7d7f943ce87&width=768&dpr=3&quality=100&sign=6ef90b58&sv=2)

选择你要购买的会员期限，如我选择月度会员，则需要4000TRX

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FtMb2fwPGEUPP913SpfxA%252F5-%25E8%25B4%25AD%25E4%25B9%25B0%25E4%25BC%259A%25E5%2591%2598.png%3Falt%3Dmedia%26token%3Dc8550b9b-81c9-4fd5-80aa-20523ac79d5f&width=768&dpr=3&quality=100&sign=77ef1446&sv=2)

确定好后，点击开通，会跳出钱包进行确认。如果钱包内余额充足，支付成功后会有以下提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fqbw65MgewuvLFPGrhSV6%252F7-%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Dfbf27770-010d-40a7-9c79-45264c844a1f&width=768&dpr=3&quality=100&sign=c653f584&sv=2)

如果钱包内余额不够，那么就会提示购买失败

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FtnvBQiQV0MRNom2oDKwT%252F8-%25E5%25A4%25B1%25E8%25B4%25A5.png%3Falt%3Dmedia%26token%3D8161c0a0-4330-4501-8722-5d8e033d9704&width=768&dpr=3&quality=100&sign=8772972a&sv=2)

如果你成功付款了，可以在会员页面看到你的到期时间

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhDjgzqXvh99Nyy1sMDjY%252F9-%25E4%25BC%259A%25E5%2591%2598%25E6%2597%25B6%25E9%2597%25B4.png%3Falt%3Dmedia%26token%3Dbe345bd3-06b7-4e90-92eb-12f97c292161&width=768&dpr=3&quality=100&sign=30135804&sv=2)

成功购买会员后，接下来就可以进行市值交易操作了

### 2.使用市值机器人

我们回到TRX市值机器人主页，操作流程如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F2LazBHwVcVR8tjA7LyOW%252F11-%25E5%25B8%2582%25E5%2580%25BC%25E6%259C%25BA%25E5%2599%25A8%25E4%25BA%25BA%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Ddb660f8b-9351-4254-a955-8b58eff360a4&width=768&dpr=3&quality=100&sign=9f802f14&sv=2)

**1.导入钱包：** 导入你的钱包私钥，可以选择同时导入多个地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FxpaqcI5VPzJtVg2aD0qx%252F12.png%3Falt%3Dmedia%26token%3D532643a1-15b9-4a69-aecc-a5b050b67b62&width=768&dpr=3&quality=100&sign=683c73e5&sv=2)

**2.刷新余额：** 导入之后刷新余额，看下目前你钱包内的代币情况

**3.基础代币：** 如果是U池子就选择U，TRX池子就选择TRX

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbElNrsYYFB9FBj9UMNwE%252F13-%25E5%259F%25BA%25E7%25A1%2580%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Ddb8c0fee-7fcb-4f8d-b71f-4f2b5f7c3110&width=768&dpr=3&quality=100&sign=57fe0dde&sv=2)

**4.目标代币：** 就是你要交易的代币，土狗币，输入合约地址查询

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLw9hPxe6O0ayRiUUtcCE%252F14-%25E5%2590%2588%25E7%25BA%25A6%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D0f505f1e-853a-4013-b37a-d6fafc20aa59&width=768&dpr=3&quality=100&sign=778f36b2&sv=2)

**5.交易间隔：** 每一笔交易之间的间隔时间，以秒为单位 

**6~7 选择金额：** 可以选择全部、随机和固定金额三个方式。

注意：如果是拉盘模式，那么金额就是TRX或者USDT的数量。如果是砸盘模式，则是土狗币的数量

**8.选择模式**

  * 拉盘模式→买入代币

  * 砸盘模式→卖出代币


**9.设置目标价格：** 拉盘模式下，目标价格要高于当前代币价格。砸盘模式下，目标价格要低于当前代币价格 

**10.查池子：** 查询池子地址和代币价格 

**11.开始：** 点击开始操作 

**12.停止：** 停止操作

## 三、疑问解答

**1、平台会拿到你的私钥吗？**

  * 答：绝对不可能，你的私钥不会存储在平台上，所有操作都是基于前端执行的，请放心使用。如果你比较担心，可以使用新的钱包操作


**2、市值管理是收费的吗？**

  * 答：需要购买会员才能使用


**3、最多可以导入多少钱包？**

  * 答：为了确保操作的稳定性和流畅性，一次性导入的钱包数量最好低于100个


**4、这个机器人能冲土狗吗？**

  * 答：市值管理机器人是为了项目方控盘用的，不是用来开盘冲土狗的。尽管可以用它来进行交易，但是并不会像市面上的PEPE BOT一样可以快速买入卖出，暂时没有这个功能


**5、为什么查不到我的池子？**

  * 答：请确认您的代币是否在Sunswap V2上线的，并确认交易对是否正确


如有不明白或者不清楚的地方，请加入官方电报群：<https://t.me/PandaTool>
