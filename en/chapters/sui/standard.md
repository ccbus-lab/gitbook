# Sui链一键发币教程

全网最详细的Sui链发币教程

Sui堪称是近2个月来的当红炸子鸡，TVL节节攀升、MEME层出不穷。不过Sui作为Move系公链，估计很多人对其代码结构不是很了解，想要参与却不知道如何进行。基于这个因素，PandaTool开发了Sui链一键发币工具，实现无代码开发Sui链MEME币，让任何人都能尽快参与到Sui的生态中。

## Sui发币前提条件

  * 发币之前，务必使用安装好Suiet钱包或者SuiWallet插件：[Suiet钱包安装](/sui/suiet)、[Suiwallet钱包钱包](/sui/slush)

  * 如果没有安装这两个钱包，欧易Web3钱包也是支持的

  * 钱包内最少准备10个SUI，如果数量不够，会导致发币失败

  * 手机发币建议使用Suiet钱包，不要用TP钱包，TP不能传logo。欧易钱包部分手机无法传logo。


## Sui发币教程

### 1、连接Sui钱包

首先，我们需要确保自己已经在浏览器里下载安装了Sui钱包，并在钱包内存储了超过10个SUI代币。如果还没有安装钱包，请参考以下教程：

  * Slush钱包安装教程：<https://help.pandatool.org/sui/slush>

  * Suiet钱包安装教程教程：<https://help.pandatool.org/sui/suiet>


经过多次测试使用，电脑发币我们推荐大家使用**Suiet** 钱包，手机发币我们推荐大家使用欧易Web3钱包。今天这篇教程，主要是教大家进行电脑发币。

钱包安装完成后，打开发币链接：<https://sui.pandatool.org/>，点击右上角“连接钱包”

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FowWkR39Ch5EBfmk2vTtP%252F1-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Da30af6a9-08a1-4bd7-bdee-3df09ec4298d&width=768&dpr=3&quality=100&sign=95a7c05b&sv=2)

这个时候会弹出页面让你选择连接哪种钱包，默认给了三个：SuiWallet、OKX Wallet、Suiet，这里我推荐大家选择Suiet或者欧易Web3钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F8N1GC4zqT5A2GYExPtFp%252F2-%25E9%2580%2589%25E6%258B%25A9%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3De5852244-3165-44ae-a3b6-1651dca24f46&width=768&dpr=3&quality=100&sign=f5c9678d&sv=2)

比如我选择Suiet钱包，点击后，钱包插件会跳出提示，继续点击连接即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FX3RVeQ05qpqJmS9Mr5u6%252F3-%25E8%25BF%259E%25E6%258E%25A5suiet.png%3Falt%3Dmedia%26token%3D963b317e-e5f7-49fa-bc60-41b4314f35d5&width=768&dpr=3&quality=100&sign=2090aab7&sv=2)

连接成功后，右上角会显示你的钱包地址，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fp1XYcHx8djnBcrVQz9F9%252F4-%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D0b32a35b-7294-491e-a719-434dbab05541&width=768&dpr=3&quality=100&sign=9e88cbf3&sv=2)

至此，钱包的连接工作就算是完成了。如果是老手的话，直接跳过这一步，我们进行下一步操作

### 2、输入代币参数

相比较Solana来说，Sui的代币参数比较简单，但是要求比较多，有以下几项

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FRwUUr5dYXRNx7isvhFBQ%252F5-%25E5%258F%2582%25E6%2595%25B0%25E5%25A1%25AB%25E5%2586%2599.png%3Falt%3Dmedia%26token%3D15075281-626b-4bc3-b3e0-1a80dd6cb492&width=768&dpr=3&quality=100&sign=7ddd8822&sv=2)

**参数都要填**

  * **全称：** 不支持中文或符号，最多**32个** 字符

  * **简称：** 不支持中文或符号，需要**2~8个** 字符

  * **精度：** 默认填9，精度与你能填写的最大供应量有关。

  * **供应数量：** 当精度为9时，供应量最大不能超过100亿。当精度为8时，不能超过1000亿，以此类推

  * **logo：** 图片小于**100k** ，尺寸建议256x256像素（正方形）

  * **简介：** 必填，且**不支持中文**


例如我填写的代币信息如下

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fds2yYfNOedhGProRDFEV%252F6-%25E5%25A1%25AB%25E5%2586%2599%25E5%258F%2582%25E6%2595%25B0.png%3Falt%3Dmedia%26token%3D255cafd8-888a-4df3-92f2-c678b15fb5eb&width=768&dpr=3&quality=100&sign=b0051996&sv=2)

这个代币的名字就叫PandaTool，简称叫Panda，logo就是我们平台的logo。确定好信息无误之后，点击“立即创建”按钮，这时候会跳出Suiet钱包，我们确认授权，并支付费用，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWIi1H0stwNXFiayfqQm9%252F7-%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3Dbe6a7003-706f-4531-a8c8-8a58c9c90d38&width=768&dpr=3&quality=100&sign=9aa8f811&sv=2)

当页面出现代币合约地址的时候，就是告诉你代币已经发布完成了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fhqx5bFk6bWWnspmi7q2w%252FScreenShot_2025-12-26_165501_714.png%3Falt%3Dmedia%26token%3De82a4a7c-b8e3-45bf-896c-a447b99ce760&width=768&dpr=3&quality=100&sign=f7bbcafd&sv=2)


这里大家可能会遇到一个问题：点击创建代币的时候，钱包是不是没有弹出？出现这个现象的主要原因有2个：1、整个页面卡顿太久了导致失效，刷新一下页面就行了。2、钱包锁住了，这个时候解锁就行了。锁住的状态就是下面这样：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fxg14cyGik7iqmOVzPLRS%252F11.png%3Falt%3Dmedia%26token%3D85199742-ead5-4c94-923c-d6db7329ffee&width=300&dpr=3&quality=100&sign=63093069&sv=2)

我们按照提示，去Sui浏览器看一下，也能看到代币信息了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQqohZadDAtI279L8yK5M%252F10-%25E6%25B5%258F%25E8%25A7%2588%25E5%2599%25A8.png%3Falt%3Dmedia%26token%3De17b8232-a538-459f-b686-b8139bf13779&width=768&dpr=3&quality=100&sign=36789290&sv=2)

此时我们打开自己的Suiet钱包或者Suiwallet，应该也可以看到代币的logo。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbHx7Qay3fAy0zPO4mHQA%252F12.png%3Falt%3Dmedia%26token%3Df5a49fd0-2bb6-49c2-b94d-2078b967ce5c&width=768&dpr=3&quality=100&sign=c1f17b89&sv=2)

至此，整个发币工作就算是完成了。

如果你需要增发代币或者修改资料，可以参考这个教程

  * Sui代币权限管理：<https://help.pandatool.org/sui/control>


如果你需要为代币创建资金池、添加流动性，可以参考下列教程

  * Cetus加池教程：<https://help.pandatool.org/sui/cetus>

  * Turbos加池教程：<https://help.pandatool.org/sui/turbos>

  * BlueMove加池教程：<https://help.pandatool.org/sui/bluemove>


## 疑问解答

**1、Sui发币需要多少钱？**

  * **答：** 发币费用是9.5 SUI


**2、手机应该怎么发币？**

  * **答：** 手机可以使用欧易web3钱包或者Slush进行操作，不支持TP钱包哦


**3、其他问题**

  * 任何问题，都可以进入Telegram电报群找志愿者解答： <https://t.me/pandatool>
