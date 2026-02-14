# Meteora DLMM稳定池创建教程

在Meteora为Solana代币创建DLMM稳定币池

传统意义上，如果我们要让一个Solana代币的价格保持稳定，可以创建Raydium CLMM稳定池。关于这种类型的资金池，PandaTool有详细的创建教程与工具

  * Raydium CLMM稳定池创建工具：<https://solana.ccbus.cc/createpool>

  * Raydium CLMM稳定池创建教程：<clmm.md>


不过，近期PandaTool更新了新的稳定币池创建工具：Meteora DLMM资金池。Meteora是Solana区块链上三大知名的DEX之一，虽然诞生的比Raydium晚，但是凭借技术创新在Solana迅速发展，成为最大的DEX之一。其创新的DLMM资金池类型，可以帮助项目方实现代币价格稳定的同时，获取交易收入。


注意：DLMM稳定池可能不被欧易Web3钱包支持，用户可以跳转到第三方DAPP交易，如Meteora、Jupiter等

### 创建DLMM稳定池的步骤

1.打开PandaTool流动性创建页面

2.确定两种代币，并创建池子

3.进一步创建仓位

4.钱包确认并支出费用和代币

5.进行代币交易

6.管理流动性（增加/移除） 

### 创建Meteora DLMM稳定池的详细教程

#### 1、打开PandanTool并连接钱包

第一步，我们需要打开PandaTool的DLMM流动性创建工具：<https://solana.ccbus.cc/meteora> ，或者从菜单栏打开，也能进入

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOtX00tsTKkF9niEYiOVL%252F1%2520%25E6%2589%25BE%25E5%2588%25B0%25E5%2588%259B%25E5%25BB%25BA%25E5%25B7%25A5%25E5%2585%25B7.png%3Falt%3Dmedia%26token%3D5ac6a410-46ee-4361-af0b-60b56985e5db&width=768&dpr=3&quality=100&sign=2cc772c9&sv=2)

之后在右上角连接钱包，此时会跳出Phantom钱包进行连接，点击之后会自动识别Phantom钱包插件，并在右上角出现你的钱包地址，这就说明钱包连接成功了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQ7BILorNuxmttPoobDh8%252F2%2520%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D6e24072b-c947-4461-8d71-2440436c393d&width=768&dpr=3&quality=100&sign=a4374353&sv=2)

#### 2、选择代币并创建资金池

钱包连接成功后，PandaTool会自动查询您钱包内的代币，并让您选择要创建流动性的代币：

  * **基础代币：** 就是您创建发行的代币（注意：**不支持税率代币** ）

  * **报价代币：** USDT、USDC、SOL等主流代币


当我们选择好两种代币之后，系统会自动查询，确定该代币之前是否创建过流动性

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FrmQCRNH0e15kYPzSBGlA%252F3%25E8%25BE%2593%25E5%2585%25A5%25E5%2590%2588%25E7%25BA%25A6%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D906d0657-975b-48cf-8e83-2deb2eef332b&width=768&dpr=3&quality=100&sign=3013eab&sv=2)

查询完成后，接下来是输入交易价格。假设我输入的价格是1，我选择的基础代币名称是PandaTool、报价代币是USDT，这就意味着，在我创建好流动性资金池后，我的代币PandaTool的价格将以USDT作为基准，即**1PandaTool=1USDT** 。假设我填0.1，那么就意味着1PandaTool=0.1USDT，以此类推


该价格是永久交易价格，以后不敢交易多少次、交易多少数量，价格都不会变。而且一旦创建后不可修改，价格永久稳定。

填写好交易价格后，我们点击创建按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fp8kZU3Ws9b83pPNnZmJG%252F4%2520%25E5%2588%259B%25E5%25BB%25BA.png%3Falt%3Dmedia%26token%3D0f312583-167a-400a-9038-4f653be67def&width=768&dpr=3&quality=100&sign=b311f033&sv=2)

