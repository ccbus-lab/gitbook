# 创建标准代币Mint预售教程

100%去中心化的预售合约创建教程

**什么是标准Mint预售？**

简单来说，就是通过Mint的方式进行预售。项目方将一定数量的代币打入预售合约地址，开启预售后，用户将BNB转入预售合约地址，预售合约会自动按照设定好的比例，将代币给到用户。


注意：创建预售的前提是，必须先创建代币。没有代币，无法预售

## 一、预售功能说明

  * **无前端：** 不需要任何网页，纯合约支持，100%**去中心化**

  * **转账即预售：** 用户将BNB转到`预售合约`，就能**自动** 获得代币

  * **不用领取：** 参与预售的用户**无需** 手动领取代币

  * **自定义功能：** 项目方可以在预售开始后通过控制台**修改** 预售价格和每份数量

  * **无软顶/硬顶：** 没有软顶或者硬顶的概念，只有一个预售总数量（份数x每份数量）


## 二、注意事项提前说明

  * 标准代币预售期间，可能会有人提前加池

  * 建议使用手动开启交易功能，以防止被加池交易

  * 请勿将预售地址加入黑名单，否则无法交易


## **三、标准Mint预售创建教程**

### **1、连接钱包（老手请忽略）**

首先，我们打开预售创建官网：<https://ccbus.cc/presales/create>，右上角点击连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjaYwyhZIo7caum3ByfMp%252F1-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D646f459f-27d6-4b10-84db-cc67eecb11d4&width=768&dpr=3&quality=100&sign=118be3e1&sv=2)

之后会弹出小狐狸让你确定要连接的钱包地址，选择一个就行了。然后下一步就是选择公链，如果您要在币安创建预售，就选择BSC。如果要在Base链创建预售，就选择Base

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fto2I45fnkhnHMnT4mrz6%252F2-%25E9%2580%2589%25E6%258B%25A9%25E5%2585%25AC%25E9%2593%25BE.png%3Falt%3Dmedia%26token%3D5c12898f-492e-4007-94ba-afa9f2fbe4e4&width=768&dpr=3&quality=100&sign=188fa091&sv=2)

之后就能在右上角看到你的钱包地址和链状态，说明已经链接成功了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FOyggh30XarBUzDeYIypN%252F3-%25E9%2593%25BE%25E5%2590%258D%25E7%25A7%25B0%25E4%25B8%258E%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3Dd2b119cc-c122-490c-be03-87d829b937c0&width=768&dpr=3&quality=100&sign=eb37c865&sv=2)

### **2、填写预售参数**

钱包连接成功后，我们通过PandaTool可视化页面创建预售，还是那个页面<https://ccbus.cc/presales/create> 打开，填写相应的预售参数：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FcXAqUQFcRW3TLdEUHKHu%252F1%25E6%25A0%2587%25E5%2587%2586Mint.png%3Falt%3Dmedia%26token%3D52f6ff9f-6d8f-4c47-861b-a1c4c8f78c2f&width=768&dpr=3&quality=100&sign=1bce69c8&sv=2)

  * check

**预售名称：** 随便起一个，如：Presale，不支持中文，只能用英文名

  * check

**预售代币地址：** 要预售的代币合约地址（前提是有代币）

  * check

**每份价格：** 每份预售需要支付多少费用，最小的价格是0.001（BNB或ETH）

  * check

**每份数量：** 每份预售里有多少个代币

  * check

**总份数:：** 一共可以预售多少份（每份数量x总份数≤代币发行总量）

  * check

**单次预售最大份数：** 一次最多可以买几份

  * check

**单钱包预售最大份数：** 一个钱包地址最多可以买几份 _（单钱包最大份数必须小于单次预售最大份数）_


例如我填写的内容如下

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F2g5Ws1v94mmY6Vz4TDt4%252F2-%25E9%25A2%2584%25E5%2594%25AE%25E5%258F%2582%25E6%2595%25B0%25E5%25A1%25AB%25E5%2586%2599.png%3Falt%3Dmedia%26token%3D84e2abae-77e8-433e-973b-6de4e7e188b9&width=768&dpr=3&quality=100&sign=c6608f1f&sv=2)

