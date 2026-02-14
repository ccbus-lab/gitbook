# 波场代币合约验证和开源教程

一篇文章学会在波场链开源

所谓合约验证，就是在波场官方浏览器上将合约源码上传，并与已经发行的代币进行匹配，由此对合约进行开源。开源后的代币，透明性更强，也更容易受到认可。

所有在PandaTool发行的波场TRC20代币，都可以参考这个教程进行开源。


代币验证之前，必须先下载合约文件

file-download

13KB

[Token合约源码.sol](https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FHAYG2qmvFJMeBxv8K4cD%2FToken%E5%90%88%E7%BA%A6%E6%BA%90%E7%A0%81.sol?alt=media&token=a43d4087-aeb6-4da4-b09b-0239fd4fe1d9)

[下载](https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FHAYG2qmvFJMeBxv8K4cD%2FToken%E5%90%88%E7%BA%A6%E6%BA%90%E7%A0%81.sol?alt=media&token=a43d4087-aeb6-4da4-b09b-0239fd4fe1d9)

Token源码

### 一、找到开源入口

首先，我们需要在波场官方浏览器找到开源入口。打开浏览器链接：<https://tronscan.org/> ，什么都别管，先设置语言。

将浏览器拉到底部位置，找到**Preferences** 点击进行偏好设置

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FBmuercHmUdfF5lc3rYIQ%252F%25E8%25AF%25AD%25E8%25A8%2580%25E5%2581%258F%25E5%25A5%25BD%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3Db6e6938b-f177-4f14-84a6-41bee7385c97&width=768&dpr=3&quality=100&sign=7bbe88d3&sv=2)

之后在出现的设置里选择中文，点击Save保存即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEIVQs8xGxfwBFGKovzbu%252F2-%25E8%25AF%25AD%25E8%25A8%2580%25E8%25AE%25BE%25E7%25BD%25AE.png%3Falt%3Dmedia%26token%3D6d50f7dc-3799-42ba-9341-aced19ae3846&width=768&dpr=3&quality=100&sign=88b75f89&sv=2)

当浏览器变为中文后，我们点击右上角连接钱包，登陆上浏览器

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FGRmBaXr9ckBV695MZkxO%252F3-1%2520%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Dc5475917-ae45-4cab-bde8-e2064e92dc02&width=768&dpr=3&quality=100&sign=512061a9&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FtEpT3wNRyFM3VExwTqgo%252F3-2%25E9%2580%2589%25E6%258B%25A9%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Dca715133-b6c3-419d-ac3f-70374890fcce&width=768&dpr=3&quality=100&sign=44c5489f&sv=2)

钱包连接成功后，我们在顶部菜单栏找到【**更多** 】，然后在出现的功能列表里选择【**合约验证** 】，就可以了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FCovDFXXJgsahTskr1X5k%252F3-%25E6%259B%25B4%25E5%25A4%259A.png%3Falt%3Dmedia%26token%3D3f0fae73-cfc4-46f3-96a5-ab2237c0edb5&width=768&dpr=3&quality=100&sign=60b033ee&sv=2)

### 二、填写开源参数并上传源码

在合约开源页面，我们能看到这样的信息

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FZQu9YKGCCDXrmiI4BYb0%252F4-%25E5%2590%2588%25E7%25BA%25A6%25E5%25BC%2580%25E6%25BA%2590%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3D610cf2a9-d878-4869-96d8-9b65d2bd0425&width=768&dpr=3&quality=100&sign=cbe55bc0&sv=2)

如果你觉得懵逼，不要紧，接下来我一 一教大家该怎么填写

  * **合约地址：** 这个很好理解，就是你的代币地址

  * **合约名称：** 这个填 **Token** （注意大小写也不能错）

  * **编译器版本：** 选择tron_v0.8.18


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FpXTe2DUsz4MxGKM8oWoY%252F5-%25E7%25BC%2596%25E8%25AF%2591%25E5%2599%25A8%25E7%2589%2588%25E6%259C%25AC.png%3Falt%3Dmedia%26token%3D585822bb-0879-4899-a6ab-361b34d30847&width=768&dpr=3&quality=100&sign=92a04120&sv=2)

  * **License：** 选择MIT

  * **优化：** Yes

  * **Runs：200**


