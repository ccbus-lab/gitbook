# Solana租金回收教程

快速回收钱包内的代币租金

## 什么是租金？

想象一下你租了一个仓库存放货物。仓库管理员（区块链网络）需要定期收租金，否则就会清空你的货物腾出空间。**Solana的租金机制正是这样的“仓库管理规则”。**

根据存储的内容和大小不同，租金也有所不同。在正常的Solana区块链里，我们接触到的主要是0.002的租金。即：钱包地址内每存储一个代币，需要收取0.002Sol的租金。

你可以将这个费用理解为Solana链的“数字快递柜押金”！

  * **每个代币都是独立包裹** ：就像快递需要单独柜格存放，每个代币在Solana上必须有独立账户

  * ​**押金防滥用** ：0.002 SOL相当于租用柜格的押金，防止有人乱占空间

  * ​**所有权仍归你** ：就像快递柜押金可退还，这个费用后续能通过PandaTool回收


## Solana租金回收流程回收

### 1、单钱包租金回收

1.打开PandaTool回收工具

2.连接钱包并查询账户

3.选择回收的账户类型或账户代币

4.确认回收

### 2、多钱包租金回收

1.打开PandaTool回收工具

2.导入钱包私钥

3.选择回收空账户或全部账户

4.确认回收


回收租金意味着销毁账户内的所有代币，请谨慎选择代币账户。一旦确认，将无法找回

## 如何回收租金

正如上面所说，您可以通过PandaTool回收您的代币租金。假设您的钱包内有10种代币，而这些代币都不再使用了，那么就可以回收：10x0.002=0.02sol的金额。如果代币超过100个，那这将是一笔不少的费用。因此，回收租金是非常有必要的。

接下来，我将给详细说明租金回收的流程

### 1、找到回收租金工具

我们可以通过PandaTool导航栏找到租金回收工具，也可以直接通过链接进去：<https://solana.pandatool.org/zh/rent>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FVbWDEpYbZ89pwJ4cGt06%252F1.%25E6%2589%25BE%25E5%2588%25B0%25E5%25B7%25A5%25E5%2585%25B7.png%3Falt%3Dmedia%26token%3D2a34e066-b3e4-4414-bb5b-c898a04aae76&width=768&dpr=3&quality=100&sign=ded5bcb4&sv=2)

### 2、连接钱包并查询

之后，我们点击右上角连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FMjFuoeocQIBIsCRlQvfS%252F2.%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D7876dcd3-c5c3-4614-ba8b-f2e6a29cf8a5&width=768&dpr=3&quality=100&sign=26a73c24&sv=2)

钱包连接成功后，点击查询按钮，可以知道自己的钱包内的代币账户情况

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FvB35DKV76BVgP3BghuXf%252F3.%25E6%259F%25A5%25E8%25AF%25A2%25E8%25B4%25A6%25E6%2588%25B7.png%3Falt%3Dmedia%26token%3Da150b0bb-aa7d-47b6-8872-dc5e68b5083f&width=768&dpr=3&quality=100&sign=6bcf0bab&sv=2)

### 3.选择回收类型

查询之后，会发现钱包内有不同类型的代币。您可以根据类型进行租金回收

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FD3hhHRpbOQeUk8D8sZJN%252F4.%25E9%2580%2589%25E6%258B%25A9%25E5%259B%259E%25E6%2594%25B6.png%3Falt%3Dmedia%26token%3Dc01ae366-89ec-4189-a9d8-aa89473535a1&width=768&dpr=3&quality=100&sign=49215574&sv=2)

  * **空账户：** 没有任何代币余额，可放心回收

  * **代币：** 账户内仍然有余额，需谨慎回收（可选择没有任何价值的代币）

  * **NFT：** 谨慎回收（可选择没有任何价值的NFT）