参数填写完成后，点击创建合约，此时会弹出提示，让你再次确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3y4VjPFEVN4DykCk9pyk%252F3-%25E5%2588%259B%25E5%25BB%25BA%25E5%2590%2588%25E7%25BA%25A6.png%3Falt%3Dmedia%26token%3D84f5185a-413d-42f7-afc4-df929c1e49a7&width=768&dpr=3&quality=100&sign=e0145ce&sv=2)

注意，开源参数无需复制，现在是自动开源的了

然后会弹出小狐狸钱包进行确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLD1L854k1LYpUDmuIfgO%252F4-%25E7%2582%25B9%25E5%2587%25BB%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3Dd4c9a127-75eb-4633-b400-326e32f85a3a&width=768&dpr=3&quality=100&sign=b64484db&sv=2)

点击后等待几秒，就会提示你预售创建完成。如果钱包内BNB/ETH余额不够，可能会导致失败

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQ9idTZdBr9C0jwJkZ62Z%252F5-%25E5%2588%259B%25E5%25BB%25BA%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D41c81afd-6614-4ed5-954f-e0dd390207ab&width=768&dpr=3&quality=100&sign=24b12671&sv=2)

**为什么点击创建没有反应？**

  * check

有可能是钱包没连上，核查一下钱包连接情况

  * check

有可能是代币合约填错了，核查一下合约地址


### **3、预售控制台操作**

创建成功后，我们进入到控制台：<https://ccbus.cc/presales/create>，看下该如何操作这个预售

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fm5GN0gbgtJdZfkExwXyw%252F6-%25E6%258E%25A7%25E5%2588%25B6%25E5%258F%25B0.png%3Falt%3Dmedia%26token%3Dcfe950a3-335a-4700-91a2-81ca77c0a68d&width=768&dpr=3&quality=100&sign=b56f8293&sv=2)

  * check

**预售控制**

    * **转让所有权** : 将合约权限转让给其他人（转移权限之前，记得复制`控制台链接`。新的权限地址必须通过控制台链接，才能进入控制台操作）

    * **开启预售：** 点击后钱包确认，即可开启预售

    * **提取合约内代币：** 可以将预售合约里面的价值币和代币提取走

  * check

**参数控制**

    * **修改每份价格 :** 重新修改预售价格，最低0.001

    * **修改每份数量：** 重新修改每份数量

    * **修改总份数：** 根据实际情况重新修改总的预售份数

    * **修改单次Mint最大份数：** 根据需求修改单次预售上限

    * **修改单钱包最大份数：** 根据需求修改单个钱包预售上限


### **4、预售怎么开始与结束？**

**1）开启预售：** 在`预售控制台`点击**开启预售** ，会进行两次确认。第一次是授权确认，第二次会让你**转入** 足够的代币进入预售合约里

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F7LuTsb4blgGzcO1opGkR%252F7%25E5%25BC%2580%25E5%2590%25AF%25E9%25A2%2584%25E5%2594%25AE.png%3Falt%3Dmedia%26token%3D98f35de2-eec2-4240-9a01-e135ca14e698&width=768&dpr=3&quality=100&sign=23ba5c9c&sv=2)

首先，点击开启预售按钮后，钱包会弹出让你进行授权

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FrPw8M1dwuDKixSgO1VP0%252F8-%25E9%2592%25B1%25E5%258C%2585%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3D53cbccb2-e4ac-4877-b479-396590d959d5&width=768&dpr=3&quality=100&sign=cb719347&sv=2)

确认授权

第一次授权成功后，紧接着会弹出钱包进行第二次确认，并将预售的代币转入预售合约地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FYwFCZ2qMczcoKISfnkUU%252F9-%25E8%25BD%25AC%25E5%2585%25A5%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D8b5b5557-0cdb-4414-8a9f-efa569affeba&width=768&dpr=3&quality=100&sign=a365f7f6&sv=2)

