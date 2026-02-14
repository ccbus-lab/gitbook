# Turbos创建CLMM流动性资金池教程

在Turbos上创建CLMM资金池

[Turbos Finance](https://turbos.finance/) 是第一个建立在 Sui 上的去中心化零滑点永续合约交易和现货交易平台，由 Sui（Turbos）驱动的去中心化永续交易平台，交易效率更快、手续费更低、清算风险更低。

Turbos提供具有集中流动性做市商(CLMM) 模型和衍生品交易功能的自动做市商(AMM) 去中心化交易所，主打一个用户友好。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqwaE0RS1lMZPbteU6z5H%252F1-%25E9%25A6%2596%25E9%25A1%25B5.png%3Falt%3Dmedia%26token%3Dba649c25-0447-4f54-aee7-b58582ba8228&width=768&dpr=3&quality=100&sign=37195954&sv=2)


注意：本文仅作为教学演示，所涉及到的资金池和代币均**没有任何实际价值** ，大家也不要进行任何形式的交易。如果因此造成资金损失，PandaTool无法对此负责

## 一、创建CLMM资金池

和[Cetus](/sui/cetus)类似，在Turbos上也只能创建CLMM资金池，无法创建AMM资金池。

### 1、连接钱包

连接钱包是所有操作的第一步，老手可以直接忽略。我们打开Turbos的官网：<https://app.turbos.finance/>，点击右上角Connect Wallet按钮，进行钱包连接

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqMIROj9M4OBK8brPlQ3r%252F2-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Ddddccf57-fb43-4db5-b33e-857b2e95c65e&width=768&dpr=3&quality=100&sign=f2fb4dd9&sv=2)

在弹出的钱包选项中，PandaTool推荐大家选择[Suiet钱包](/sui/suiet)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVI6LTpPuMVWHwqHl6OXk%252F3-suiet%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D5450ea76-2790-4fd1-a15a-d6e06c09fc72&width=768&dpr=3&quality=100&sign=e193fa1b&sv=2)

和所有的DAPP一样，连接成功后，右上角会出现钱包地址。此时我们点击[Earn](https://app.turbos.finance/#/pools)这个按钮，即可找到创建池子的页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FuVd0Isiu5Mo0CmJXLaqi%252F4-%25E9%2592%25B1%25E5%258C%2585%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Da330ec95-d5a1-42ee-97b2-d554901e729a&width=768&dpr=3&quality=100&sign=995b0bbf&sv=2)

### 2、创建交易对

当然，我们也可以直接通过链接进入加池页面：<https://app.turbos.finance/#/pools> ，进来之后，我们找到**Creat a Pool** 这个位置，点击进入即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fv9yQ5KXnjS0shmPIgxvH%252F5-%25E5%2588%259B%25E5%25BB%25BA%25E6%25B1%25A0%25E5%25AD%2590.png%3Falt%3Dmedia%26token%3D17248f06-d873-4c00-8ccc-f52076c6cefe&width=768&dpr=3&quality=100&sign=d8ab6c19&sv=2)

第一步，我们需要先选择代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fs2O8zXdGyQ8R2gDC27z6%252F6-%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D4e1768bf-93c2-4e97-8805-ea5b86b99e17&width=768&dpr=3&quality=100&sign=43aafd51&sv=2)

  * **base token：** 基础代币，就是你发行的土狗币

  * **quote token：** 报价代币，就是SUI、USDT、USDC这种主流币


例如我通过合约地址选择Panda作为基础代币，SUI作为报价代币，就是下面这样

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FaOsME034H6N8mdzdUlv0%252F7-%25E6%2589%25BE%25E5%2588%25B0%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D3b1327cb-c0a0-4ba3-bd60-77ac0735c964&width=768&dpr=3&quality=100&sign=b785eb29&sv=2)

输入合约地址找到代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnObFkURMAVOl7DanYIvB%252F8-%25E6%2589%25BE%25E5%2588%25B0%25E4%25BA%25A4%25E6%2598%2593%25E5%25AF%25B9.png%3Falt%3Dmedia%26token%3Dbf766f35-a20f-43e9-82c4-b5c3fb3d05bb&width=768&dpr=3&quality=100&sign=b89be537&sv=2)

找到交易对

确认好两个代币交易对之后，我们继续进入下一步

### 3、设置资金池

在资金池设置页面，我们需要设置费率、初始价格、价格范围等内容，具体可参考下图所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fa8HlQIbvLm2xDegK9ypJ%252F9-%25E8%25B5%2584%25E9%2587%2591%25E6%25B1%25A0%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Dbd2c925b-d329-449e-b709-fa997a78d92f&width=768&dpr=3&quality=100&sign=cfe7b2f8&sv=2)

创建资金池可能涉及到的选择

  * **费率/滑点：** 虽然给出了多个等级，但是默认只能**选择1%** ，没有其他选项

  * **设置初始价格：** 即代币的上线价格，如果是SUI池子，则该价格以SUI计价，例如我要设置Panda的上线价格是0.0000001 SUI，那么在这个输入框里填入0.0000001即可

  * **设置流动性范围：** 其实就是该流动性的价格波动范围，这个大家请直接选择**Full** ，即**全范围** ，表示代币价格没有下限或上限。如果选择Custom，则需要设定一个价格下限与上限，这样不利于项目的长期运作

  * **加池数量：** 填写你要放入资金池的代币数量

  * **提示：** 最后会有一个提示，大概意思就是说，池子不能小于100U


