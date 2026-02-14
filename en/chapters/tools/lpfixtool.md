# LP流动性修复

LP流动性修复视频操作教程：

近期，BSC链上出现了一种新型的无差别攻击方式，有人向新创建的代币资金池地址转入少量的wBNB或者USDT，使得合约创建者无法添加池子，会出现一种提示： _添加流动性失败，未知错误，请尝试提高您的滑点上限。_**或者直接无法加池，不能看到加池页面**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FP75tVnYq4vtuEXGaFtVy%252F%25E6%2597%25A0%25E6%25B3%2595%25E5%258A%25A0%25E6%25B1%25A0%25E5%25AD%2590%25E6%258F%2590%25E7%25A4%25BA2.jpg%3Falt%3Dmedia%26token%3D2ece39a7-346f-4132-9d9a-aafb90124e5e&width=768&dpr=3&quality=100&sign=3e97e271&sv=2)

或者出现这种提示：目前无法在 PancakeSwap UI 上为此 V2 币对增加流动性。请按照说明使用区块链浏览器解决该问题（Adding liquidity to this V2 pair is currently not available on PancakeSwap UI. Please follow the instructions to resolve it using blockchain explorer.）。都表明了，池子遭到了攻击。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOWCwMqJGxQQQ15bwsJsR%252FLP%25E4%25BF%25AE%25E5%25A4%258D%25E6%258F%2590%25E9%2586%25922.png%3Falt%3Dmedia%26token%3D28c6a0f0-47e4-4721-8808-68636d0707db&width=768&dpr=3&quality=100&sign=4fccbbe7&sv=2)

该攻击方式的实现原理是这样的：有人通过脚本监控薄饼的工厂合约，当有新的资金池被创建出来之后，就向该池子地址无差别转入wBNB或者USDT，每次转入数量为0.000000000000001个左右。当池子被转入单种代币之后，就无法创建交易对，从而不能加池。如下图所示：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZylf33EYmn8AlJBye55H%252FLP%25E6%2594%25BB%25E5%2587%25BB%25E6%25A1%2588%25E4%25BE%258B1.png%3Falt%3Dmedia%26token%3D20c46719-d920-4f8d-ace2-d82fb51c0bb8&width=768&dpr=3&quality=100&sign=b8eaa46f&sv=2)

BNB池子被攻击

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FgtmD74cOBWWAHD9AxkXO%252FLP%25E6%2594%25BB%25E5%2587%25BB%25E6%25A1%2588%25E4%25BE%258B2.png%3Falt%3Dmedia%26token%3De7d1fe5a-c225-4d0e-9600-a0b167676093&width=768&dpr=3&quality=100&sign=19edb596&sv=2)

USDT的池子被攻击

据调查，受影响的池子已经达到5000+。该攻击并不会对资金和任何资产造成影响，就是恶心人，搞得非常麻烦，且攻击者不会获得任何好处。为此，我们推出了LP流动性修复工具，任何受此影响的代币和资金池，都可以使用该工具解决这个问题。


请注意，该工具仅用于修复被攻击的流动性池，其本质目的不是用来修改价格的。不用来修改价格，不用来修改价格。使用该工具可能造成巨大未知风险，请在管理员指导下使用。

### 一、操作流程

1、打开工具 <https://pandatool.org/#/LPfixtool>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FXhP4sed2l4VLG8gZBuYs%252FLP%25E4%25BF%25AE%25E5%25A4%258D.png%3Falt%3Dmedia%26token%3Ded2437df-e18d-4a2e-b7d6-c50f9d52575d&width=768&dpr=3&quality=100&sign=e326bac6&sv=2)

2、选择交易所Pancake，输入**资金池地址** 。其中，资金池地址可以在控制台查询，如：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCNIlpJKm2JMSiX4TNEmI%252F%25E6%25B1%25A0%25E5%25AD%2590%25E5%259C%25B0%25E5%259D%2580%25E6%259F%25A5%25E8%25AF%25A2.png%3Falt%3Dmedia%26token%3Dedc8661e-f524-4ecb-a4d2-97a2fcb62cb6&width=768&dpr=3&quality=100&sign=5069d4de&sv=2)