大家需要注意的是，除了合约地址是你们自己的以外，其他的全部都不能错。例如我填写的信息大概是这样的：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPlkWZ94KQcYyZL8xDslB%252F%25E5%2590%2588%25E7%25BA%25A6%25E9%25AA%258C%25E8%25AF%2581%25E5%258F%2582%25E6%2595%25B0.png%3Falt%3Dmedia%26token%3Df5f20c17-b7ea-4ad3-b8ba-4ef55dbaa782&width=768&dpr=3&quality=100&sign=1f59eb33&sv=2)

参数填写完成之后，就是上传合约文件。我们将刚刚下载的合约文件传上来，如果没有下载，可以点击这里下载

file-download

13KB

[Token合约源码.sol](https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FHAYG2qmvFJMeBxv8K4cD%2FToken%E5%90%88%E7%BA%A6%E6%BA%90%E7%A0%81.sol?alt=media&token=a43d4087-aeb6-4da4-b09b-0239fd4fe1d9)

[下载](https://1885923539-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FnmLBiMxr5iATgeZGW8in%2Fuploads%2FHAYG2qmvFJMeBxv8K4cD%2FToken%E5%90%88%E7%BA%A6%E6%BA%90%E7%A0%81.sol?alt=media&token=a43d4087-aeb6-4da4-b09b-0239fd4fe1d9)

合约文件上传成功，就可以看到源码了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fy827NIxs3LVBNye0L95e%252F%25E7%259C%258B%25E5%2588%25B0%25E6%25BA%2590%25E7%25A0%2581.png%3Falt%3Dmedia%26token%3D66668e04-86ea-4234-80a5-60527c1b494a&width=768&dpr=3&quality=100&sign=156822c5&sv=2)

### 三、验证并发布

文件上传后，将页面往下拉，能发现一个人机验证的提示，点击进行谷歌人机验证

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FbDXVuU21wseFGX4QDag8%252F8-%25E4%25BA%25BA%25E6%259C%25BA%25E9%25AA%258C%25E8%25AF%2581.png%3Falt%3Dmedia%26token%3Df953806b-fe56-43dd-8f27-fadb0c460534&width=768&dpr=3&quality=100&sign=44c34d29&sv=2)

人机验证完成，点击**【验证并发布】**

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FaygpcMnjTGge9ZIwERnA%252F%25E9%25AA%258C%25E8%25AF%2581%25E5%25B9%25B6%25E5%258F%2591%25E5%25B8%2583.png%3Falt%3Dmedia%26token%3D76bae61c-03af-4be1-8b74-6cf7049ecc1a&width=768&dpr=3&quality=100&sign=51d2a1e6&sv=2)

等待几秒钟，如果开源成功，会给你跳转到一个新的页面，可以看到你的合约源码

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fo5whJSMYIzw9eGMh2vwk%252F%25E9%25AA%258C%25E8%25AF%2581%25E5%25BC%2580%25E6%25BA%2590%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D20dc5946-d2c3-4404-a4a4-dc321e0b6fe7&width=768&dpr=3&quality=100&sign=effff6f&sv=2)

如果开源失败，会给出下图的提示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F5T1xp1a9VKApmPPtTSey%252F10-%25E5%25BC%2580%25E6%25BA%2590%25E5%25A4%25B1%25E8%25B4%25A5.png%3Falt%3Dmedia%26token%3Df82367fa-f520-45e0-8822-3618ff6d21c9&width=768&dpr=3&quality=100&sign=93287dab&sv=2)

此时你需要再去检查一下，看看开源参数是不是填写正确了。重新填写之后，再刷新页面重试

### 四、疑问解答

1、合约开源需要付费吗？

  * **答：** 不需要，合约开源不会收取任何费用


2、任何人都能开源吗？

  * **答：** 是的，只要有这套源码且参数填对的话，任何人都能按照这个流程开源


3、为什么我没有看到**人机验证** ？

  * **答：** 谷歌人机验证必须在开启梯子的前提下才会有，请检查网络是否正确


如果您有其他问题，还可以进入Telegram电报群找志愿者解答： <https://t.me/pandatool>
