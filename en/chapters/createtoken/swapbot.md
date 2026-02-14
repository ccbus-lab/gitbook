# 代币批量交易/市值管理教程

使用PandaTool的批量交易机器人

## **一、市值工具解读**

该工具是PandaTool开发、针对于以太坊兼容链的市值管理工具升级版，不仅支持了更多的链，工具速度、支持的资金池类型也有显著提升。

### **1、功能概念**

用户可以导入多个钱包地址，针对某一代币进行批量交易。通过设定交易次数、交易价格等要素，来实现交易的停止与启动。其目的在于解放双手，快速实现代币的大量交易。

### **2、支持类型**

该市值管理工具支持多条区块链、多个资金池类型，具体如下：

  * **BNB Chain：** PancakeSwap V2、PancakeSwap V3

  * **Ethereum** ：Uniswap V2、Uniswap V3

  * **Avalanche：** Uniswap V2、Uniswap V3

  * **Polygon：** Uniswap V2、Uniswap V3

  * **Arbitrum、Optimsim、Base：** Uniswap V2、Uniswap V3


## **二、市值工具使用教程**

我们打开市值工具的操作页面：<https://evmswap.pandatool.org/> 然后根据以下教程进行操作

### **1、查询资金池**

第一步，我们需要选择基础的信息，包括链、代币等：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FJ122hbI4xwJIElir71BR%252F1%25E5%259F%25BA%25E7%25A1%2580%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3D4e06f7fd-c5e0-4e61-9dd2-162f5657ca59&width=768&dpr=3&quality=100&sign=9d9e648b&sv=2)

  * **选择链：** 选择您要交易的区块链，目标代币在哪条链，就选择哪条链

  * **交易所：** 选择您创建的资金池类型，主要是V2和V3的区别

  * **报价代币：** 就是您的资金池代币，一般是BNB、ETH、USDT等，看下您的资金池交易对

  * **代币地址：** 您要交易的目标代币地址，直接填进来


确定好信息填写无误后，我们点击查询资金池：

  * 如果查询没问题，则页面右边会出现代币i的价格，并提示您资金池正常


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZuwIORokxKUElGRzSyVM%252F3%25E6%259F%25A5%25E8%25AF%25A2%25E6%25AD%25A3%25E5%25B8%25B8.png%3Falt%3Dmedia%26token%3Dfb5be02e-d537-45d8-b05f-71e36e32c5f4&width=768&dpr=3&quality=100&sign=483967b9&sv=2)

  * 如果查询有问题，会提示您查询错误，您需要核对选择的区块链或者交易所是否正确


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLhjne57ET9IWec3o3gZ3%252F2%25E6%259F%25A5%25E8%25AF%25A2%25E9%2594%2599%25E8%25AF%25AF.png%3Falt%3Dmedia%26token%3De93a4722-6478-43b7-9cb9-d3051272e806&width=768&dpr=3&quality=100&sign=457b4a19&sv=2)

### **2、导入钱包**

查到资金池和价格后，我们点击右边的按钮导入钱包（私钥）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLrQVS8C6uLRn9jspqgDs%252F4%25E5%25AF%25BC%25E5%2585%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Da6d29345-56d1-48de-860f-faf65be19f59&width=768&dpr=3&quality=100&sign=20e3b57e&sv=2)

在弹出的页面输入钱包的私钥，一行一个，然后点击导入私钥。（一般导入几十个就可以了）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4CfI2ZfUwUidbws9AtKo%252F5%25E5%25AF%25BC%25E5%2585%25A5%25E7%25A7%2581%25E9%2592%25A5.png%3Falt%3Dmedia%26token%3D5aa972e7-80fc-4632-8399-abc5f1cf67d4&width=768&dpr=3&quality=100&sign=9c9bade0&sv=2)

钱包导入之后，我们就能看到各个钱包地址了，然后点击**刷新余额** ，确认一下钱包内的代币情况

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FvmDLcCtN3oc5ZUiHsJVr%252F6%25E5%2588%25B7%25E6%2596%25B0%25E4%25BD%2599%25E9%25A2%259D.png%3Falt%3Dmedia%26token%3D704258fc-0068-4c5d-a567-63b75e245bad&width=768&dpr=3&quality=100&sign=1614783e&sv=2)

余额刷新之后，我们进行下一步

### **3、买入与卖出交易设置**

目前代币的交易方式有三种，分别是：**买入交易、卖出交易和刷量交易，** 同时会选择不同的操作类型。现在我们了解一下买入和卖出的交易设置

#### **金额类型（使用买入和卖出同理）**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3d5L1AagDEMZrXolcQqz%252F7%25E9%2587%2591%25E9%25A2%259D%25E7%25B1%25BB%25E5%259E%258B.png%3Falt%3Dmedia%26token%3Dee48e1b5-2b46-4cb9-8749-6f416cb0b611&width=768&dpr=3&quality=100&sign=668d0858&sv=2)

  * **按照数量：** 设定每笔交易的买入数量，以报价代币计算（如USDT，BNB等）

  * **按照比例：** 设定每笔交易钱包支出的余额比例

  * **范围：** 设定交易数量或者比例的范围


**关于比例：** 这个比例是钱包余额的比例。如果您设置1%，钱包内1000U的话，那么第一笔交易就是10U。此时钱包内只有990U了，那么第二笔交易就是9.9U，以此类推

