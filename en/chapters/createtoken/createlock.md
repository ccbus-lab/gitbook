# 创建锁池或锁仓教程

在PandaTool创建锁池/锁币的完整教程

## **一、概念解读**

### **1、什么是锁池？什么是锁仓？**

  * **锁仓：** 也叫锁币，就是将自己钱包里面的代币锁在某个地方不能动，以减少市场流通

  * **锁池：** 就是项目方将流动性资金池的凭证代币LP锁在某个地方，从而无法撤池子跑路


### **2、什么是LP代币？**

  * 即流动性资金池 (Liquidity Pool, LP) 代币。当您提供两种代币 (A 和 B) 作为流动性时，您得到是 LP 代币作为收据凭证。有了这个LP，才能撤池子。LP锁住了，池子就撤不了了。


### **3、池子有权限吗？**

  * 池子是没有权限这个概念的，因为资金池是所有人共有的，任何一个添加流动性的人，都拥有相应比例的份额。例如一个池子只有一个人加流动性，那么他就掌握了所有池子。如果一个池子有100人加流动性，那么每个人按照比例掌握相应的份额。


## **二、代币锁仓流程**

1、打开PandaTool连接钱包

2、填写锁仓信息（代币地址、数量等）

3、授权代币

4、确认锁仓

5、查看锁仓信息

好的，接下来我们详细看一下该如何操作

### **1、连接钱包**

首先，我们要打开锁仓页面：<https://www.pandatool.org/#/createLock?lang=zh-CN> ，右上角连接钱包

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fso8KsIXSobk3A07xLIXI%252F1%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3D08e486da-4c18-422c-bac0-c7e3cd8fefef&width=768&dpr=3&quality=100&sign=83071083&sv=2)

连钱包需要注意两点：

  * 1、**钱包插件：** 欧易OKX、小狐狸Metamask、Phantom都可以，但是只能保留一个。其他的钱包插件，最好都关闭掉

  * 2、**钱包地址：** 注意切换到钱包地址和链，如果错误，可能识别不出来


### **2、填写锁仓信息**

连接钱包后，我们需要填写正确的代币信息和锁的信息

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjObjWOmYJXBJiV84iC5Z%252F2%25E9%2594%2581%25E4%25BB%2593%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3Dba1ff8a4-e57b-44d8-b89d-a82bb76eca42&width=768&dpr=3&quality=100&sign=499363b4&sv=2)

  * **锁仓代币地址：** 填写要锁的代币合约地址（如果是填写池子地址，那就是锁池了）

  * **锁仓数量：** 根据查询的代币填写要锁的数量，要锁多少就填多少

  * **解锁日期：** 选择要解锁的日期（到期之前无法提前解锁，时间为您的本地时间）

  * **锁仓标题：** 这个标题随便写一个就是，就是为这个锁起个名字

  * **授权：** 将代币授权给路由合约


锁仓代币地址可以填写池子地址（即：LP代币地址）。如果您填写**池子地址，就是锁池** 。如果您填写**代币地址，就是锁币** 。

例如我填写的内容如下

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FgLyp7qiP4XLcwtWedgmA%252F3%25E5%25A1%25AB%25E5%2586%2599%25E9%2594%2581%25E4%25BB%2593%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3D731ab502-f510-422a-aaf0-ba4ef5a090b1&width=768&dpr=3&quality=100&sign=cf77c3a9&sv=2)


**注意：** 带有最大持仓限制或者修改钱包余额的代币，是不支持锁的

### **3、授权代币**

确定填写的信息无误之后，点击授权，钱包确认后会提示授权成功

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhejxdA2zVcbYUFLkA4oC%252F5%25E6%258E%2588%25E6%259D%2583%25E7%25A1%25AE%25E8%25AE%25A4.png%3Falt%3Dmedia%26token%3Da538eb31-e9b5-4dc3-874f-208f4a959159&width=768&dpr=3&quality=100&sign=63b6f1f4&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEaXi7HjT1TUxQ5tpF6BZ%252F6%25E5%25B7%25B2%25E6%258E%2588%25E6%259D%2583.png%3Falt%3Dmedia%26token%3Dec56c0b8-7094-4191-acdf-6f4166508022&width=768&dpr=3&quality=100&sign=8588a2a2&sv=2)

