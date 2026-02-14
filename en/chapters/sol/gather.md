# Solana批量归集教程

Solana最强批量归集工具

批量归集，顾名思义就是将多个钱包地址里面的代币(和sol)集中转账到一个地址，方便大家对钱包进行管理，也就是我们常说的**多对一** 。归集之后的主接收钱包继续使用，其他钱包就放弃了。对于一些需要多地址交易和控盘的用户，以及撸毛用户来说，这个功能还是相当有用的。

接下来，我将通过这个教程让大家学会使用在Solana链上进行钱包批量归集

## Solana批量归集教程

### 1、填写信息并导入钱包

首先，我们打开Solana批量归集的官网：<https://solana.pandatool.org/gather> ，按照下图顺序和要求，填写并配置相关信息，同时导入要`归集`的钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FJYKTiKtjeQqoKaxRDLm4%252F%25E6%2589%25B9%25E9%2587%258F%25E5%25BD%2592%25E9%259B%2586%25E6%25B5%2581%25E7%25A8%258B%25E5%259B%25BE.jpg%3Falt%3Dmedia%26token%3D1ba7d11f-ec5b-4dfb-94e9-7606dda9e011&width=768&dpr=3&quality=100&sign=9f3684b3&sv=2)

  * **接收地址：** 接收归集代币的指定钱包地址

  * **归集代币：** 要归集的代币合约地址，如果不填就默认是sol

  * **导入钱包：** 导入要归集的钱包`私钥`

  * **刷新余额：** 刷新钱包内代币余额


### 2、选择归集方式

  * **发送全部：** 将钱包内某个`指定代币`全部归集到指定的钱包地址

  * **归集数量：** 可以自定义要归集的代币数量，如果部分钱包数量不足，将跳过

  * **保留余额：** 在钱包内保留固定余额的代币，其余的归集出去。如果余额不够，将跳过


### 3、核对信息并归集

当我们将所有信息填写完成后，大概可以得到下图所示的样子

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FgbKoFrBFBowx3FvxzpgC%252F%25E7%25A1%25AE%25E8%25AE%25A4%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3D300b0e38-c0e1-4981-b364-65d8a5051a68&width=768&dpr=3&quality=100&sign=37fac3dd&sv=2)

确认归集的地址和代币无误后，点击归集，等待几秒钟，就会出现归集结果，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjxXy3npUzyUguVVNnHqW%252F%25E5%25BD%2592%25E9%259B%2586%25E7%25BB%2593%25E6%259E%259C.png%3Falt%3Dmedia%26token%3D8bd98515-3774-429c-ba08-b450150ef422&width=768&dpr=3&quality=100&sign=764fe790&sv=2)

不管执行结果是成功还是失败，都会给你展示出来。如果遇到失败的情况，可以点击地址栏的`执行`按钮，再次执行归集

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPvdXik5LF2KyTJre3CLe%252F%25E5%258D%2595%25E4%25B8%25AA%25E9%2592%25B1%25E5%258C%2585%25E6%2589%25A7%25E8%25A1%258C%25E5%25BD%2592%25E9%259B%2586.png%3Falt%3Dmedia%26token%3D3d25123f-58c6-4705-9e33-a048f644b771&width=768&dpr=3&quality=100&sign=13c3242c&sv=2)

## Solana归集疑问解答

**1、为什么归集会失败？**

  * 如果接收地址没有该代币的话，第一个归集地址可能会失败，此时点击**执行** 即可

  * 如果要转账的地址内的sol余额不足，也有可能会失败

  * 如果solana区块链刚好卡住了，也会导致部分钱包失败


**2、归集需要收费吗？**

  * PandaTool的归集产品，除了**gas** 以外，每个地址会象征性收取0.0001sol的费用，以观察归集成功率


**3、为什么归集后没有返回结果？**

  * 可能是链卡住了，耐心等待几秒钟，就会有结果返回的


有任何关于批量归集的的问题，可以在电报群联系志愿者：<https://t.me/pandatool>
