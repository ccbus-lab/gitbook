# 代币与LP链上解锁教程

通过区块链完成代币或者流动性的解锁

如果我们通过PandaTool将代币或者LP锁住了，没到解锁时间，PandaTool网站无法打开了（尽管这种情况发生的可能性几乎为0）。这种情况下，我们该如何完成代币或者LP的解锁呢？到了时间，我们该如何取回自己的代币？

今天这篇教程，就是教大家通过区块链浏览器来完成代币或者LP的解锁。

  * PandaTool锁池工具：<https://ccbus.cc/liquidity-control/create-lock>

  * PandaTool解锁工具：<https://ccbus.cc/liquidity-control/lock-console>


### **一、解锁操作指南**

首先，我们需要在区块链浏览器找到锁池合约（以BSC链为例）：<https://bscscan.com/address/0x407993575c91ce7643a4d4ccacc9a98c36ee1bbe#writeContract>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FALYC22tLRYVNbUB6kMtg%252F1web3.png%3Falt%3Dmedia%26token%3D84ceeee2-9043-48d5-979a-a79e7c6cd0b0&width=768&dpr=3&quality=100&sign=16c81799&sv=2)

打开之后，点击那个**Connect to Web3，然后** 连接上钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FYaUgXr2Ra67tnLmFLyWd%252F2%25E7%25A1%25AE%25E5%25AE%259A.png%3Falt%3Dmedia%26token%3D4d31c27a-f3ba-463e-9daa-7c0108c3624f&width=768&dpr=3&quality=100&sign=8cc9316c&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOzUpKtWeFznjME1MmzRi%252F3%25E9%2593%25BE%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D89c62e2e-2e07-4fc7-ae48-d9f194b1477f&width=768&dpr=3&quality=100&sign=4dce602d&sv=2)

需要注意的是，一定要用锁池/锁仓的那个钱包连接，不然没有意义。哪个钱包锁的，哪个钱包才有权限操作。

接下来，我们找到第7个选项：unlock，在里面需要输入一个数值lockid，指的就是锁ID

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F5pxVMkwaQcmieXfLSpPP%252F4unlock.png%3Falt%3Dmedia%26token%3Dd6438874-ae3b-45f6-bc06-2e0d3f3967e2&width=768&dpr=3&quality=100&sign=9bc0a756&sv=2)

这个ID是多少呢？我们不知道，需要去查。

怎么查？找到你当时锁池/锁仓的哈希，在区块链浏览器里搜索，然后点击那个logs

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6ihr6rLXwfz07SKiFCSQ%252F5logs.png%3Falt%3Dmedia%26token%3D7e14cae6-f0ad-4788-925a-5e51084e4982&width=768&dpr=3&quality=100&sign=1111732c&sv=2)

然后在最下面有两个数值，分别是ID和unlockDate，把这两个数值记下来：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FaSW0NgVGfzy8n9Mkjn64%252F6%25E6%2595%25B0%25E5%2580%25BC.png%3Falt%3Dmedia%26token%3Dc31d8346-d98f-49d4-93a2-40da970dc960&width=768&dpr=3&quality=100&sign=97555baf&sv=2)

这个ID（1348849）就是刚才需要输入的，而这个unlockDate（1767110400）就是你的解锁日期。该数字需要通过时间戳来转换具体得日期时间，可以在这里转换：<https://tool.lu/timestamp/>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQQ3IFKGNNloFTzkhWU8R%252F7%25E6%2597%25B6%25E9%2597%25B4%25E6%2588%25B3.png%3Falt%3Dmedia%26token%3Ddb960053-4cf6-4155-a9d4-f95e5cec2f8c&width=768&dpr=3&quality=100&sign=3b6e49e4&sv=2)

可以看到，1767110400经过转换之后，就能获得一个时间是2025年12月31日。在这个时间，我们才能操作解锁。

假设你的锁时间已经过了，那么就会回到刚才的**unlok** 操作页面，在输入框里输入**1348849** ，然后点击**Write** ，弹出钱包确认即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FIOChQoIXObcdbLYsalAR%252F8unlock.png%3Falt%3Dmedia%26token%3Dabc57c82-f561-4f9d-80cf-36b91da78b93&width=768&dpr=3&quality=100&sign=e19bc664&sv=2)

到这里，整个解锁流程就完成了。接下来，是一些可能涉及到的疑问，我也一并给大家解答一下

### **二、解锁疑问解答**

**1、为什么我点击write没有反应？**

  * **答：** 只有两个原因，要么是您没有连钱包，或者是链接的钱包不是当初锁的钱包。要么就是还没到解锁时间，所以操作不了。


**2、为什么我的时间戳转换的日期不对？**

  * **答：** 时间戳日期转换，分别有**秒** 和**毫秒** 两种格式。我们平台锁仓给的时间戳都是按照秒的格式转换，有些时间戳是毫秒，所以这个不要搞错了。如果不对，换一下就行


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fs5G2GXQlAPMVFXxGwrtO%252F9%25E6%2597%25B6%25E9%2597%25B4%25E6%2588%25B3%25E7%25A7%2592.png%3Falt%3Dmedia%26token%3D59e2f0e8-3849-4d05-8ce9-01b2fead9dfa&width=768&dpr=3&quality=100&sign=23409f36&sv=2)

**3、找不到当初锁的哈希怎么办？该如何获得时间戳以及LockID？**

  * 答：如果操作时间太久，导致你找不到当时操作的锁池/锁仓哈希，以至于无法获得ID。那么还有其他办法。


我们需要在锁合约里Read Contact页面，找到`**normalLocksForUser**`函数和`**lpLocksForUser**`函数。进入页面：<https://bscscan.com/address/0x407993575c91ce7643a4d4ccacc9a98c36ee1bbe#readContract>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FK5IFrotm8D2VBE539RFO%252F10%2520foruser.png%3Falt%3Dmedia%26token%3D4b632ebc-e1f5-42b5-b441-1f1b94a73a21&width=768&dpr=3&quality=100&sign=a1879950&sv=2)

  * **14 lpLocksForUser：** 假设你锁的是池子/LP，那么就在这里输入创建锁的钱包地址，点击**Query** ，就能得到LockID，以及时间戳

  * **17 normalLocksForUser：** 假设你锁的是代币，那么就在这里输入创建锁的钱包地址，点击**Query** ，就能得到LockID，以及时间戳


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FwzFficOLzkM7Y3wZAiNF%252F11%25E6%259F%25A5%25E8%25AF%25A2.png%3Falt%3Dmedia%26token%3Df97cca64-331c-4b76-9a54-a92ff2aa2bb6&width=768&dpr=3&quality=100&sign=ee2e0264&sv=2)

总的来说，针对代币和LP，分红要调用不同的合约函数去获得ID和时间戳，但流程都是一样的。

如果你针对这个锁还有什么问题，可以进入我们的官方Telegram，咨询志愿者：<https://t.me/pandatool>