假设您已经确认不再需要该钱包了，就可以点击“全选”，如下图所示

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FsbeWZ5MPaUqP2pxnz2a3%252F5.%25E5%2585%25A8%25E9%2580%2589.png%3Falt%3Dmedia%26token%3D70c07d2a-ba06-46bb-93ca-b6e3c489e0bd&width=768&dpr=3&quality=100&sign=d27adc40&sv=2)

### 4.确认回收

选择好要回收的账户类型后，点击“确认回收”按钮，此时会弹出钱包进行确认，钱包确认后等待几秒钟，即可完成租金回收的工作

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FKP02dyztKhYLSYfU5MtY%252F7.%25E9%2592%25B1%25E5%258C%2585%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3Dfe7ce035-3c1a-4b35-97d8-a2ac91d01c49&width=768&dpr=3&quality=100&sign=e85fd66f&sv=2)

## 批量回收租金

前面的教程，是针对单个钱包进行租金回收的。假设我们有很多钱包都需要回收租金，该怎么办呢？可以使用批量租金回收工具来完成


注意：批量回收租金之前，仍然需要先连接钱包，以支付Gas费

### 1、打开批量租金回收工具

在租金回收的工具页面，找到批量回收工具

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F41eAsYpyKAfZaejwHQXP%252F8.%25E6%2589%25B9%25E9%2587%258F%25E5%259B%259E%25E6%2594%25B6.png%3Falt%3Dmedia%26token%3Dda27bb9d-2e97-4616-80f8-6e8c94041bf5&width=768&dpr=3&quality=100&sign=ac9398a5&sv=2)

### 2、导入钱包私钥

将要回收租金的钱包私钥导入，您需要回收几个钱包，就导入几个钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FIvVCNqa6i2dRUDYGcEWl%252F9.%25E5%25AF%25BC%25E5%2585%25A5%25E7%25A7%2581%25E9%2592%25A5.png%3Falt%3Dmedia%26token%3Ded2e581b-7761-4a7b-b43d-f0f3d1981189&width=768&dpr=3&quality=100&sign=7e2eddc9&sv=2)

### 3.选择账户类型

成功导入钱包后，可以看到钱包内的账户类型。我们需要选择回收全部账户，还是回收空账户

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F6nO0HfEV148Vwlkgm8y3%252F10.%25E9%2580%2589%25E6%258B%25A9%25E8%25B4%25A6%25E6%2588%25B7.png%3Falt%3Dmedia%26token%3D18b07d32-e086-4b58-9123-cba353bf3357&width=768&dpr=3&quality=100&sign=1fd7fbf7&sv=2)

### 4.确认回收

选择好之后，我们点击“确认回收”按钮，弹出钱包确认即可完成

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FqGmIrVoUk4iQ5N6vz9w6%252F11.%25E7%25A1%25AE%25E8%25AE%25A4%25E5%259B%259E%25E6%2594%25B6.png%3Falt%3Dmedia%26token%3D7695e2a7-877d-4d94-93ab-979d6ebd6339&width=768&dpr=3&quality=100&sign=3eb6e2c&sv=2)

## 租金回收疑问解答

**1、租金回收后还能找回代币吗？**

  * 答：回收租金是不可逆操作，会将代币全部销毁，且永远无法找回，请谨慎操作


**2、租金回收需要手续费吗？**

  * 答：PandaTool平台收取4.88%的服务费。假设您应该回收了0.1sol，我们会收取0.00488sol的服务费


**3、如何知道自己会获得多少Sol？**

  * 答：当您选择好要回收的账户后，PandaTool会显示出您可以获得的Sol数量。每个代币账户可以回收约0.002sol的费用


**4、为什么我已经导入了私钥，仍然提醒我连接钱包？**

  * 答：因为租金回收的gas费，需要由连接的钱包收取，且回收的租金会给到连接的钱包地址。这样可以保证，一个地址内没有任何sol作为gas费的情况下，也能进行租金回收


如您针对租金回收问题，还有不明白或者不清楚的地方，请加入官方电报群：<https://t.me/PandaTool>
