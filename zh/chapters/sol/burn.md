# Solana销毁代币、烧池教程

将Solana链的池子燃烧掉

  * **烧池子：** 将LP代币销毁，无法撤出流动性

  * **燃烧代币：** 将任何代币销毁，减少代币供应量


### 烧池概念问答

**1、LP是什么东西？**

  * 答：LP本身也是一个代币。当您在创建流动性的时候，Raydium会给你发放一些LP代币作为凭证（类似于：银行存单）。以后你去撤池子，钱包就会自动将LP转给Raydium销毁掉，然后Raydium就让你把流动性撤出。所以，它是一个流动性/池子凭证。


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3FoW68yyXZZEMJwnUrLG%252FLp.png%3Falt%3Dmedia%26token%3D4d4eeae5-43e1-4808-80f8-ddbfe25ed50a&width=768&dpr=3&quality=100&sign=daaf656f&sv=2)

**2、销毁LP又是什么意思？**

  * 答：前面我们提到，LP是一个流动性凭证。Raydium只认Lp，不认钱包（ _银行只认存单，不认人_ ）。如果将Lp转移给被人，那么别人就可以撤。谁有这个LP，谁能撤池子。如果将LP销毁掉，那就说明这个LP不存在了，无法再撤出流动性了。这个就是我们说的**烧池子** 。


**3、烧池子是什么意思？池子烧完还能交易吗？**

  * 答：很多人误区，认为池子烧了，池子里面的Sol和代币就不存在了，这是错误的观念。销毁LP=烧池子=无法撤池子。注意，池子依然存在，只是不能撤了而已。所以，**烧完池子后还能交易** ，不受影响。

  * 如果你自己将银行存单烧了，这个笔钱还是在银行的，只能没人可以取了。


通过我们的工具，大家不仅可以烧池子，也能将代币销毁掉，具体操作的教程如下：

打开链接<https://solana.ccbus.cc/burn>，右上角连接你的Phantom钱包（如未安装钱包，可参考→[Phantom安装教程](/sol/phantom)）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FKw1dQjuslFX4hwVazhIQ%252F%25E9%2580%2589%25E6%258B%25A9%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D80530c3a-becd-45dc-85bd-654844608863&width=768&dpr=3&quality=100&sign=2b0f97b6&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqrmzAYWhaxYQK0PAPaYF%252F%25E9%2580%2589%25E6%258B%25A9phantom.png%3Falt%3Dmedia%26token%3Dd0611d81-9cfd-4165-b7c4-f1dafc5a02bd&width=768&dpr=3&quality=100&sign=5ad717ff&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOY5Y97N5BOzV99Hh17SO%252F%25E9%2592%25B1%25E5%258C%2585%25E5%25B7%25B2%25E8%25BF%259E%25E6%258E%25A5.png%3Falt%3Dmedia%26token%3D04d64a8e-bcdb-4909-9fa1-f32a10d72207&width=768&dpr=3&quality=100&sign=e4406d3c&sv=2)

连上钱包后，在选择框能看到你钱包内目前拥有的代币和LP

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGw3O9z71kzUgfKPuS9Qr%252F%25E7%2587%2583%25E7%2583%25A7%25E4%25BB%25A3%25E5%25B8%2581%25E9%25A1%25B5%25E9%259D%25A2.png%3Falt%3Dmedia%26token%3D53265ef8-fc43-4d2b-9206-35d3b1ebde09&width=768&dpr=3&quality=100&sign=d9c8e4ab&sv=2)

这个时候，你想烧毁代币，就点击代币，大概页面是这样的：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FxwL2xhUItWZqAGobKsyB%252F%25E7%2583%25A7%25E6%25AF%2581%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D99033709-e524-495c-9603-7072cec04d3e&width=768&dpr=3&quality=100&sign=fde79fcd&sv=2)

想烧毁LP，就点击LP。烧毁LP，就是烧池子，大概页面是这样的

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjIpMpGfInIX1F58o0W1C%252F%25E9%2594%2580%25E6%25AF%2581LP.png%3Falt%3Dmedia%26token%3Db2a8a7c1-77ea-41e7-8ca1-1318a94a83c8&width=768&dpr=3&quality=100&sign=6807a8c6&sv=2)

当查询到你钱包的LP数量之后，你可以填入销毁LP的数量，然后点击“销毁”就行。当然，你想全部销毁，就把右边那个“全部销毁并关闭账户”给勾选上，然后点击销毁，钱包确认就行了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FJRG2vFoAzHYppobwn8zv%252F%25E9%2594%2580%25E6%25AF%2581%25E5%25B9%25B6%25E5%2585%25B3%25E9%2597%25AD%25E8%25B4%25A6%25E6%2588%25B7.png%3Falt%3Dmedia%26token%3D5e3708ba-7c55-4d97-a251-731c2ad81135&width=768&dpr=3&quality=100&sign=bedf0af8&sv=2)

## 疑问解答

#### 1、关闭账户是什么意思？

  * **答：** 你每收到一个新的代币，Solana系统会自动在你的地址里开设一个代币存储账户。所谓“关闭账户”，就是把代币全部销毁，账户也关掉的意思。关闭账户并不影响你自己的钱包，因此不用担心。


**2、NFT可以销毁吗？**

  * **答：** 在Orca加池子获得是NFT，这个暂时是不支持销毁/烧池的。目前可以销毁的是Ryadium和Meteora的LP。


**3、烧池后还能撤回流动性吗？**

  * **答：** 烧池后，永久无法撤出流动性


有任何烧池子的问题，可以在电报群联系志愿者：https://t.me/pandatool