转入代币

第二次确认成功后，会提示你预售开启成功，同时也能看到代币已经转入到合约里面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F8WLAMev46qXYo66QIawa%252F10-%25E9%25A2%2584%25E5%2594%25AE%25E5%25BC%2580%25E5%2590%25AF%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Df93e8286-e08a-4fd0-ad22-115940f85092&width=768&dpr=3&quality=100&sign=244eb707&sv=2)

**3）结束预售：** 如果你想提前结束预售，只需要通过“提取合约内代币”的功能，将合约里面的代币全部提出来，就无法预售了，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FwbEMLbAjkokMLSRTmCNL%252F%25E6%258F%2590%25E5%258F%2596%25E5%2590%2588%25E7%25BA%25A6%25E5%2586%2585%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D1452cfbf-f477-49b7-b2ba-b4278b949433&width=768&dpr=3&quality=100&sign=f8c6745a&sv=2)

## **四、相关问答**

  * check

**为什么开启预售失败？**

    * **钱包里没有足够的代币：** 假设你设置的预售【每份数量x总份数=10000枚代币】，但是你的钱包里只有9000枚代币，那么就会提示预售失败

    * **预售合约没有加白名单：** 如果没有把预售合约地址加入到代币白名单里面，就有可能出现预售开启失败的情况

    * **代币合约有持币限制：** 假如之前的代币合约有最大持仓限制，而你预售的数量超过这个限制，导致代币无法转入到预售地址里，就会造成预售开启失败的情况


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3wgQCJgqnGH5O5VeQozP%252F%25E9%25A2%2584%25E5%2594%25AE%25E5%25BC%2580%25E5%2590%25AF%25E5%25A4%25B1%25E8%25B4%25A5.png%3Falt%3Dmedia%26token%3Db60e1267-6bf1-433e-9efa-66b898c995c0&width=768&dpr=4&quality=100&sign=a8a6170a&sv=2)

  * check

**预售开启成功后，为什么用户转账预售失败？**

    * **价格问题：** 用户转账的BNB数量低于每份价格，就会失败，BNB原路返还

    * **Gas问题：** 如果gas费设置的太低，就有可能会导致预售失败

    * **合约总量问题：** 如果合约地址内已经没有足够的代币用于预售，那用户自然无法参与

    * **份数填写错误：** 单钱包最大份数必须大于或等于单次预售最大份数

    * **达到了预售限制：** 如果达到了单次预售限制或者单钱包预售限制，则无法再购买

    * **预售已完成：** 假设你设置的预售总份数是10份，如果已经达到10份，那就代表着预售已经完成，此时将无法继续预售。如果权限还在，可以通过修改预售份数的方式继续预售。如果权限不在了，那就没办法了

  * check

**可以用wBNB或者USDT预售吗** ？

    * 不支持，目前只支持使用原生代币预售。如BSC链用BNB，Base链用ETH

  * check

**批量预售与实际发放份数问题**

    * **整倍数预售：** 假设1份100个币，每份价格0.03BNB。用户转账0.06BNB，发放200个；用户转账0.09BNB，发放300个币，以此类推

    * **非整倍数预售：** 同样是1份100个币，价格0.03BNB。假设用户转账0.04个BNB，则会发放100个币，并退回多余的0.01BNB。如果用户转账0.05BNB，则会发放100个币+退回0.02BNB。假设用户转账0.07BNB，则会发放200个币+退回0.01BNB。合约会自动按照最大倍数发放，多余退还

  * check

**预售有没有最大/最小限制？**

    * **最小限制：** 单个地址单次预售，这个最小限制就是你设定的最小价格，低于这个价格无法预售。

    * **最大限制：** 单次和单个钱包都分别有最大限制


如有不明白或者不清楚的地方，请加入官方电报群：<https://t.me/PandaTool>