### **4、立即锁仓**

授权代币后，我们再核对一下填写的日期、数量是否无误。确认无误后，点击‘立即锁仓’的按钮，此时钱包会弹出确认

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEY0n5sLKOxrlSkpQPUpV%252F7%25E7%25AB%258B%25E5%258D%25B3%25E9%2594%2581%25E4%25BB%2593.png%3Falt%3Dmedia%26token%3D73c6577f-aa96-40ce-9af4-e66a1dc5b1ae&width=768&dpr=3&quality=100&sign=177f8393&sv=2)

钱包确认后等待几秒钟，即可完成锁仓

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FiRs4DEbTlb7qLg8odrZJ%252F8%25E9%2594%2581%25E4%25BB%2593%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3Dbad4505e-7090-4c0f-9e64-9f027274995b&width=768&dpr=3&quality=100&sign=517d9bd&sv=2)

### **5、查看锁仓信息**

锁仓之后，我们怎么查看自己的锁仓信息呢？时间到了，我要去哪里解锁呢？为此，PandaTool开发了锁仓控制台，可以让大家查询并解锁。

我们点击进入锁仓控制台：<https://www.pandatool.org/#/lockList?lang=zh-CN> 就能看到所有的锁仓与锁币信息了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FRDuGefsLotmVZFqO4lhV%252F9%25E9%2594%2581%25E4%25BB%2593%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3D75644e4c-7818-498f-b9c1-8a14028c1a4a&width=768&dpr=3&quality=100&sign=69ecf810&sv=2)

时间到了之后，您就可以在这里进行解锁。

如果您想将锁仓时间改成永远，该怎么做呢？正常情况下是不支持修改时间的，但是你也可以点击`**弃权**`按钮，即可变成**永远锁仓** ，那么就永久拿不回来了。 

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FEH3tjkCfv8Y5e6gEoDET%252F10%25E5%25BC%2583%25E6%259D%2583.png%3Falt%3Dmedia%26token%3Df9370d4b-efbb-4387-93da-92b274a430b6&width=768&dpr=3&quality=100&sign=19a455d8&sv=2)

## **三、流动性锁池教程**

锁仓的讲完了，那么锁池该怎么操作呢？锁池有两种方法：

  * **第一种：** 在锁仓页面输入池子地址，将LP代币锁住

  * **第二种：** 通过流动性控制台直接锁池


### **1、第一种锁池：锁仓操作**

这种锁池方法，与锁仓/锁币是大同小异的，我们只需要在代币地址哪里，填入池子地址（也就是LP地址），其他流程一样，即可完成锁池

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FM666Q5UCIW9aCqFnozUH%252F1%25E5%25A1%25AB%25E5%2586%2599%25E6%25B1%25A0%25E5%25AD%2590%25E4%25BF%25A1%25E6%2581%25AF.png%3Falt%3Dmedia%26token%3D992f4ef5-4d19-430b-8018-20cf48631d05&width=768&dpr=3&quality=100&sign=f7148342&sv=2)

