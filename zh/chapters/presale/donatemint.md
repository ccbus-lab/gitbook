# 创建代币Mint捐赠预售教程

预售即加池、自动分发LP、人人都是做市商

**什么是Mint捐赠预售？**

简单来说，就是通过Mint的方式预售，并将收到的BNB捐赠给名人钱包。j具体来说，项目方将一定数量的代币打入预售合约地址，开启预售后，用户将BNB转入预售合约地址，预售合约会自动按照设定好的比例，将一部分的代币或者BNB给到名人钱包，如V神钱包地址，方便后续的炒作。

和标准预售、加池预售不同，捐赠预售借助了名人营销的方式，主动的将V神等钱包地址加入到项目中来，给项目打造了新的叙事，便于后续的传播。

### 一、Mint捐赠预售功能说明

  * **捐赠预售：** 预售的同时将BNB或者代币给到名人钱包

  * **无前端：** 不需要任何网页，纯合约支持，100%**去中心化**

  * **转账即预售：** 用户将BNB转到`预售合约`，就能**自动** 获得代币

  * **自定义功能：** 项目方可以在预售开始后通过控制台**修改** 预售价格和每份数量

  * **无软顶/硬顶：** 没有软顶或者硬顶的概念，只有一个预售总数量（份数x每份数量）


### 二、注意事项提前说明

  * V神后期有砸盘的风险，注意防范

  * 标准代币合约**不建议** 开启预售，因为预售期间可能会有人加池

  * 其他代币合约请不要开始交易（如有手动开盘功能的话）


## **三、捐赠预售创建教程**

### **1、连接钱包（老手请忽略）**

首先，我们打开捐赠预售创建官网：<https://ccbus.cc/presales/create> ，右上角点击连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjaYwyhZIo7caum3ByfMp%252F1-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D646f459f-27d6-4b10-84db-cc67eecb11d4&width=768&dpr=4&quality=100&sign=118be3e1&sv=2)

之后会弹出小狐狸让你确定要连接的钱包地址，选择一个就行了。然后下一步就是选择公链，如果您要在币安创建预售，就选择BSC。如果要在Base链创建预售，就选择Base

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fto2I45fnkhnHMnT4mrz6%252F2-%25E9%2580%2589%25E6%258B%25A9%25E5%2585%25AC%25E9%2593%25BE.png%3Falt%3Dmedia%26token%3D5c12898f-492e-4007-94ba-afa9f2fbe4e4&width=768&dpr=4&quality=100&sign=188fa091&sv=2)

之后就能在右上角看到你的钱包地址和链状态，说明已经链接成功了

### 2、填写预售参数

钱包连接成功后，我们通过PandaTool可视化页面创建预售，还是那个页面：<https://ccbus.cc/presales/create> 打开，填写相应的预售参数：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fxlrqv5JVLlWxcP27Tt8g%252F1-%25E6%258D%2590%25E8%25B5%25A0%25E9%25A2%2584%25E5%2594%25AE.png%3Falt%3Dmedia%26token%3D418bf7bd-f60b-4a96-8d35-cf473e6778d7&width=768&dpr=3&quality=100&sign=7bbfcca0&sv=2)

  * check

**预售名称** : 给你的预售起个名字，仅支持英文

  * check

**预售代币地址** : 你要预售的代币合约地址（前提是有代币）

  * check

**每份价格 :** 每份预售的价格，最小的单位是0.001

  * check

**每份数量** : 每份有多少个代币

  * check

**总份数:：** 一共可以预售多少份（每份数量x总份数≤代币发行总量）

  * check

**单次预售最大份数：** 一次最多可以预售几份

  * check

**单钱包预售最大份数：** 一个钱包最多可以预售几份 _（单钱包最大份数必须小于单次预售最大份数）_

  * check

**捐赠BNB/ETH比例：** 将预售的BNB/ETH按照多大的比例（0~100）捐赠给某个地址

  * check

**接收BNB/ETH的地址：** 将BNB/ETH捐赠给哪个地址（一般是名人钱包）

  * check

**捐赠代币的比例：** 将预售的代币按照多大的比例（0~100）捐赠给某个地址

  * check

**接收BNB/ETH的地址：** 将代币捐赠给哪个地址（一般是名人钱包）


V神钱包地址：0xd8da6bf26964af9d7eed9e03e53415d37aa96045