了解完所有选项配置之后，PandaTool填写的参数示意如下

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FapFTqzRKG2h8HZat2fZo%252F10-%25E8%25B5%2584%25E9%2587%2591%25E6%25B1%25A0%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Dde915a80-578f-4e05-bb89-830dd10aa83c&width=768&dpr=3&quality=100&sign=b4135e99&sv=2)

填写完成之后，点击Create Turbos pool and deposit（创建池子并存入代币），进行二次确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9n23MHTXbn8G0nolDvhj%252F11-%25E5%2586%258D%25E6%25AC%25A1%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D034258b2-44f8-4462-af91-31183c733432&width=768&dpr=3&quality=100&sign=fe37c981&sv=2)

再次确认信息无误之后，点击按钮，会弹出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FtSw5h2elDumIt8g4SJud%252F11-%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3Ddcff6601-8876-469e-ba91-277aeb7e516e&width=768&dpr=3&quality=100&sign=85e84ffe&sv=2)

钱包点击Approve后，等待几秒钟，Trubos会提示你创建成功

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbkF30uxQblxFlKEnpqlT%252F12-%25E5%2588%259B%25E5%25BB%25BA%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Def6a710b-138c-4c75-a60b-33ec39e4a522&width=768&dpr=3&quality=100&sign=dbc31323&sv=2)

### 3、交易代币

池子创建成功后，就可以交易了。我们进入到Trurbos的官网首页：<https://app.turbos.finance/> ，选择卖出Panda代币3000万个


注意：做完池子后，等待至少30分钟后，才能交易。流动性池子初始化需要时间，无法立即开始交易

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbTwKw8OgvRgeXHDy4D6y%252F13-%25E4%25BB%25A3%25E5%25B8%2581%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3D111c1285-00a0-4c37-abc2-3c27d9c03f42&width=768&dpr=3&quality=100&sign=32ed1155&sv=2)

点击Trade后，钱包确认即可完成交易

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FTp8uqLytjTxSsO8dRcqu%252F14-%25E4%25BA%25A4%25E6%2598%2593%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D8944f063-63ba-4981-a516-eaefcc5cf753&width=768&dpr=3&quality=100&sign=e93b0747&sv=2)

## 二、增加与撤出流动性池子

池子创建好之后，在哪里加池子和撤池子呢？首先，我们进入到Turbos的流动性管理页面：<https://app.turbos.finance/#/pools> ，选择[Manage Positions and Rewards](https://app.turbos.finance/#/pools?tab=position)（管理流动性与奖励）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FoHQ6RzdoQxQTie47f9Hx%252F15-%25E7%25AE%25A1%25E7%2590%2586%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D8032c0b8-624d-4461-8b2d-616476790223&width=768&dpr=3&quality=100&sign=58573e5e&sv=2)

管理流动性

之后就能看到你钱包里面的所有流动性了，包括流动性的金额、范围、APR等都很清晰的展示，我们选择要增加或者撤出的流动性交易对

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FncuWarOtQgolJnG4ohTV%252F16-%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7png.png%3Falt%3Dmedia%26token%3D1bfb0079-62e4-4fe7-a4b4-18bcbc6dbd9c&width=768&dpr=3&quality=100&sign=52a98e06&sv=2)

在进入的页面里，就可以对这个流动性进行管理了，包括增加或者撤出流动性

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVIMFsJ0DjpxzdGGmpYhh%252F17-%25E5%25A2%259E%25E5%258A%25A0%25E4%25B8%258E%25E6%2592%25A4%25E5%2587%25BA%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D24910571-8a21-4fe0-b110-ceec49c0165b&width=768&dpr=3&quality=100&sign=f3cb15e8&sv=2)

  * Increase Liquidity：增加流动性（加池子）

  * Remove Liquidity：撤出流动性（撤池子）


假设我们点击**增加流动性** ，就可以按照比例进行增加相应的代币，然后钱包确认即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhnyZMgl5GSdLLEB0quDW%252F18-%25E5%25A2%259E%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Da3b06ab8-13f0-43ef-ab63-d4c90dcf27d4&width=768&dpr=3&quality=100&sign=25b5df6b&sv=2)

加池子-增加流动性

假设我们点击撤出流动性，就可以按照比例进行移除相应的代币，然后钱包确认即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1nCxeqvB4Sv0hvRM4MgZ%252F19-%25E7%25A7%25BB%25E9%2599%25A4%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D64c09cd0-d3c7-435b-9f37-856bee4b8635&width=768&dpr=3&quality=100&sign=b0cd71bb&sv=2)

撤池子-移除流动性

## 三、疑问解答

**1、为什么我加了池子后看不到自己的池子，也不能交易？**

  * 答：池子初始化需要一些时间，大概30分钟之后才能看到池子，才能交易


**2、创建资金池的过程中不弹出钱包怎么办？**

  * 答：如果在页面操作时间过久，就会这样，可以刷新页面重试。或者查看一下钱包是否锁住，如果上锁了，把钱包解锁后刷新页面就可以了


**3、Turbos创建池子要收费吗？**

  * 答：根据实际操作经验来看，在Turbos创建池子不收取费用


如有大家还有不明白或者不清楚的地方，请加入官方电报Telegram群：<https://t.me/PandaTool>
