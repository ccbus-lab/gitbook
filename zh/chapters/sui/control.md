# Sui代币权限管理教程

管理Sui链代币权限，含增发、更新等

在PandaTool平台创建的Sui链的代币，会有4个权限：增发权限（铸币权）、更新资料权限、冻结权限和全局冻结权限

  * **增发权限：** 可以增发、铸造代币，提高代币供给量

  * **更新资料权限：** 可以修改代币名称、logo等

  * **冻结权限：** 可以冻结任意持币地址，使其无法转账与卖出

  * **全局冻结权限：** 冻结所有地址的代币交易与流通，仅在紧急情况下使用


如果是在PandaTool发行的代币，并已上传了logo，会自带这两个权限。


**增发铸币** 的功能在两个场景下使用：

  * 1、发币的时候没有进行二次确认，导致发币没有完成，此时可以通过铸币来实现代币创建

  * 2、发币的时候代币数量填少了，此时通过铸币功能来增发代币，提高供给


尽管如此，该功能的使用依旧不利于项目的长期良性发展，我们**鼓励大家丢弃权限**

### **一、代币冻结与解冻教程**

**代币冻结，** 指的是权限所有者，可以将持币地址拉黑。被拉黑的地址，将不能转出代币，或者卖出代币。所以，这个也叫黑名单功能。可以冻结，就可以解冻，这是相互的。


该功能的使用，非常不利于项目的长期发展。我们**非常不建议** 大家使用该功能，并因此提高了使用费用，请大家谨慎操作。如无必要，请勿使用该功能

首先，我们打开代币的权限管理页面：<https://sui.ccbus.cc/control> ，右上角连接钱包后，点击`冻结/解冻账户`按钮。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fzs2JIxDAZWB5EZgtgIZQ%252F1%25E5%2586%25BB%25E7%25BB%2593.png%3Falt%3Dmedia%26token%3D1ab02482-e4db-4983-b739-745f83d4ad4a&width=768&dpr=3&quality=100&sign=d70014ac&sv=2)

之后，我们选择代币，从列表中找到您要操作的代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FasGQfgDBX2FN7k4O2Vlc%252F2%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D654c285d-7d63-430b-87e0-aa295314e557&width=768&dpr=3&quality=100&sign=263ac6e5&sv=2)


如果您无法找到要操作的代币，可能有以下几个原因：

1、右上角没有连接钱包

2、代币不是本平台发行的（或者是在8月25日之前发行的）

3、网络问题，可以刷新重试

确定代币后，我们输入某个持仓地址（必须是持有该代币的地址，否则无法操作），点击`冻结账户`按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLd7fiawnpMLPa2InOKCW%252F3%25E5%2586%25BB%25E7%25BB%2593%25E8%25B4%25A6%25E6%2588%25B7.png%3Falt%3Dmedia%26token%3D9eaa6f1f-e09f-4865-a4c7-cdfc017a57f1&width=768&dpr=3&quality=100&sign=76d637f3&sv=2)

然后会跳出钱包，点击确认即可完成冻结操作。被冻结或者说被拉黑的地址，将无法再转出代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FcYEiFJVLWj52ciBhjKnq%252F4%25E5%2586%25BB%25E7%25BB%2593%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D3ac3325a-de86-4984-afbf-8bec55c0bfe1&width=768&dpr=3&quality=100&sign=2db8961&sv=2)

当一个地址被冻结之后，他转账会出现以下提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FIQ2n9ZB78MSHuaKmjaEX%252F5%25E6%2597%25A0%25E6%25B3%2595%25E8%25BD%25AC%25E8%25B4%25A6.png%3Falt%3Dmedia%26token%3D32c493dc-a48c-4873-ac9a-418780ebcc92&width=768&dpr=3&quality=100&sign=c05080bf&sv=2)

如果你想解冻，也非常简单。点击解冻按钮，即可完成

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F043aZmbcyLU9YjWdxl1w%252F6%25E8%25A7%25A3%25E5%2586%25BB.png%3Falt%3Dmedia%26token%3D88763a35-6f96-4f22-8962-3e32443f0bd6&width=768&dpr=3&quality=100&sign=29941565&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FUb0rVQLE6YmEKX7c3Ifp%252F6-2%25E8%25A7%25A3%25E5%2586%25BB%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Dda4acc30-a931-4f3b-b7e8-774b9431119c&width=768&dpr=3&quality=100&sign=80b597c4&sv=2)