例如我下面填写的内容参数

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FScTs5B4H0KQDWEoWrMuw%252F2-%25E6%258D%2590%25E8%25B5%25A0%25E5%258F%2582%25E6%2595%25B0%25E5%25A1%25AB%25E5%2586%2599.png%3Falt%3Dmedia%26token%3D7408ab7c-f46a-40a6-bfcf-6ef7f9f83275&width=768&dpr=3&quality=100&sign=f456cd3a&sv=2)


根据上面填写的参数，以0.001BNB的价格可以Mint一份，一份的数量是100个代币，其中捐赠比例都是20%。

什么意思呢，就是说：用户每Mint一次，将会有0.0002的BNB和20个代币给到V神钱包。用户自己只能获得80个代币，项目方只能获得0.0008BNB的预售费用。

参数填写完成后，点击创建合约，此时会弹出钱包进行确认，等待几秒，就会提示你预售创建完成

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FNN9Z2c5XGV64ap0avDMh%252F%25E5%2588%259B%25E5%25BB%25BA%25E5%2590%2588%25E7%25BA%25A6.png%3Falt%3Dmedia%26token%3Dc7b2544e-0e22-48ec-8442-b0bf26361f96&width=768&dpr=3&quality=100&sign=e721acac&sv=2)

  * check

**为什么点击创建没有反应？**

    * 有可能是钱包没连上，核查一下钱包连接情况

    * 有可能是代币合约填错了，核查一下合约地址


### 3、预售控制台操作

创建成功后，我们进入到控制台：<https://ccbus.cc/presales/create>，看下该如何操作这个预售

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbAOPoCDogtmeAbrg5Vj6%252F3-%25E6%258E%25A7%25E5%2588%25B6%25E5%258F%25B0.png%3Falt%3Dmedia%26token%3Df248a2e6-6cc8-4120-a841-7a4031b3a739&width=768&dpr=3&quality=100&sign=1c6244ee&sv=2)

  * check

**权限控制**

    * **转让所有权** : 将合约权限转让给其他人（转移权限之前，记得复制`控制台链接`。新的权限地址必须通过控制台链接，才能进入控制台操作）

    * **开启交易：** 点击按钮后，钱包确认后，即可开始预售

    * **提取合约内代币：** 可以将预售合约里面的BNB/ETH和代币提取走

  * check

**参数控制**

    * **修改每份价格 :** 重新修改预售价格，最低0.001

    * **修改每份数量：** 重新修改每份数量

    * **修改总份数：** 根据实际情况重新修改总的预售份数

    * **修改单次Mint最大份数：** 根据需求修改单次预售上限

    * **修改单钱包最大份数：** 根据需求修改单个钱包预售上限

  * check

**捐赠控制**

    * **修改接收BNB/ETH的钱包：** 重新设置接受捐赠的钱包地址

    * **修改捐赠BNB/ETH的比例：** 重新设置捐赠的比例

    * **修改接受代币的钱包：** 重新设置接受捐赠的钱包地址

    * **修改捐赠代币的比例：** 重新设置捐赠的比例


### 4、预售怎么开始与结束？

**1）加白名单：** 预售创建成功后，将预售合约加入到你本身代币合约的税率白名单中，例如

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F64F5oy5Famh7eD3waxFB%252F%25E5%258A%25A0%25E7%2599%25BD%25E5%2590%258D%25E5%258D%2595.png%3Falt%3Dmedia%26token%3Dcb4dfd3a-eb4e-4986-89d5-1a4461d799bf&width=768&dpr=3&quality=100&sign=7b1ba07e&sv=2)

**2）开启预售：** 在`预售控制台`点击**开始交易** ，会进行两次确认。第一次是授权确认，第二次会让你**转入** 足够的代币进入预售合约里

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FvOS5tnaPlCXIvdn0UBqU%252F%25E9%2592%25B1%25E5%258C%2585%25E6%258E%2588%25E6%259D%2583%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D4f897c59-7b49-4ef1-995e-298019437190&width=768&dpr=3&quality=100&sign=60f80742&sv=2)

第一次授权成功后，紧接着会弹出钱包进行第二次确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCmqw3QIWiJjSMyDHXjdx%252F%25E9%2592%25B1%25E5%258C%2585%25E4%25BA%258C%25E6%25AC%25A1%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3D486d003f-343d-48aa-98a7-1f2c4e9c5cfd&width=768&dpr=3&quality=100&sign=13618f45&sv=2)

