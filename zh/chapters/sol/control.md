# Solana权限管理(增发、冻结、弃权）

Solana链代币权限管理

## **一、权限解读**

Solana有两种代币标准：SPL Token和SPL Token2022。前一种就是普通的代币，占据市场95%的份额。后一种是基于标准代币推出的高级拓展代币，具有多种功能，用的不多。我们分开解读两种不同代币的权限。

### **1、普通SPL代币权限**

普通的Solana SPL代币创建出来后，会有3个权限：增发权限（铸币权）、拉黑权限（冻结权）、更新资料权限

  * **增发权限：** 可以增发、铸造代币，提高代币供给量

  * **拉黑权限：** 可以冻结任何一个地址，使代币不能转入与转出

  * **更新资料权限：** 可以修改代币名称、logo等


如果是在PandaTool发行的代币，并已上传了logo，会自带这三个权限。如果是其他平台发行的代币，可能会带有2个权限或者1个权限。

当然，不管你是在哪里创建发行的代币，都可以通过PandaTool的工具放弃权限，或者使用拉黑、冻结功能，以实现代币的权限管理。

### **2、Token2022权限**

高级的Token2022代币创建出来后，除了有上述三种权限以外，还有2个权限：**超级管理权限和暂停交易权限**

  * **超级管理：** 可以将持仓地址的代币转走或者销毁

  * **暂停交易：** 暂停全网代币的转账、交易


下面，我们详细看一下这些权限**。**

## **二、放弃权限**

我们提倡大家在发币之后，将权限放弃。打开权限管理页面， <https://solana.ccbus.cc/control> ，然后输入代币的合约地址，可能会给你以下几个提示：

### **1、当前地址无代币权限**

如果你已经丢弃了所有权限，查询代币时会提示你：当前代币已禁止更新资料、当前地址无代币增发权限、当前地址无代币的冻结权限。

出现该情况，说明你的钱包没有该代币的权限，不支持放弃。如果你确认没有放弃权限，那就是你连接的钱包不是发币钱包，可以更换钱包后刷新再试

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLNNjX5zjU35IAbeyApY5%252F%25E6%2597%25A0%25E6%259D%2583%25E9%2599%2590.png%3Falt%3Dmedia%26token%3D83d20ee4-0f9d-4a93-8473-2a130834e8ba&width=768&dpr=3&quality=100&sign=1fa2549d&sv=2)

## 2、没有任何提示

如果点击查询代币，发现没有任何提示，说明你可以正常放弃权限。此时将权限按钮勾选上，然后确认就可以了。需要放弃哪个权限，就勾选哪个。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FmIoEkn6QwhvIKTfyxqtj%252F%25E4%25B8%25A2%25E5%25BC%2583%25E6%259D%2583%25E9%2599%2590.png%3Falt%3Dmedia%26token%3D91b9333e-58e8-4952-9f39-1e2f3c849dba&width=768&dpr=3&quality=100&sign=d51eee09&sv=2)

## **二、普通SPL代币使用权限**

如果你不愿意放弃权限，那就可以使用权限工具，对代币进行增发或者拉黑操作

### **1、增发代币**

很好理解，就是增加代币的总量。我们只需要点击增发按钮，输入增发数量，点击确认即可。

以下面这个代币为了，从浏览器可以看出，该代币的总量是1000

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FAfhWmoxyO0jM0pkRI7H5%252F%25E5%25A2%259E%25E5%258F%2591%25E5%2589%258D.png%3Falt%3Dmedia%26token%3Dc83add81-5dd6-449a-a417-e60038867b42&width=768&dpr=3&quality=100&sign=3200d397&sv=2)

现在我使用增发功能，增发1000个代币，操作如下：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fx3Wc3oy3VguDeeH6joS5%252F%25E5%25A2%259E%25E5%258F%2591%25E6%258C%2589%25E9%2592%25AE.png%3Falt%3Dmedia%26token%3D4164e70e-0c66-42eb-9c85-5a6522508b0d&width=768&dpr=3&quality=100&sign=def17808&sv=2)

点击确认，钱包确认后，会提示你增发成功

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FBfwp6TaL280IxRg2pKII%252F%25E5%25A2%259E%25E5%258F%2591%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Dacc091ee-be5d-467a-af9e-10e210df790d&width=768&dpr=3&quality=100&sign=550adc95&sv=2)