### **二、全局冻结教程**

所谓全局冻结，指的是该代币所有钱包地址都将无法转账、交易，全网代币**均被冻结** ，无法进行任何交易。该功能只在紧急情况下使用，如被黑客攻击、价格异常波动等等。

想要开启全局冻结也很简单，我们只需要点击`全局冻结`按钮，即可完成。如果问题已经解决，我们再点击解冻，即可解除冻结状态。

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F4pgaiXLTsgftdCDuu3J0%252F7%25E5%2585%25A8%25E5%25B1%2580.png%3Falt%3Dmedia%26token%3D83e756cf-a6c7-4a3e-a275-3858ac3f6227&width=768&dpr=3&quality=100&sign=f6afb0e5&sv=2)

### **三、增发铸币教程**

具体该怎么使用呢？首先，我们打开控制台链接：<https://sui.ccbus.cc/control> ，右上角连接钱包（这一步之大家应该很熟悉了），连接成功后右上角能看到钱包地址

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F78SFZZhKuiQMWCeeMSbj%252F1.png%3Falt%3Dmedia%26token%3D1fe14639-36d6-4ce1-b7ea-92d8b5dee609&width=768&dpr=3&quality=100&sign=72aae677&sv=2)

确认钱包已经连接

钱包连接完成后，我们开始选择代币，此时平台会列出所有你有权限可以管理的代币，我们选择要增发的代币，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FR11uez28aM1P6UFz24I8%252F2.png%3Falt%3Dmedia%26token%3D281804f9-4e62-42da-97ac-e08a3f201726&width=768&dpr=3&quality=100&sign=75a3f574&sv=2)

选择代币

然后输入要增发的数量，点击确认即可，比如我选择增发1个亿，就按照下图进行操作

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fh59X51OFLwkbBxGIAbjL%252F3.png%3Falt%3Dmedia%26token%3Db7212c31-b11a-4033-a9c1-0442ee49f76e&width=768&dpr=3&quality=100&sign=fb31c618&sv=2)

之后钱包确认，即可完成

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fml7qUm91beFtkYtJ7xYb%252F4.png%3Falt%3Dmedia%26token%3D88530f7c-6399-4e99-b5de-5e5c9f8af126&width=768&dpr=3&quality=100&sign=aa4170fb&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVlfObcBKLVreQyRPUJUt%252F4-2.png%3Falt%3Dmedia%26token%3D3fc48985-6e82-4c26-85a1-e112799b43ee&width=768&dpr=3&quality=100&sign=fb1d64dd&sv=2)

增发成功

怎么确认自己已经完成增发？可以通过钱包的数量来确认，如下图所示的对比。增发前Panda币是100亿，增发后是101亿，这多出来的1亿就是增发来的

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F5uYccuoSQsEMcADPK9Wx%252F5-1.png%3Falt%3Dmedia%26token%3D4255c6bf-87cd-4505-90f5-ab3ca3577326&width=768&dpr=3&quality=100&sign=162b83d4&sv=2)

### **四、代币资料更新教程**

**更新资料** 指的是代币创建成功后，将代币的名称、头像等进行修改更新


该功能的使用，非常不利于项目的长期发展。我们**非常不建议** 大家使用该功能，并因此提高了使用费用，请大家谨慎操作。如无必要，请勿使用该功能

和增发一样，我们打开PandaTool的代币控制页面：<https://sui.ccbus.cc/control> ，首先要连接钱包（这一步就不演示了），然后点击**更新资料** 按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FHqx88OoARMXnvO3o4GO0%252F1-%25E6%259B%25B4%25E6%2596%25B0%25E8%25B5%2584%25E6%2596%2599.png%3Falt%3Dmedia%26token%3D6176c6e8-67cd-4792-a2d9-fc4feab8ddf1&width=768&dpr=3&quality=100&sign=1434f0b2&sv=2)