此时会弹出钱包进行确认，点击确认即可完成创建

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F8zMrdUKG46Uib0qmMdt4%252F5-2%2520%25E7%25A1%25AE%25E8%25AE%25A4%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3D59f7e480-f88c-439b-8e69-966f8a0b603f&width=768&dpr=3&quality=100&sign=343a25f5&sv=2)


注意，如果钱包有提示：`此交易在模拟过程中已被撤销`，则说明创建会失败，因为Meteora DLMM不支持带有税率的Token2022代币，只支持无税Token2022

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FD1xqW3V9IdzUXEIPp0YM%252F5%2520%25E9%2594%2599%25E8%25AF%25AF%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3D557f027a-47c5-4ea2-9f87-54e06e0fbaac&width=300&dpr=3&quality=100&sign=3caa8f67&sv=2)

到这一步，你的资金池就算是创建完成了。

此时你一定会疑惑：**我还没往资金池里放代币呢，怎么就完成了呢？** 别着急，放代币的问题，我们在下一步完成。

#### 3、创建流动性仓位

正如我们刚才所说，虽然池子里面创建成功，但是此时池子里依然是没有代币的。我们需要为资金池创建一个流动性仓位，这样才算是真正意义上的完成。因为没有流动性，就意味着无法交易。

如何创建呢？首先，我们还是要在这个页面。选择好代币后，系统会自动查询是否有资金池。**等待几秒钟** ，如果查询到有，就会跳转到仓位页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWMRZkGdnVNX4FCx2w5n4%252F8%25E8%25B7%25B3%25E8%25BD%25AC%25E6%258F%2590%25E7%25A4%25BA.png%3Falt%3Dmedia%26token%3Df2863088-6039-4b44-a273-24820df93d3f&width=768&dpr=3&quality=100&sign=8162e068&sv=2)

跳转之后，您就可以看到代币流动性的操作管理页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FgrLJOkSTcj6e4UW3C91I%252F9%2520%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D95d0947a-235b-4c2f-9b57-bbbcd04416ad&width=768&dpr=3&quality=100&sign=7994b948&sv=2)

在仓位页面，您可以看到当前池子的代币数量，以及要添加的代币数量、价格范围等信息。目前，池子内没有任何代币，所以数量为0。接下来，我将分别填入两种代币数量：、

  * PandaTool：100000枚

  * USDT：1枚


注意，两种代币的数量**可以随意填** ，无需遵照任何比例。比如我现在设置的价格是1，但是添加代币的数量无需按照1:1的比例添加，随意就行。

确认好入池数量后，点击添加流动性按钮，此时会弹出钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLUUkSHvKdXOuTKLh7I6y%252F10%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A72.png%3Falt%3Dmedia%26token%3Dd4576ca9-eed5-413c-b294-3cf2c4442608&width=768&dpr=3&quality=100&sign=49bfe6d6&sv=2)


在添加流动性的时候，请确保钱包内有至少**0.5个SOL** ，否则可能无法交易

等待几秒钟后，流动性仓位即可创建成功，此时就能看到代币的流动性了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FvnCw6UCSCMIKS7FV6LjN%252F11%2520%25E5%2588%259B%25E5%25BB%25BA%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Dfd5d4752-b873-47ff-a7b5-5fcf3e2c6e47&width=768&dpr=3&quality=100&sign=3c0d204e&sv=2)

#### 4、交易代币

既然流动性创建成功了，下面就可以交易了，以确定价格是否稳定。还是在这个页面，点击交易按钮进入交易页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FMpVGm5le2BRDX10JBLYh%252F12%2520%25E4%25BA%25A4%25E6%2598%2593%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D500c997e-8176-41a5-9f16-1c9cde31aa43&width=768&dpr=3&quality=100&sign=8896462b&sv=2)

可以发现，0.1USDT购买0.0999个代币，价格基本稳定在1USDT，浮动在万分之一左右，可以忽略不计，稳定性很高。兑换完成之后，可以看到池子里面的代币金额相应发生了变化

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FMByMF7k225VRnjKD43I0%252F13%25E5%2585%2591%25E6%258D%25A2%25E5%25AE%258C%25E6%2588%2590.png%3Falt%3Dmedia%26token%3D34dc5afb-4eb0-41d4-80e7-49ab3d6bed71&width=768&dpr=3&quality=100&sign=95bcce7f&sv=2)

