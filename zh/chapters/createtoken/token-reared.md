# 持币分红教程

币安链持币分红（万能分红）合约创建视频教程：

持币分红合约教程 

### 合约功能

1、有黑名单、白名单 、销毁、营销钱包等功能 

2、持币分其他币（USDT、USDC等），不支持分本币

3、持币分红可以设置门槛

4、发币之后，可以调整买卖税率 

5、电报交流群：https://t.me/pandatool

### 一、代码参数 

  * name_ = "Jack Token";//名称

  * symbol_ = "Jack";//简称

  * totalSupply_ = 300000;//供应量 不用后面 18 位 

  * rewardAddr_ = XXXXXXXX;//分红币合约地址 

  * marketingWalletAddr_ = XXXXXX;//营销钱包地址 

  * buyFeeSetting_ = [1,1,1,1];//买入税：持币分红、回流、营销钱包、销毁 

  * sellFeeSetting_ = [1,1,1,1];//卖出税：持币分红、回流、营销钱包、销毁 

  * tokenBalanceForReward_ = XXXX;//持币门槛，后面+18 个 0


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FkebD1sfs3uNog6M2pJtQ%252F%25E4%25BB%25A3%25E7%25A0%2581%25E4%25BF%25AE%25E6%2594%25B9.png%3Falt%3Dmedia%26token%3Dc72ed022-73fb-4ada-a6d2-58fd08b32065&width=768&dpr=3&quality=100&sign=d049f2f7&sv=2)

代码修改

### 二、编译参数

  * 版本号 COMPILER： v0.8.17+commit.e28d00a7.js 

  * Enable optimization: 开启并使用默认值 200


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F85ryL3HHw8MdyW4M9Teb%252F%25E5%259B%25BE%25E7%2589%25871.png%3Falt%3Dmedia%26token%3Dd7ed04b6-6e6a-4ddb-aead-c91f8548908e&width=768&dpr=3&quality=100&sign=3efbdd54&sv=2)

合约编译

### 三、合约部署

  * Environment：选择第三个Injected Provider Metamask

  * GAS LIMIT：默认不用该

  * Value：50000000000000000（5后面16个0）


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FNJpPDffqeq8nhKCtyHZF%252F%25E5%259B%25BE%25E7%2589%25872.png%3Falt%3Dmedia%26token%3D1b40d634-e30d-4028-bc18-458737945956&width=768&dpr=3&quality=100&sign=9f877dc&sv=2)

合约部署

### 四、合约开源

  * 选择文件类型：solidity（Single file）单文件 

  * 选择版本号：v0.8.17+commit.e28d00a7.js 

  * 选择开源许可证类型：No licernes


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FlCmvI8vJZxYeuTdpWnHN%252F%25E5%2590%2588%25E7%25BA%25A6%25E5%25BC%2580%25E6%25BA%2590.png%3Falt%3Dmedia%26token%3Dc30401a7-02ca-4043-98b5-bf35a715ab75&width=768&dpr=3&quality=100&sign=31c5a7ed&sv=2)

合约开源

Optimization是否优化：yes

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FmXxH6fBfNCSBthJh3W0E%252F%25E6%2598%25AF%25E5%2590%25A6%25E4%25BC%2598%25E5%258C%2596.png%3Falt%3Dmedia%26token%3D2512dd7c-44f9-4132-979b-a3a697e8344f&width=768&dpr=3&quality=100&sign=19f74953&sv=2)

是否优化

### 五、修改合约

在权限没放弃的情况下，可以在区块链浏览器找到代币合约的Write Cntact页面，在连上钱包之后，调用下列的函数进行修改：

1、EnemyAddress 设置黑名单

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FwCa9fgUcQNWufqVc2hbl%252F%25E9%25BB%2591%25E5%2590%258D%25E5%258D%2595.png%3Falt%3Dmedia%26token%3D91e86263-ea07-4367-a5d3-85a857ed2ff0&width=768&dpr=3&quality=100&sign=1b6dc979&sv=2)

设置黑名单

10、renounceOwnership 放弃权限

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FDWY9FiBcCxfu56CMO81z%252F%25E6%2594%25BE%25E5%25BC%2583%25E6%259D%2583%25E9%2599%2590.png%3Falt%3Dmedia%26token%3D7cf3e723-fffc-4ab6-ac77-2405c3601bfb&width=768&dpr=3&quality=100&sign=61a8cc07&sv=2)

12~15 调整买入税率：销毁比例、流动性比例、营销钱包比例、分红比例

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQviqaERIsMrJxaCy2XNz%252F%25E4%25B9%25B0%25E5%2585%25A5%25E7%25A8%258E%25E7%258E%2587.png%3Falt%3Dmedia%26token%3Dd24ea7bd-5eff-4915-9471-a01918d2c504&width=768&dpr=3&quality=100&sign=e29f5225&sv=2)

设置买入税率

17 修改营销钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FsrmZS2q0TK747FeDtgGd%252F%25E8%25AE%25BE%25E7%25BD%25AE%25E8%2590%25A5%25E9%2594%2580%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D335a5da0-f5fa-4300-a0d2-0208a091cf96&width=768&dpr=3&quality=100&sign=2c4f54b0&sv=2)

设置新的营销钱包地址

18~21调整卖出税率：销毁比例、流动性比例、营销钱包比例、分红比例

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4ARSl1VwHKvsEdsXzcK1%252F%25E5%258D%2596%25E5%2587%25BA%25E7%25A8%258E%25E7%258E%2587.png%3Falt%3Dmedia%26token%3Dd80e257b-e786-4325-beb5-175f034ed93d&width=768&dpr=3&quality=100&sign=9a3324f4&sv=2)

设置卖出税率

26 transferOwnership转让合约权限

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEnNARXkksCFjVjsSE7uL%252F%25E8%25BD%25AC%25E8%25AE%25A9%25E5%2590%2588%25E7%25BA%25A6%25E6%259D%2583%25E9%2599%2590.png%3Falt%3Dmedia%26token%3D750fc367-78a6-46f1-b495-631d4261cc90&width=768&dpr=3&quality=100&sign=d67c8f16&sv=2)

转让合约权限

### 六、注意事项

1、合约代码仅能在BSC主网使用，若想在其他链使用，请自行修改

2、不能分BNB、wbnb这两个币

3、如果卖出税率出现异常，可以尝试提高滑点多卖几笔

4、如果资金池撤不出来，请选择Wbnb撤出

5、池子必须是BNB池子，且最好大于1BNB，不可以是USDT池子或者其他池子

6、博饼池子必须V2 的池子，不能加V3的池子

7、要分红的币，必须是此前就在博饼已经有了足够的BNB池子

### 七、合约代码下载

上述合约代码文件及相关教程下载链接：

  * 百度网盘：<https://pan.baidu.com/s/1PXqB3Ggo7sKh-ffW54swTA?pwd=qzev >

  * Mega网盘：<https://mega.nz/folder/kHtHBayB#QXN6czytHkkdJCIRAwuU1g>