在更新资料的操作页面，我们需要按照以下方式填写操作相关内容

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FdlSK3HQnxn0xa3BBFV4x%252F2-%25E6%259B%25B4%25E6%2596%25B0%25E8%25B5%2584%25E6%2596%2599%25E5%2586%2585%25E5%25AE%25B9.png%3Falt%3Dmedia%26token%3D4142feca-4023-42dc-951b-2b5fbd4945ad&width=768&dpr=3&quality=100&sign=dabf6468&sv=2)

  * **选择代币：** 只能选择自己有权限的代币进行更新

  * **代币全称：** 不能是中文或符号，不能超过**32** 个字符

  * **代币简称：** 不能是中文或符号，控制在**2~8** 个字符

  * **Logo：** 尺寸小于100k，建议是1:1比例

  * **简介：** 不能带中文或符号，不能超过**320** 个字符


例如我要将之前发行的Panda代币，修改为SuiPanda代币，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F9X4A3PSmCTIEn2wppscH%252F3-%25E6%259B%25B4%25E6%2596%25B0.png%3Falt%3Dmedia%26token%3Dabd20d08-fa72-4458-a9ed-dfd8c3e98b64&width=768&dpr=3&quality=100&sign=4bb0663e&sv=2)

更新资料

确认信息无误后，点击确认，钱包支付费用就可以了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FxEwqkEwy2YTLMgttSFOp%252F6-%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3Deb5a9d49-834e-492f-9f10-473cd1aa903b&width=768&dpr=3&quality=100&sign=6a33c94d&sv=2)

钱包确认

等待半小时后，我们验证一下是否更新成功，首先是钱包里的logo已经发生变化（Suiet钱包更新比较慢，SuiWallet更新较快）

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FN2Xqk2uhdcbAKClnJtm8%252F4.png%3Falt%3Dmedia%26token%3D892d0141-2a32-419b-8a7e-3badab2d6206&width=768&dpr=3&quality=100&sign=58e5d45f&sv=2)

整个更新流程到这里就结束了，接下来解答一些问题

### **五、放弃权限教程**

权限放弃是非常简单的，我们只需要在点击放弃权限按钮，并选择要放弃的权限（增发权限与冻结权限要分别丢弃），钱包确认，即可完成

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FoZmCaIuqUbQAvo7ZUG74%252F8%25E6%2594%25BE%25E5%25BC%2583%25E6%259D%2583%25E9%2599%2590.png%3Falt%3Dmedia%26token%3D9705d01b-06d4-43d8-8a6d-72c790d3776e&width=768&dpr=3&quality=100&sign=b13279ca&sv=2)

放弃权限之后，该代币在各大平台的检测都非常完美，可以让投资者放心。我们强烈建议大家使用该功能。

### **六、疑问解答**

**1、为什么我更新成功了，但是钱包logo没变？**

  * 答：不同钱包更新的有快有慢，像SuiWallet几分钟就会更新，Suiet要半小时以上。如果几个小时仍然没有更新，那可能是缓存问题，记得关闭钱包再重新打开试一下


**2、为什么有的代币会增发失败？**

  * 答：这可能与代币精度有关系。如果代币精度为9 ，那么该代币的总量上线就是100亿左右。超过这个上线，就无法再继续增发了


**3、增发代币以及更新资料是否需要额外收费？**

  * 答：是的，每次增发铸币，PandaTool平台会收取1 SUI的费用。每次更新资料，会收取5SUI的费用。


**4、冻结与全局冻结需要收费吗？**

  * 答：是的，冻结（或解冻）一次会收取3SUI的费用。全局冻结（全局解冻）会收取5SUI的费用。


**5、为什么查不到我的代币？**

  * 答：如果您无法找到要操作的代币，可能有以下几个原因：

  *  _右上角没有连接钱包_

  *  _代币不是本平台发行的（或者是在8月25日之前发行的）_

  *  _网络问题，可以刷新重试_


**6、放弃权限需要收费吗？**

  * 答：不需要，放弃权限是完全免费的，无需任何费用


**7、使用该增发或者冻结功能会产生哪些危害？**

  * **答：** 恶意使用增发权限与冻结权限，会损害项目的长期发展。事实上，我们不建议使用该功能


如果使用权限的过程有相关问题，欢迎进群询问解答：<https://t.me/pandatool>
