# BlueMove创建AMM流动性资金池教程

在BlueMove创建AMM流动性资金池

BlueMove是一款基于 Aptos 和 Sui 区块链构建的应用程序，为用户提供 NFT交易、DEX等功能。最初，它只是一个多链NFT市场，后面逐步拓展到集DEX、Bridge为一体的综合应用程序。

值得注意的是，BlueMove也是Sui区块链上为数不多的支持AMM的去中心化交易所，所以PandaTool建议大家可以在这里创建流动性。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPPMSPfQCVXBzFFSqkXLJ%252F1.png%3Falt%3Dmedia%26token%3D122bbc72-573f-4994-b9dc-4b33653e0f3c&width=768&dpr=3&quality=100&sign=55ce46bf&sv=2)


注意：本文仅作为教学演示，所涉及到的资金池和代币均**没有任何实际价值** ，大家也不要进行任何形式的交易。如果因此造成资金损失，PandaTool无法对此负责

## 一、创建流动性资金池

### 1、连接钱包

所有的链上操作第一步都是连接钱包，以识别你的地址。我们打开BlueMove的官网：<https://dex.bluemove.net/> ，点击右上角[**连接钱包** ](https://dex.bluemove.net/connect-wallet)按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FSndfO8TMeMfsNwP4aaNf%252F2.png%3Falt%3Dmedia%26token%3Dec85180e-a769-41b2-8b72-e1d488dc0aff&width=768&dpr=3&quality=100&sign=235fcebb&sv=2)

点击之后，会弹出提示让你选择钱包，我们可以选择Suiet

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FKMry9VCwN6vVMmSm5prU%252F3-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Df6ee8f99-2785-4447-8d2e-98fce291d760&width=768&dpr=3&quality=100&sign=4c1c5503&sv=2)

之后会弹出钱包让你确认，点击继续连接就可以了（如果没有弹出钱包，看一下是不是钱包上锁了）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3gw0Dyo724i9gf5KJkzY%252F4%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Db74da240-7d24-4de2-b9df-fd591710c34f&width=768&dpr=3&quality=100&sign=ea001baa&sv=2)

连接钱包

和所有的DAPP一样，连接成功后右上角会出现钱包地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLRNtOLdMsClnhj7JIoxX%252F5%25E9%2592%25B1%25E5%258C%2585%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D5b48f431-1482-40bd-b78c-18aa0aa4b8b9&width=768&dpr=3&quality=100&sign=7ad1811&sv=2)

钱包连接成功

### 2、找到资金池

我们在首页找到Pools点击进入，直接通过链接进入：<https://dex.bluemove.net/pool>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FUhEN0Skd8qbUDbqzzPaE%252F6-%25E6%2589%25BE%25E5%2588%25B0Pools.png%3Falt%3Dmedia%26token%3Da5ac4daf-d0b1-428b-a4e7-3be5b524589f&width=768&dpr=3&quality=100&sign=d933862d&sv=2)

之后会进入到流动性管理页面，在这个页面你可以看到自己的流动性情况

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FdCtJOCqDdNpTz43sV1uw%252F7-%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Dd20b2874-d108-4dd4-aa06-fc29d3d8aeff&width=768&dpr=3&quality=100&sign=e8f4bc17&sv=2)

我们创建资金池的话，就点击Creat a pool，然后进入到代币选择页面

### 3、确认交易对

左边一般就选择Sui或者USDC、USDT这些，右边就是我们自己发行的土狗币，通过合约地址进行搜索

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FumJX37xaILYlOHjk4Uy7%252F9-%25E6%2590%259C%25E7%25B4%25A2%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Dc053bbf0-c2dc-46c0-9f0d-b1cc9b57a51a&width=768&dpr=3&quality=100&sign=ff112a70&sv=2)

搜索代币

例如我选择用Panda这个币添加流动性，大概就是下面这样

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZaLceKPLkshZPrpuPdiC%252F10-panda%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Ddb74967f-04c7-4d2a-94dd-dce8e82b1793&width=768&dpr=3&quality=100&sign=50d4cc83&sv=2)

### 4、设定初始价格

确认代币交易对之后，下面我们需要输入各个代币的数量与比例

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fa0xGQXx9G2w5gbGBA0wm%252F11%253D%25E4%25BA%25A4%25E6%2598%2593%25E5%25AF%25B9%25E6%25AF%2594%25E4%25BE%258B.png%3Falt%3Dmedia%26token%3Da86454b6-7609-4ebb-8aa9-97b91c5412d4&width=768&dpr=3&quality=100&sign=85cad8fa&sv=2)