**3、点击“查询池子”，** 可以看到池子中的代币数量

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCfi9ZyvQrzcjQrWg8OVm%252F%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%259F%25A5%25E8%25AF%25A2.png%3Falt%3Dmedia%26token%3Dfa7f0bb1-daab-4c0f-b048-8568421128a1&width=768&dpr=3&quality=100&sign=14d44f06&sv=2)

可以看到，目前池子里被人恶意转入了0.00000000000001个USDT，这也是你无法正常加池子的原因

**4、确定目标价格**

根据你的开盘价格，分别输入你自己发行的代币的数量和底池代币的数量。例如，你要做的是USDT的池子，且开盘价定为0.001U，那么你需要在左边输入1000个代币，右边输入1个USDT。如果是BNB的池子，那就相应的使用wBNB（如果钱包没有wBNB，可以在薄饼兑换）。具体如图：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWHS71UTHBmgp40pY7Nl3%252FLP%25E4%25BF%25AE%25E5%25A4%258D-%25E7%259B%25AE%25E6%25A0%2587%25E4%25BB%25B7%25E6%25A0%25BC%25E7%25A1%25AE%25E5%25AE%259A.png%3Falt%3Dmedia%26token%3D893fcaf1-5433-4866-8b04-5cc307cbb5eb&width=768&dpr=3&quality=100&sign=97defa56&sv=2)

注意，不管是1000个代币还是1U，都不是你要最终加池的数量，它只是用来确定你的代币价格比例，仅此而已。具体应该往池子里放多少币？需要点击 _**核算加池数量**_ ，然后会给你一个数据，如：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9VQvV1cfOL06OYGw0ijA%252F%25E6%25A0%25B8%25E7%25AE%2597%25E5%258A%25A0%25E6%25B1%25A0%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D574621d5-cdc2-4e98-9502-c3f5ae80bbdb&width=768&dpr=3&quality=100&sign=e66ec7e9&sv=2)

这个数据就是你修复需要使用的代币数据，接下来就是授权了

**5、授权并修复**

分别对你自己发行的代币和USDT进行授权（如果是BNB的池子，就需要授权wBNB），当两个代币分别授权完成之后，点击**“确认修复”** ，即可完成修复。之后再去薄饼加池子，就可以正常加入了。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fbpc6Pw3FzQdvrS8LsiK3%252F%25E7%25A1%25AE%25E8%25AE%25A4%25E4%25BF%25AE%25E5%25A4%258D.png%3Falt%3Dmedia%26token%3Dc788b2d0-cc1a-42ef-859d-2de2599679ef&width=768&dpr=3&quality=100&sign=500d79db&sv=2)

### 二、注意事项

#### 1、给修复合约添加白名单

假设您的代币拥有交易开关功能，在未开启交易之前，需要将修复合约的地址添加到**税率白名单** 里（通过控制台操作），之后才能完成修复，否则会修复失败。

 _修复合约地址：0xEbd1Ad0f26088FC150128e4d55Cb5dB738eB4159_

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FtK2DXZzPqD6KTViyFd2N%252F%25E7%25A8%258E%25E7%258E%2587%25E7%2599%25BD%25E5%2590%258D%25E5%258D%2595.png%3Falt%3Dmedia%26token%3Dfd5d776a-c3cf-49ac-a232-fa8ce74c600f&width=768&dpr=3&quality=100&sign=6e3da51e&sv=2)

税率白名单

#### 2、任何代币都能修复

不管是在PandaTool平台发行的代币，还是在其他平台发行的代币，只要遭遇了池子被攻击的问题，都可以使用本修复工具解决

#### 3、修复失败怎么办

如果按照教程完成了操作步骤，依然修复失败，请加入电报群，联系客服处理 [@pandatool](https://t.me/pandatool)
