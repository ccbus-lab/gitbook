# 如何锁仓与锁池？

**锁仓，** 指的是将一定额度的代币锁在某个地方，这些代币将无法流入市场。**锁池，** 指的是将LP锁在某个地方，这样项目方将无法撤池，以确保项目的稳定运行。

在教大家锁仓和锁池之前，先简单回答几个问题：

### 1、权限丢了还能撤池子吗？

答：丢权限和撤池子没有关系，池子只有锁了才不能撤出。

### 2、锁池的原理是什么？

答：简单来说，当你在pancakeswap或者uniswap加了V2的池子后，交易所会给一些LP代币。这些LP代币就是你拥有该池子的凭证，所谓撤池，就是将LP代币给回到交易所，然后交易所就把相对应的流动性给你了。所以锁池，就是将LP代币转移到某个地方无法取出，这样就锁住了。

### 3、锁池有几种方式？

答：锁池一般有两种方式：永久锁和带时间锁。

  * **永久锁池：** 将LP代币转入黑洞地址，这样永远无法取出，池子永久锁住。

  * 黑洞地址：0x000000000000000000000000000000000000dEaD

  * **带时间锁：** 将LP代币转入某个第三方锁池合约，到时间将LP取回即可。


### 4、什么是LP代币？

答：即流动性资金池 (Liquidity Pool, LP) 代币。当您提供两种代币 (A 和 B) 作为流动性时，您得到是 LP 代币作为收据凭证。

### 5、如何查看LP代币？

答：当你创建好资金池之后，链上会生成一个资金池地址，这个资金池地址就是LP代币的合约地址。你可以在钱包里添加这个地址，就能看到自己的LP代币数量了。

### 6、池子有权限吗？

答：池子是没有权限这个概念的，因为资金池是所有人共有的，任何一个添加流动性的人，都拥有相应比例的份额。例如一个池子只有一个人加流动性，那么他就掌握了所有池子。如果一个池子有100人加流动性，那么每个人按照比例掌握相应的份额。

### 7、具体应该如何锁池？

如果按照时间锁，可以选择PinkSale平台（免费），接下来就给大家演示一下锁池的步骤

#### **第一步：选择锁池平台**

我们选择PinkSale粉红锁池，打开链接：<https://www.pinksale.finance/pinklock/create> 既可以在手机钱包里打开，也可以在浏览器里打开。网站打开之后，连上钱包，会看到如下页面：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fx5latWCDOXIVIbwe1rnU%252F%25E9%2594%2581%25E6%25B1%25A0%25E9%25A1%25B5%25E9%259D%25A2.png%3Falt%3Dmedia%26token%3D8058089e-6019-46be-9fca-73de0335a8db&width=768&dpr=3&quality=100&sign=aa202de5&sv=2)

锁池页面

#### **第二步：填写代币或者LP合约地址**

如果你填写的是代币合约地址，那么你就是锁仓（锁币）。如果你填写的是LP合约地址，那么你就是锁池。

代币合约地址好理解，LP合约地址怎么获得呢？要么从区块链浏览器里查询，要么从Ave里面查询。在Ave展示的代币行情页面，可以看到池子地址，复制它：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVlqYhgkhkgyKS2QfS5D8%252F%25E6%25B1%25A0%25E5%25AD%2590%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D5525cbf3-b846-4ab2-b821-d6a08f15365d&width=768&dpr=3&quality=100&sign=e8703cce&sv=2)

Ave代币页面

这个池子地址就是你的LP地址。此外，你还可以通过PandaTool的控制台查看并复制池子地址，如下图所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F0DdeaKp3zwSdDheCzK3T%252F%25E5%25BE%25AE%25E4%25BF%25A1%25E6%2588%25AA%25E5%259B%25BE_20231226183607.png%3Falt%3Dmedia%26token%3Dbbb5fb57-e44d-45c6-91f9-f545a4eb8f82&width=768&dpr=3&quality=100&sign=30f34a26&sv=2)

复制之后，输入LP地址，就能看到你当前钱包的LP数量了，如下图所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FP82TYfp421tFpF23PkZV%252FLP%25E4%25BD%2599%25E9%25A2%259D.png%3Falt%3Dmedia%26token%3Dc25717b2-b946-4987-89d2-75b080a833e1&width=768&dpr=3&quality=100&sign=f1c33bcb&sv=2)