#### 5、管理流动性

当我们成功创建流动性仓位以后，接下来可以进行多项操作管理，包括增加流动性、移除流动性、关闭流动性仓位以及领取奖励等，下面给大家一一说明

**1）增加流动性**

顾名思义，增加流动性就是往池子里添加代币，使得流动性更大、更充足。我们点击流动性的按钮，可以进入到流动性管理页面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FIZ3gF1EnskNVYviWvbOX%252F14%2520%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%258C%2589%25E9%2592%25AE.png%3Falt%3Dmedia%26token%3D812c3e6c-9757-4ef1-939f-3829affe6097&width=768&dpr=3&quality=100&sign=a20a9f6a&sv=2)

之后根据需要填写对应的代币添加数量，钱包确认后，即可增加流动性

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPyrLNUsLY7FTtC26zYvL%252F15%2520%25E5%25A2%259E%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Dd544e44e-382b-4d48-83e0-4977d0e79c11&width=768&dpr=3&quality=100&sign=27ed7895&sv=2)

**2）移除流动性**

在同一个页面，点击移除流动性按钮，并选择要移除的比例，钱包确认后即可移除

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FA2t5mEJwQzJiVuwC59HI%252F16%2520%25E7%25A7%25BB%25E9%2599%25A4%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Ddbedc16f-752e-4f60-bd37-2df349dd711c&width=768&dpr=3&quality=100&sign=cdf454bd&sv=2)

**3）领取费用**

这个领取的费用，指的是交易手续费。目前该手续费默认是0.01%，如果该资金池交易数量足够大的话，是可以领取到不少资金的。我们只需要点击领取按钮，会自动弹出钱包进行确认的

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZdDO4ClI0MCnRgkSAXQL%252F17%25E9%25A2%2586%25E5%258F%2596%25E5%25A5%2596%25E5%258A%25B1.png%3Falt%3Dmedia%26token%3D7c9e1e78-cbdd-444e-9f90-4c83891073a7&width=768&dpr=3&quality=100&sign=e9a299fa&sv=2)

**4）关闭流动性**

所谓关闭流动性，指的是完成撤出并将整个仓位关掉。关闭之后，可以获得Meteora退还的0.05SOL左右的创建费用。

具体如何操作呢？我们在移除流动性页面，选择移除100%流动性，然后选择对应的按钮，钱包确认后即可关闭

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEpFYNyQBl2MZRQ14U6Sg%252F18%25E5%2585%25B3%25E9%2597%25AD%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3Da767b7f7-604d-487b-a9d4-3a2e60102ba6&width=768&dpr=3&quality=100&sign=62cab6d6&sv=2)

### 创建DLMM稳定池疑问解答

**1、资金池创建成功后，为什么还不能交易**

  * **答：** 资金池创建只是第一步，还需要创建流动性仓位。因为，需要进入流动性管理，添加流动性才可以。


**2、资金池和流动性仓位都创建成功后，可以在哪里交易？**

  * 答：首先，在PandaTool的Meteora流动性管理页面，支持代币交易。您还可以去Meteora、Jupiter等平台进行交易


**3、交易时可以保证价格百分百稳定吗？**

  * 答：完全可以。通常来说，不管交易多少数量的代币，价格幅度范围不会超过千分之一。假设您设置的交易价格为1USDT，那么实际交易的价格会在0.99~1.0001之间浮动


**4、为什么我创建失败了？**

  * 答：Meteora不支持带有税率的代币，如果您是带有转账税率的Token2022的代币，则创建会失败。此外，创建仓位的话，钱包内应有不少于0.5个SOL，否则可能因为余额不够导致失败。


**5、创建DLMM稳定池，需要多少费用？**

  * 答：第一步创建资金池是不需要费用的，创建仓位需要将近0.4SOL的费用。


如果您对创建Meteora DLMM资金池还有其他的问题，可以加入我们的Telegram交流群：<https://t.me/pandatool>