可以说，除了填写的地址从代币地址换成资金池地址外，其他都是一模一样的，操作起来很方便。那么，如何获得池子地址呢？可以在[流动性控制台](https://www.pandatool.org/#/LPmanage?lang=zh-CN)查询，并复制→<https://www.pandatool.org/#/LPmanage?lang=zh-CN>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhRKZpB7DG0hZ8Wp5x4r7%252F2%25E5%25A4%258D%25E5%2588%25B6%25E6%25B1%25A0%25E5%25AD%2590%25E5%259C%25B0%25E5%259D%2580.png%3Falt%3Dmedia%26token%3D9cb54526-4617-44b4-8bb4-dc22c5131fb8&width=768&dpr=3&quality=100&sign=3562180d&sv=2)

### **2、第二种锁池：流动性控制台锁**

如果您已经创建了流动性，可以在我们的[流动性控制台](https://www.pandatool.org/#/LPmanage?lang=zh-CN)查询到您的资金池，那么就可以直接点击锁池。我们进入流动性控制台→<https://www.pandatool.org/#/LPmanage?lang=zh-CN>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F93qv7ur6n5xlTqdgSCVM%252F3%25E6%25B5%2581%25E5%258A%25A8%25E6%2580%25A7%25E6%258E%25A7%25E5%2588%25B6%25E5%258F%25B0.png%3Falt%3Dmedia%26token%3D06cbb74a-0792-486e-80cf-46fd6f4c7adb&width=768&dpr=3&quality=100&sign=b21a8d18&sv=2)

点击锁池按钮，然后输入相关的信息

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F1D66h3GEswzG0OIj8Gnt%252F2%25E9%2594%2581%25E6%25B1%25A0%25E8%25AF%25A6%25E6%2583%2585.png%3Falt%3Dmedia%26token%3D5fd0c0a2-a7bf-41f7-9046-c11cafb6798d&width=768&dpr=4&quality=100&sign=971378fc&sv=2)

  * **锁池百分比** ：这个百分比指的是您占有的池子比例的百分比，而非所有流动性的百分比

  * **锁池数量：** 由百分比自动计算出LP的数量

  * **解锁日期：** 根据您当地的时区来设定解锁日期，到期前不可取出LP

  * **锁池标题：** 随便起个名字就行，不是必须要填的

  * **LP代币授权：** 在撤池前需要进行授权


**关于百分比：** 假设池子都是您一个人加的， 那么这个百分比=池子的百分比。如果池子是多个人加的，就需要另外算的。比如，您本身占有池子份额的20%。那么您即便选择100%，整个池子也只是锁了20%的流动性而已。如果您选择20%，那么整个池子也就是锁了4%的流动性。

LP授权之后，点击确认锁池，等待几秒钟，就可以完成了

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FWryatRNMp8JdO9afKzhB%252F3%25E7%25A1%25AE%25E8%25AE%25A4%25E9%2594%2581%25E6%25B1%25A0.png%3Falt%3Dmedia%26token%3D41a5079a-72da-4c97-9928-e1486cd516e9&width=768&dpr=4&quality=100&sign=4362947c&sv=2)

锁池之后，我们去哪里看呢？可以在[锁仓控制台](https://www.pandatool.org/#/lockList?lang=zh-CN)里查询我们的锁信息。进入锁仓控制台 → <https://www.pandatool.org/#/lockList?lang=zh-CN>

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FQtM54U3DdMdOVyZ9vmMf%252F4%25E9%2594%2581%25E4%25BB%2593%25E6%258E%25A7%25E5%2588%25B6%25E5%258F%25B0.png%3Falt%3Dmedia%26token%3D267347e5-4df6-4696-b6bd-00de9a982578&width=768&dpr=4&quality=100&sign=7eec453b&sv=2)

至此，整个锁池与锁仓的教程就到这里了。下面，就一些重点问题做一些解答

## **四、疑问解答**

**1、为什么提示锁仓失败？**

  * 答：首先需要排查，您的代币合约是否有`持仓限制`等功能，这种带限制是没办法锁的。如果确定这个没有问题，请再看一下钱包内的BNB数量是否大于0.01个。余额不足可能导致锁仓失败。


**2、锁仓/锁池需要收费吗？大概多少钱？**

  * 答：是的要收费，在BSC链，每次锁池/锁仓，均需要支付`0.01BNB`的费用


**3、有没有办法可以提前解锁？**

  * 答：没有任何办法，智能合约的运作不以人的意志为转移。一旦锁住，不到时间是`无法解锁`的


**4、这个解锁时间，是什么时区的？**

  * 答：这个时间不用额外设置时区，所有的时间默认是您所在地区的时间


如果您有任何关于锁池或者锁仓的问题，均可以在Telegram群里咨询我们的志愿者：<https://t.me/pandatool>