第二次确认成功后，会提示你预售开启成功，同时也能看到代币已经转入到合约里面

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FxqL5BpGfpoQM1Sl4JGGO%252F%25E9%25A2%2584%25E5%2594%25AE%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3De6cc22d2-723c-43d2-9a95-7657b64ff1e0&width=768&dpr=3&quality=100&sign=d0385b1d&sv=2)

**3）结束预售：** 如果你想提前结束预售，只需要通过“提取合约内代币”的功能，将合约里面的代币全部提出来，就无法预售了，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FwbEMLbAjkokMLSRTmCNL%252F%25E6%258F%2590%25E5%258F%2596%25E5%2590%2588%25E7%25BA%25A6%25E5%2586%2585%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D1452cfbf-f477-49b7-b2ba-b4278b949433&width=768&dpr=3&quality=100&sign=f8c6745a&sv=2)

### **四、相关问答**

  * check

**捐赠的比例范围是多少？**

    * 最少捐赠0%，最大捐赠100%

  * check

**捐赠BNB和捐赠代币有什么区别？**

    * **捐赠BNB/ETH：** 项目方获得的BNB/ETH变少

    * **捐赠代币：** 用户获得的代币变少

  * check

**为什么开启预售失败？**


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F3wgQCJgqnGH5O5VeQozP%252F%25E9%25A2%2584%25E5%2594%25AE%25E5%25BC%2580%25E5%2590%25AF%25E5%25A4%25B1%25E8%25B4%25A5.png%3Falt%3Dmedia%26token%3Db60e1267-6bf1-433e-9efa-66b898c995c0&width=768&dpr=3&quality=100&sign=a8a6170a&sv=2)

  * **钱包里没有足够的代币：** 假设你设置的预售【每份数量x总份数=10000枚代币】，但是你的钱包里只有9000枚代币，那么就会提示预售失败

  * **预售合约没有加白名单：** 如果没有把预售合约地址加入到代币白名单里面，就有可能出现预售开启失败的情况

  * **代币合约有持币限制：** 假如之前的代币合约有最大持仓限制，而你预售的数量超过这个限制，导致代币无法转入到预售地址里，就会造成预售开启失败的情况


  * check

**预售开启成功后，为什么用户转账预售失败？**

    * **价格问题：** 用户转账的BNB数量低于每份价格，就会失败，BNB原路返还

    * **Gas问题：** 如果gas费设置的太低，就有可能会导致预售失败

    * **合约总量问题：** 如果合约地址内已经没有足够的代币用于预售，那用户自然无法参与

    * **份数填写错误：** 单钱包最大份数必须大于或等于单次预售最大份数

    * **代币提前交易导致：** 这种情况一般出现在加池模式下，如果你的代币本身已经有池子在交易了，且具有了价格。如果这个价格与预售价格不符，就会出现预售失败的情况

    * **预售已完成：** 假设你设置的预售总份数是10份，如果已经达到10份，那就代表着预售已经完成，此时将无法继续预售。如果权限还在，可以通过修改预售份数的方式继续预售。如果权限不在了，那就没办法了

  * check

**为什么标准代币不适合做预售？**

    * 因为选择标准代币，用户预售的同时自动加池子就开始交易了，会导致后续预售无法正常进行。

  * check

**可以用wBNB或者USDT预售吗** ？

    * 不支持，目前只支持公链的原生代币进行预售，如BSC链的BNB、Base链的ETH

  * check

**批量预售与实际发放份数问题**

    * **整倍数预售：** 假设1份100个币，每份价格0.03BNB。用户转账0.06BNB，发放200个；用户转账0.09BNB，发放300个币，以此类推

    * **非整倍数预售：** 同样是1份100个币，价格0.03BNB。假设用户转账0.04个BNB，则会发放100个币，并退回多余的0.01BNB。如果用户转账0.05BNB，则会发放100个币+退回0.02BNB。假设用户转账0.07BNB，则会发放200个币+退回0.01BNB。合约会自动按照最大倍数发放，多余退还

  * check

**预售有没有最大/最小限制？**

    * **最小限制：** 单个地址单次预售，这个最小限制就是你设定的最小价格，低于这个价格无法预售。

    * **最大限制：** 单次和单个钱包都分别有最大限制


如有不明白或者不清楚的地方，请加入官方电报群：<https://t.me/PandaTool>
