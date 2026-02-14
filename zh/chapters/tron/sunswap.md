# SunSwap做流动性资金池子教程

一篇文章学会在SunSwap创建流动性资金池

SunSswap是波场TRON链最大的DEX，好像也是唯一一个？集波场TRON链上通证交换、流动性挖矿、稳定币兑换质押及平台自治功能于一体。基本上所有的TRC20代币要做池子，都需要在SunSwap创建流动性。SunSswap以前叫JustSwap，后面被SUN收购了才改成现在的名字。


SunSwap唯一官网：[https://sunswap.com/#](https://sunswap.com/#/home)

今天这个教程，主要是教大家使用电脑在SunSwap上面创建流动性资金池，也就是俗称的加池子。

### 一、找到SunSwap平台

首先，我们打开SunSwap的官网：[https://sunswap.com/#](https://sunswap.com/#/home) ，然后点击页面**左下角** 位置，先将语言设置为中文

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fjh35CKlmaRjsR7tEkXuF%252F1-%25E8%25AE%25BE%25E7%25BD%25AE%25E8%25AF%25AD%25E8%25A8%2580.png%3Falt%3Dmedia%26token%3D4d25a24c-eae2-44e2-85a6-c6af468cda2c&width=768&dpr=3&quality=100&sign=d6c80fb0&sv=2)

之后，我们点击左上方的连接钱包按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FjTQDdCzqcWXgHHBmB24J%252F2-%25E8%25BF%259E%25E6%258E%25A5%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Daafab43f-0b25-44e3-b309-2b80b5fc1803&width=768&dpr=3&quality=100&sign=784fb972&sv=2)

会出现不同的钱包让你选择，我们默认选择TronLink波宝钱包。如果您还没有下载安装钱包插件，可参考 → [波宝钱包TronLink安装教程](/tron/tronlink)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FLBM25nuN5TfcgbLyr65N%252F3-%25E9%2580%2589%25E6%258B%25A9%25E9%2592%25B1%25E5%258C%2585.png%3Falt%3Dmedia%26token%3Df246898b-701a-457d-b642-d7d8181a9b17&width=768&dpr=3&quality=100&sign=c61741bf&sv=2)

假设我们点击TronLInk，会弹出钱包让你选择确认。你需要勾选要连接的钱包地址，然后点击**连接** 即可

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FhnRwGmBdAAJ7nsiUuWA2%252F4-%25E7%2582%25B9%25E5%2587%25BB%25E8%25BF%259E%25E6%258E%25A5.png%3Falt%3Dmedia%26token%3D0a0dfc4f-83fd-4ebe-b9c8-c81fda4deb60&width=768&dpr=3&quality=100&sign=cbfa607d&sv=2)

连接成功后，我们可以在左上角看到自己的钱包地址和余额

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FnobqCZi3uhtDfnszfrg8%252F5-%25E8%25BF%259E%25E6%258E%25A5%25E6%2588%2590%25E5%258A%259F.png%3Falt%3Dmedia%26token%3D261bdb1e-b6b1-430f-87e3-2dfd465adadc&width=768&dpr=3&quality=100&sign=3a8ea0af&sv=2)

这些准备工作完成后，我们就进行加池工作

### 二、SunSwap添加流动性

在创建流动性资金池之前，我们需要选择版本号。一般来说，SunSwap默认的是V2，我们也建议大家选择V3。因为V1只支持TRX交易对、V3的话池子过于复杂，V2是使用最多、相对最简单的池子。

在V2版本的基础上，我们点击主页面的**资金池** 按钮

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FiKyTG26aKLDl9kxBJGWx%252F6-%25E8%25B5%2584%25E9%2587%2591%25E6%25B1%25A0%25E4%25B8%258E%25E7%2589%2588%25E6%259C%25AC%25E5%258F%25B7.png%3Falt%3Dmedia%26token%3D4604972c-4844-40d3-a876-e1c064f2353b&width=768&dpr=3&quality=100&sign=cb969e45&sv=2)

然后选择要创建的交易对。上面那里选择USDT或者TRX，下面就选择您要做池子的代币

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FPtauA4if4xKeriFoIsEp%252F7-%25E9%2580%2589%25E6%258B%25A9%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3Debc970d8-865d-48d5-ba40-acb8179cb428&width=768&dpr=3&quality=100&sign=bf7560ca&sv=2)

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252Fr7axYV95J7kjQ3FpJSSH%252F7-1%25E6%259F%25A5%25E8%25AF%25A2%25E4%25BB%25A3%25E5%25B8%2581.png%3Falt%3Dmedia%26token%3D512a7bad-39eb-4f93-95e3-7a3220f923aa&width=768&dpr=3&quality=100&sign=83b959f8&sv=2)

代币交易对确认之后，再分别输入要添加的代币数量，设置初始价格

> 代币初始价格怎么计算？如果TRX与代币的数量比例是1:1，那么代币的初始上线价格就是1TRX，即：0.15U

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FgIQaHOD0FiTsRjQBJoRJ%252F8-%25E7%25A1%25AE%25E8%25AE%25A4%25E4%25BB%25A3%25E5%25B8%2581%25E6%2595%25B0%25E9%2587%258F.png%3Falt%3Dmedia%26token%3D55ba8a1e-de82-427a-ac26-c04119fc132f&width=768&dpr=3&quality=100&sign=ceba3858&sv=2)

确认数量无误之后，点击提供按钮，钱包确认就可以了。


注意：加池子可能需要消耗大量的能量或TRX，建议预留最少1000TRX在钱包里，以防止加池失败。即便加池失败，也会扣除TRX，所以请谨慎操作

如果您还有其他问题，可以加入PandaTool一键发币群询问，志愿者会给你一些解答：<https://t.me/PandaTool>