#### **停止类型（买入和卖出同理）**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FpZRlnjJaoMvZqsICvX15%252F8%25E5%2581%259C%25E6%25AD%25A2%25E7%25B1%25BB%25E5%259E%258B.png%3Falt%3Dmedia%26token%3D981fad1e-8d5b-4d33-b7db-86de3ce82849&width=768&dpr=3&quality=100&sign=dc7042&sv=2)

  * **按价格：** 就是到了某个价格，停止交易

  * **按次数：** 交易了多少次之后，就停止交易

  * **间隔：** 每一笔交易的间隔时间，以秒为单位

  * **线程数：** 同一秒发起多少笔交易，线程越大，交易频率越高（最大为6）


#### **设置案例**

例如我填写的代币交易设置是这样的：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FlPJw6iZCiBdBM71Ewyql%252F9%25E4%25BA%25A4%25E6%2598%2593%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3D2aec806b-bc57-436a-a601-17593e8d7b14&width=768&dpr=3&quality=100&sign=d668cc1b&sv=2)

这是一笔批量买入的交易，每次买入的金额是0.0001BNB到0.001BNB之间。一共交易6次就停止，没错交易间隔时间为0~3秒，不固定，线程数是2.

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FR94BiYRadcGcJbVKyCoX%252F10%25E5%25BC%2580%25E5%25A7%258B%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3D47b845a9-d27d-4c7f-aef0-380f8c0315d2&width=768&dpr=3&quality=100&sign=cd411cb2&sv=2)

设定完成后，我点击右边的开启交易按钮，即可开始交易

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FlaUelszn5BcNUn6q92k6%252F11%25E4%25BA%25A4%25E6%2598%2593%25E6%2597%25A5%25E5%25BF%2597.png%3Falt%3Dmedia%26token%3De6e8a9d5-a2eb-4661-bc2d-a8e096a3de46&width=768&dpr=3&quality=100&sign=10010e7f&sv=2)

可以看到，如果钱包内gas不足，会直接跳过。一旦达到停止条件，会自动停止交易。

### **4、买卖交易设置**

不同于前面两种针对某个方向的交易，买卖交易指的是自动实现买和卖两种交易方式。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FJ3QGW3f14BBLYR9k6k7F%252F12%25E4%25B9%25B0%25E5%258D%2596%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Dca5e63d6-5a19-4a7a-a94c-b4718f803dee&width=768&dpr=3&quality=100&sign=14f61db7&sv=2)

**金额类型（仅支持按数量交易）**

  * **按数量：** 输入您要交易的代币数量范围

  * ~~**按比例：**~~~~设定每笔交易钱包支出的余额比例~~


**买卖概率**

  * **买单概率：** 系统发起一笔交易时，这笔交易是**买单** 的概率有多大

  * **卖单概率：** 系统发起一笔交易时，这笔交易是**卖单** 的概率有多大

  * 买单概率与卖单概率相加为100%


**数量设置**

  * **买入：** 设置每笔买单的买入数量范围（如果数字一样，则为固定数量）

  * **卖出：** 设置每笔卖单的卖出数量范围（如果数字一样，则为固定数量）


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FrWuBudOPZKINwYCXsrM8%252F13%25E4%25B9%25B0%25E5%258D%2596%25E6%2595%25B0%25E9%2587%258F%2520%25E8%258C%2583%25E5%259B%25B4.png%3Falt%3Dmedia%26token%3D7dc5ec25-1282-41ba-bbdb-856ec10d9164&width=768&dpr=3&quality=100&sign=bfef671a&sv=2)

**停止方式（设置交易次数）**

  * **按次数：** 当买卖笔数达到多少笔时停止交易

  * ~~**按价格：**~~~~达到多少价格时停止交易~~

  * **间隔：** 每一笔交易的间隔时间，以秒为单位

  * **线程数：** 同一秒发起多少笔交易，线程越大，交易频率越高（最大为6）


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FMnQnHyF2nTWxJiVIk2OR%252F14%25E4%25BA%25A4%25E6%2598%2593%25E5%2581%259C%25E6%25AD%25A2.png%3Falt%3Dmedia%26token%3D139ee1d0-173f-434d-8a28-96dae36237a6&width=768&dpr=3&quality=100&sign=8ae55946&sv=2)

设定完成后，我点击右边的开启交易按钮，即可**开始交易**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnnABLeJzzrTqnNvJzB0E%252F15%25E5%25BC%2580%25E5%25A7%258B%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3D2655615c-967b-4b8e-b514-240a22e6b47f&width=768&dpr=3&quality=100&sign=cc3a7759&sv=2)

## **三、疑问解答**

**1、代币地址没有错，为什么提示错误？**

  * **答：** 如果确认代币地址没有错，那么可能是您选择的区块链错误，或者是交易所资金池类型错误


**2、为什么会交易失败？**

  * **答：** 通常的原因是钱包内Gas不足或者代币余额不足导致的


**3、私钥会不会泄露？**

  * **答：** 私钥仅保存在您的电脑页面，不上传至服务器，至少PandaTool是看不到的


**4、最多可以导入多少钱包？**

  * **答：** 理论上是没有上限的，但考虑到您的电脑CPU以及用户体验，几十个应该是比较合适的


**5、市值管理工具如何收费？**

  * **答：** 您可以在右上角查询我们的收费标准


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FTu0upzghIbiWda54KkSi%252F16%25E6%2594%25B6%25E8%25B4%25B9%25E6%25A0%2587%25E5%2587%2586.png%3Falt%3Dmedia%26token%3De2307c05-46e9-45cd-9336-40da6c9468e7&width=768&dpr=3&quality=100&sign=227ab29a&sv=2)

如果您在市值管理工具的运行过程中，遇到了无法解决或者不清楚的地方，可以在PandaTool的官方交流群联系客服处理：<https://t.me/pandatool>