此时我们回到浏览器刷新一下，就可以看到浏览器的代币数量发生了变化，达到了2000枚

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnBlTWiD2ZvhdHsRF3pRf%252F%25E5%25A2%259E%25E5%258F%2591%25E5%2590%258E.png%3Falt%3Dmedia%26token%3Db6cae63a-91cc-463e-a841-012d3b62840b&width=768&dpr=3&quality=100&sign=2f721313&sv=2)

### **2、冻结/解冻账户**

冻结账户也叫拉黑账户，指的是持有该代币的地址被拉黑后，将无法把代币转出，即无法转账及卖出。同时，其他地址也无法向该地址转账。我们建议大家谨慎使用该功能，以确保项目的长久运行。如果冻结之后要解冻，直接点击解冻账户就行了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqgdsgEbE9r37dlQm9Vyt%252F%25E5%25BE%25AE%25E4%25BF%25A1%25E6%2588%25AA%25E5%259B%25BE_20241002140919.png%3Falt%3Dmedia%26token%3Dfe60826a-a1e1-47d9-a047-9c8b56ea8a3d&width=768&dpr=3&quality=100&sign=13512db3&sv=2)

地址被冻结之后，转账出去会提示“无法发送”，这就说明冻结成功了。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPOeW74k5a01ul1ZmU5th%252F%25E6%2597%25A0%25E6%25B3%2595%25E5%258F%2591%25E9%2580%2581.png%3Falt%3Dmedia%26token%3D3a41d993-ce34-488b-8682-42d9481f623a&width=768&dpr=3&quality=100&sign=9d644add&sv=2)

  * 注意，该地址为钱包地址，不是Account地址


## **三、Token2022代币使用权限**

Token2022代币的增发、冻结和更新资料，与普通代币是一样的，就不做过多解释了，主要是看一下高级功能。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FNVnLmFoSc7zomtEGf985%252F2%25E5%2585%25A8%25E5%25B1%2580%25E6%258E%25A7%25E5%2588%25B6%25E4%25B8%258E%25E6%259A%2582%25E5%2581%259C%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3D848f0e51-008d-4384-afbe-c19931fc419e&width=768&dpr=3&quality=100&sign=524ab534&sv=2)

### **1、超级管理权限**

超级管理权限，就是截图中显示的全局管理。您可以通过该权限，对其他钱包地址的代币进行操作：转账与销毁。

**转账代币：** 输入目标钱包地址、代币数量和接收地址，即可将代币转走

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCOEGCPwBuC5HDeAtZH5D%252F3%25E8%25BD%25AC%25E8%25B4%25A6%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D3b6f5123-a7b7-4895-b075-a083f23e15df&width=768&dpr=3&quality=100&sign=f44f0039&sv=2)

**销毁代币：** 输入目标钱包地址和销毁数量，即可将该钱包内相应数量的代币销毁掉

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6oFtkJzetTXs0KvpHrw2%252F4%25E9%2594%2580%25E6%25AF%2581%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D2ae15abf-80ab-41ec-afb9-84113cb58b77&width=768&dpr=3&quality=100&sign=dc6bdd2e&sv=2)

### **2、暂停交易权限**

可以将代币所有的交易与转账全部冻结住，使其无法再进行任何任何操作。这个权限主要用于紧急情况，例如代币被盗等。

**暂停交易：** 点击该按钮，钱包确认好后即可暂停

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fz3jrHxOCpv5UT2hVHu8d%252F5%25E6%259A%2582%25E5%2581%259C%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3Df62402d7-b4bd-4b0a-b00f-c6ce828d6ddd&width=768&dpr=3&quality=100&sign=c684993&sv=2)

**恢复交易：** 交易暂停后，还可以恢复，我们点击`恢复交易`按钮就可以了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbGc7F8WbMKJCvaj3lasR%252F6%25E6%259A%2582%25E5%2581%259C%25E4%25BA%25A4%25E6%2598%2593.png%3Falt%3Dmedia%26token%3Dc0c823f2-3b21-4363-ba11-a710c6a9b3a5&width=768&dpr=3&quality=100&sign=284e8303&sv=2)

至此，关于普通的SPL Token和Token2022的权限管理使用教程，就到这里全部结束了。

如果使用权限的过程有相关问题，欢迎进群询问解答：<https://t.me/pandatool>
