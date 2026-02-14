# STON.fi加池子(创建流动性)教程

在STON上创建AMM资金池

[STON.fi](http://ston.fi/)是一个基于 TON 区块链的去中心化自动做市商 (AMM)，也是TON链上最大的去中心化交易所。提供几乎零费用、低滑点、极其简单的界面以及与 TON 钱包的直接集成。

## 为什么选择 STON.fi

STON.fi 成立于 2022 年。它的目标是建立一个用户友好的加密货币交易所，通过接触 `Telegram `受众来实现大规模采用。 STON.fi 高度重视社区，代表着一个人性化的 `DEX`，为用户提供快速支持并考虑他们的意见。

具有分片功能的 TON 区块链架构允许 STON.fi DEX 用户每秒进行数百万笔交易。

如果你想在TON区块链上发行代币并使其可以交易，[STON.fi](http://ston.fi/)是一个很棒的选择。这篇文章，将教大家在[STON.fi](http://ston.fi/)创建代币流动性，也就是俗称的加池子，和撤池子。

## STON加池子教程

### 1、连接钱包

首先，我们打开STON的官网：<https://app.ston.fi/pools> ，点击右上角`Connect Wallet`

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FDq31mC8p3B503KRsqwJr%252F%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Dbce4909f-eafe-4eba-916f-3c2ccc222f23&width=768&dpr=3&quality=100&sign=d8f663b6&sv=2)

此时会弹出一列钱包让你选择，如果你安装了`Tonkeeper`，就选择这个（[Tonkeeper安装教程](/ton/tonkeeper)）。如果你安装了OpenMask，就选择OpenMask。一般来说，我们会推荐大家使用Tonkeeper

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FkXfICr3xm7HSEwnD7wx8%252F%25E9%2580%2589%25E6%258B%25A9Tonkeeper.png%3Falt%3Dmedia%26token%3Db1b6771c-c4ab-4d2e-9f17-134d024d4529&width=768&dpr=3&quality=100&sign=1a39d33b&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FvgXQKY9GCON1QK1vP2xc%252F%25E9%2580%2589%25E6%258B%25A9%25E6%25B5%258F%25E8%25A7%2588%25E5%2599%25A8.png%3Falt%3Dmedia%26token%3Ddeb25901-bd79-4226-bb1a-01b06ea2f43e&width=768&dpr=3&quality=100&sign=73b68c7b&sv=2)

然后会弹出钱包插件，点击`连接钱包`即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FskJcoSoWdlRJm7zmirel%252F%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585%25E6%258F%2592%25E4%25BB%25B6.png%3Falt%3Dmedia%26token%3D6f1826d8-3839-45dc-b49e-72c5dba9d030&width=768&dpr=3&quality=100&sign=9744d968&sv=2)

连接钱包

连接成功之后，右上角会出现你的钱包地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhTVyaVCFi6aw0X8cvCIA%252F%25E9%2592%25B1%25E5%258C%2585%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D5c36f840-1402-4708-89b2-6b7a296ac852&width=768&dpr=3&quality=100&sign=29def10f&sv=2)

钱包连接成功

### 2、创建流动性

点击页面的`Add liquidity`，并选择你要`加池`的代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOtQNrCDCRjNMSPkfqmOt%252F%25E6%25B7%25BB%25E5%258A%25A0%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7.png%3Falt%3Dmedia%26token%3D2fc040a0-3909-49fc-8797-347e29e82fc7&width=768&dpr=3&quality=100&sign=86eda1d4&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FuRYEmAjcdNy6gqhTXBZ7%252F%25E5%25A1%25AB%25E5%2586%2599%25E4%25BA%25A4%25E6%2598%2593%25E5%25AF%25B9.png%3Falt%3Dmedia%26token%3D12ee775a-8f83-498b-9461-ca1f0bb60d77&width=768&dpr=3&quality=100&sign=12de2635&sv=2)

输入代币合约地址，并且确定要添加的代币数量

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fl0TeIzmfTEXTbQ8gJwwB%252F%25E7%2582%25B9%25E5%2587%25BB%25E5%2590%258C%25E6%2584%258F.png%3Falt%3Dmedia%26token%3Dd766367d-a63b-4c61-9bcd-d091f211b091&width=768&dpr=3&quality=100&sign=c5c5291e&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLuVy6rnYatn47ljssTow%252F%25E8%25BE%2593%25E5%2585%25A5%25E4%25BB%25A3%25E5%25B8%2581%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D7484fa29-f25a-4e99-8763-934d10ccaad4&width=768&dpr=3&quality=100&sign=b4295305&sv=2)

注意，两个代币数量的比例，决定了代币的初始价格。例如，我添加1TON和100000个Panda，说明Panda代币的上线价格是0.00001TON。按照TON的价格5.9U计算的话，我的代币上线初始价格就是0.000059

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqehoK3EY7hL8nymc8SLf%252F%25E7%25A1%25AE%25E5%25AE%259A%25E6%2595%25B0%25E9%2587%258F%25E5%2592%258C%25E6%25AF%2594%25E4%25BE%258B.png%3Falt%3Dmedia%26token%3Df2c69cf3-0b56-4437-9f6a-f41119fd4fb8&width=768&dpr=3&quality=100&sign=5befabf&sv=2)

确定好数量和比例后，点击Create Pool，此时会让你进行二次确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F98gNXFW4gyot4AOT84cj%252F%25E4%25BA%258C%25E6%25AC%25A1%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D415f80b8-5274-4ae6-8842-a66367864865&width=768&dpr=3&quality=100&sign=f70a8c7b&sv=2)

注意，创建一个资金池，可能需要支出0.3~1.6TON的手续费，所以建议你的钱包至少得有2TON。如果算上加池子的费用，可能还需要更多的TON。

确认无误后，点击Confirm，会弹出钱包，钱包确认就可以了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FoP4nSuSPwhl6aoJnbm5G%252F%25E5%2581%259A%25E6%25B1%25A0%25E5%25AD%2590%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D6e5584b9-2daf-4233-ab39-88e357c31d78&width=768&dpr=3&quality=100&sign=409c442f&sv=2)

## STON加池子注意事项

**1、STON上面没有代币头像怎么办？**

  * 答：需要在STON完成申请，且池子内有超过1万U的流动性，才能进入到STON的默认列表里，从而获得头像。申请链接：<https://docs.google.com/forms/d/e/1FAIpQLScGTZjf5DVRutqykFKF477MHoFS9-qzPhkdbOKmo_hZn66FVA/viewform>


**2、创建流动性的时候提示余额不够？**

  * **答：** 在STON创建池子，连同gas，需要额外支出1.7个TON，他会要求钱包里至少2.7TON才能发起交易


**3、在STON上面交易需要支付费用吗？**

  * **答：** 每笔交易需要支出0.3%的费用，其中0.2% 的费用将作为增加资金池规模而支付给流动性提供者的费用，0.1% 的费用支付给STON.fi协议


如有不明白或者不清楚的地方，请加入官方电报群：<https://t.me/PandaTool>