创建池子的初始数量和比例，决定了代币的上线价格。例如我加入10SUI和100000000个Panda币，那么代币的上线价格就是10÷100000000=0.0000001SUI。假设SUI的价格是1.8U，那么Panda代币的价格就是：0.0000001 x 1.8 =0.00000018U（注意：该说法仅作为演示，本文涉及到的代币没有任何实际价值）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FFPhpEsH6BzZgPc1xRwzB%252F12-%25E5%2588%259B%25E5%25BB%25BA%25E4%25BB%25B7%25E6%25A0%25BC.png%3Falt%3Dmedia%26token%3D56a690a8-9692-416f-9543-e4c1ab1066f2&width=768&dpr=3&quality=100&sign=418fa77c&sv=2)

确定自己输入的代币数量和SUI数量无误后，点击Creat Pool，此时会弹出钱包让你确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FpCtxvXPDO2rEb9ghvsOs%252F13-%25E5%2588%259B%25E5%25BB%25BA%25E6%25B1%25A0%25E5%25AD%2590%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D185d5973-ca9e-4c6d-899e-daf11cd3fd96&width=768&dpr=3&quality=100&sign=a3d21723&sv=2)

点击Approve之后，等待几秒钟就会有提示告诉你池子创建完成了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fb5G5iOIpmZfRnyHxDITl%252F14.png%3Falt%3Dmedia%26token%3De069f8c9-2ca1-4aff-b984-9812948e9066&width=768&dpr=3&quality=100&sign=e138bd68&sv=2)

### 5、进行代币交易

正常来说，我们在BlueMove做了池子后，就可以在BlueMove的首页进行交易了。但是这个平台不知道遇到什么问题了，加了池子无法交易。因此，我们只能选择另一个平台交易：FlowX

我们打开官网：<https://flowx.finance/trade/swap> ，右上角连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FU3Xt3dG2CEO7q3QWFEbi%252Fflowx%25E4%25BA%25A4%25E6%2598%25931.png%3Falt%3Dmedia%26token%3Daa826ac0-6e6b-4bc6-b2bf-c8860b721b8a&width=768&dpr=3&quality=100&sign=cd263fb0&sv=2)

FlowX连接钱包

之后我们选择代币进行交易

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FlDRkQA3OhFOvcG13x9OM%252Fflowx%25E4%25BA%25A4%25E6%2598%25932.png%3Falt%3Dmedia%26token%3D2c079c0c-b5b9-460f-9f83-235ccb861910&width=768&dpr=3&quality=100&sign=b7d560f8&sv=2)

之后填写代币的交易数量，点击swap确认即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4Js3qe5Ay5R3dKVtAxtB%252Fflowx%25E4%25BA%25A4%25E6%2598%25933.png%3Falt%3Dmedia%26token%3D75aa3e24-e490-4315-a1e0-bd488e82de64&width=768&dpr=3&quality=100&sign=163a0c7&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FrVs6qFK2KJSM5Sorsa0n%252Fflowx%25E4%25BA%25A4%25E6%2598%25934.png%3Falt%3Dmedia%26token%3Da5db67d9-8496-4716-a58a-0ec6ffe462df&width=768&dpr=3&quality=100&sign=fde81821&sv=2)

最后会跳出钱包进行确认授权，并进行代币支出

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FkRp65lqhPanbRhDRmkkV%252Fflowx%25E4%25BA%25A4%25E6%2598%25935.png%3Falt%3Dmedia%26token%3D6ca3b2dc-f92f-405b-b0a0-6cf471a753f4&width=768&dpr=3&quality=100&sign=ca97e6d5&sv=2)

最后交易就完成了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4RyzJfII8LlKhnRCF5qq%252Fflowx%25E4%25BA%25A4%25E6%2598%25936.png%3Falt%3Dmedia%26token%3Da8305ed4-510b-4d5d-94f0-8c810dbd381c&width=768&dpr=3&quality=100&sign=a2654ec4&sv=2)

到这里，创建池子以及交易的流程就介绍完了

## 二、添加与撤出流动性

创建了池子后，如果我们想继续加池子怎么办呢？如果想撤池子怎么办呢？其实也很简单，我们进入BlueMove的流动性管理页面：<https://dex.bluemove.net/pool> ，就能看到自己加的池子

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fz1yEVa7SZFsMJHnGwkZ2%252F15-%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E7%25AE%25A1%25E7%2590%2586.png%3Falt%3Dmedia%26token%3Dbc179077-f687-4a2b-92ce-a9b6b683637c&width=768&dpr=3&quality=100&sign=355fb879&sv=2)

之后我们可以选择加池子（增加流动性）或者撤池子（移出流动性）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9CI6VWEGRyPNEMmZvJjC%252F16-%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E7%25AE%25A1%25E7%2590%2586.png%3Falt%3Dmedia%26token%3D9bf63dcc-90f3-4909-9f7a-c49b9e5f711c&width=768&dpr=3&quality=100&sign=dc15a027&sv=2)