#### **第三步：写个标签Totle**

这个所谓的标签，可填可不填，主要是用来分辨的。假设你锁了很多池子，或者锁了很多代币，有个标签可以帮助你快速找到每个锁。

#### **第四步：确实锁池份额（数量）**

根据上图可知，我现在有15174.667012422317318271个LP代币，我可以选择将这些LP全部锁了，也可以选择锁一部分，每一部分锁不同的时间，都可以。为了方便操作，我选择MAX，全部锁池：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FcjRIDVObNDEt9nKZ06Yb%252F%25E9%2594%2581%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D852281c7-f57d-4b8e-a45f-7e7543b028ad&width=768&dpr=3&quality=100&sign=4a017d61&sv=2)

注意，use vesting是一种较为复杂的循环释放方式，搞不懂的话可以不管。

#### **第五步：确定锁池日期**

也就是解锁的时间。注意：该时间为UTC时间，与北京时间相差8个小时。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fo20dw8Us9qJaJmit81LW%252F%25E9%2594%2581%25E6%25B1%25A0%25E6%2597%25B6%25E9%2597%25B4.png%3Falt%3Dmedia%26token%3D591f9807-9a2f-4baf-8735-7fe0ceaf95a9&width=768&dpr=3&quality=100&sign=d6581f1d&sv=2)

锁池时间

可以看到，我将池子锁到2027年7月8日下午14：40分。这个是UTC时间，换算成北京时间要加8个小时，就是2027年7月8日下午22：40分。

#### **第六步：授权**

在确定好锁池份额和时间后，点击授权。此时钱包会要求你支付一笔gas费，并确认要授权的LP代币数量。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9FJ4BHCA88tMDdnwqXDX%252F%25E6%258E%2588%25E6%259D%2583%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D209d6153-f790-475c-b66a-221553b7733f&width=768&dpr=3&quality=100&sign=c338a27b&sv=2)

授权并批准

#### **第七步：锁池**

很多人以为授权完就结束了，其实不是。授权只是将你的代币授权给合约，还没有开始锁。授权成功后，还需要点击**“锁”** 这个步骤，然后支付gas费，才能锁池成功。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FSbB6P9PzUuKRzYidZt2T%252F%25E9%2594%2581%25E6%25B1%25A0png.png%3Falt%3Dmedia%26token%3Db5f6cffd-05bc-4f9f-93b9-55ea015dfcdd&width=768&dpr=3&quality=100&sign=cec8f960&sv=2)

锁池

#### **第八步：查询锁池信息**

怎么确认自己是否锁池成功呢？我们打开锁池查询页面：<https://www.pinksale.finance/pinklock/liquidity> 输入LP合约地址，就能查询到你的锁池信息，如下图所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fp92o0M15X7rnBQXA2gOB%252F%25E9%2594%2581%25E6%25B1%25A0%25E4%25BF%25A1%25E6%2581%25AF1.png%3Falt%3Dmedia%26token%3D3bebf599-63e3-4b63-80f4-4f6c2d9466ed&width=768&dpr=3&quality=100&sign=245cb0f6&sv=2)

锁池查询

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FN0kVEtWja1zEg4yo3Gyb%252F%25E9%2594%2581%25E6%25B1%25A0%25E4%25BF%25A1%25E6%2581%25AF2.png%3Falt%3Dmedia%26token%3Dbe9a252a-5d76-4706-9102-dc74ba0f21e5&width=768&dpr=3&quality=100&sign=27cf51a5&sv=2)

锁池详细信息

### 7、锁仓应该怎么锁？

锁仓的操作和锁池是一样的，只是把LP地址换成代币合约地址即可。查询锁仓信息，可以在该页面查询：<https://www.pinksale.finance/pinklock/token>

### 8、其他锁池平台

除了粉红PinkSale之外，还有几个其他的锁池平台：

  * 绿马锁池：<https://app.uncx.network/>

  * DxLock锁池：<https://dxsale.app/dxlock>


### 9、V3的池子能锁吗？

目前大多数锁池平台，暂时均不支持V3的池子锁池。