### 1、增加流动性

点击Add liquidity Instead后，按照当前的价格与比例进行添加流动性

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FHJEAwbA1VMueQ5TuQFVU%252F17-%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Da5b9349c-9cac-46d8-8640-a960ccb70cec&width=768&dpr=3&quality=100&sign=a17942b3&sv=2)

之后点击Add Liquidity，会跳出钱包进行确认。授权后，即可完成添加

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fyg4zZ9u8LLLKJ0xk7w8q%252F18-%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Dca37f31f-5f80-4b4b-92ff-5d7746135508&width=768&dpr=3&quality=100&sign=76867723&sv=2)

如果流动性添加成功，会出现以下提示（请确保自己钱包内的代币足够添加）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhdDnTnOX95I5ylJnXq8Z%252F19-%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D8c8d3a2d-8c1c-4393-8ef2-fd2f85ad06fe&width=768&dpr=3&quality=100&sign=34b3d16a&sv=2)

### 2、撤出流动性

撤出流动性或者说移出流动性其实也很简单，在[流动性管理](https://dex.bluemove.net/pool)页面点击Remove，会跳出移除页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9feBlObMZ7Krgqm68Fol%252F20-%25E6%2592%25A4%25E5%2587%25BA%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D44ee94fd-6444-4065-a69b-46d586fcffd9&width=768&dpr=3&quality=100&sign=c5f82c4a&sv=2)

我们可以根据自己的需要选择要移出的流动性比例，从1%到100%都可以选择。确定好比例之后，点击Remove Liqiudity，会跳出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FAEikf8sfBYZzY6aSwx1M%252F20-%25E6%2592%25A4%25E5%2587%25BA%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Dd37b8754-fcdb-4c12-9051-711e664469c7&width=768&dpr=3&quality=100&sign=383df09c&sv=2)

点击钱包的Approve按钮，等待几秒钟后，即可完成流动性的撤出

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqLacZVH0zFFYuGmdGjOr%252F22-%25E6%2592%25A4%25E5%2587%25BA%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D990f2075-94f6-454f-ad96-9f90c492049f&width=768&dpr=3&quality=100&sign=7799ed5b&sv=2)

至此，我们关于BlueMove的加池子、撤池子教程，就算是介绍完毕了。教程写的很详细，大家仔细看都能学会，接下来教大家烧池子（锁LP）

## 三、烧毁池子LP（锁池子）

锁池子的概念其实并不复杂，就是将Lp转移到某个地址不能取出，从而向用户证明自己不能撤池子了。如果是在BSC链，可以带时间锁，到时间就取出。但是在Sui链上，只能通过烧池子的方式完成。池子烧了之后，就不能再撤池子，永久不能撤了。

就以Cetus这个交易所来说，他们提供了烧池的入口，方便快捷。我们进入流动性管理页面：<https://app.cetus.zone/pool/position/> ，找到 Lp Burn按钮，点击进入

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FBFWXgdbOl8kBXK6mO3v9%252F30-%25E7%2583%25A7%25E6%25B1%25A0%25E5%25AD%2590.png%3Falt%3Dmedia%26token%3D0fbde3d3-d5c5-457f-a165-b4cad818db31&width=768&dpr=3&quality=100&sign=9eb869ce&sv=2)

在新的页面勾选您要锁的流动性，然后点击Lock Liquidity，钱包确认即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fa8T5HQdjuQKWkgNUj2MA%252F31-%25E9%2594%2581%25E5%25AE%259A%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D12c2d032-5179-48a2-bf30-17d6ec064099&width=768&dpr=3&quality=100&sign=e3d06da3&sv=2)

注意，流动性是永久锁定，且无法取回，是一个不可逆的操作。一旦完成锁定，将无法撤出该部分池子，请谨慎处理。

## 四、疑问解答

1、创建资金池的时候出现以下错误该怎么办？

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FIoBG9rYJTnvtofMUeRim%252F%25E9%2594%2599%25E8%25AF%25AF%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3Dfbce66fb-4830-4ec7-bb72-e6ed63ab2101&width=768&dpr=3&quality=100&sign=32f9ea24&sv=2)

  * 答：出现这个问题的原因在于钱包网络不在主网，将其切换到主网mainnet就可以了


2、BlueMove创建池子要收费吗？

  * 答：根据实际操作经验来看，在BlueMove创建池子不收取费用


3、为什么在BlueMove创建的资金池不能在他的平台交易

  * 答：这确实是一个令人困惑的问题，经过我们查验，该问题主要是由于他的前端Bug导致的，只能等BlueMove那边自己修复了


如有大家还有不明白或者不清楚的地方，请加入官方电报Telegram群：<https://t.me/PandaTool>
