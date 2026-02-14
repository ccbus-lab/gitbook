# 合约开源教程

通过PandaTool, 在`BSC`、`ETH`等基础设施完善的链上发行代币时, 合约会自动开源, 无需进行手动操作.

但是在Core等区块浏览器功能不完善的链上,或者因为一些无法预料的情况 无导致法自动开源时, 就需要用户在创建代币完成后, 进行手动开源

下面以BSC测试链为例, 详细描述开源流程

## 1\. 复制开源参数

在创建代币的确认页面, 将会显示 “开源参数” 选项卡, 点击后可展开信息, 标注了开源时需要用到的各种参数：

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FTFR3lWoHBLVj1Y92cZ9F%252F%25E5%25BC%2580%25E6%25BA%2590%25E5%258F%2582%25E6%2595%25B0.png%3Falt%3Dmedia%26token%3Dfd493f29-c78e-47ed-841a-714b7fd16980&width=768&dpr=3&quality=100&sign=110a0dd6&sv=2)

需要记住开源参数，并将`源代码`和`构造参数`复制到本地

## 2、区块浏览器验证

代币创建完成后, 点击页面中的 `浏览器查看` 按钮, 跳转至 `BSC测试链`的区块浏览器的代币页面。此外，也可以手动进入浏览器中, 在搜索框中搜索生成的代币合约

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252F36zDWPM3DxrDqbMlFyGf%252F%25E5%2590%2588%25E7%25BA%25A6%25E9%25AA%258C%25E8%25AF%2581.png%3Falt%3Dmedia%26token%3D396e6be0-ae58-4811-9696-0f589045f056&width=768&dpr=3&quality=100&sign=495b17f8&sv=2)

找到合约后，点击“Verify and Publish”（验证与发布合约），之后进入下一步

## 3、选择开源信息

根据刚刚创建页面中的合约参数, 选择开源信息

  * `Compiler Type` 选择单一文件 `Single file`

  * 编译器版本选择 `V0.8.24`

  * 开源协议选择 `MIT`


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FstXkTpARvBIt9HvOezzW%252F%25E5%25BC%2580%25E6%25BA%2590%25E5%258F%2582%25E6%2595%25B02.png%3Falt%3Dmedia%26token%3D9c34fdbe-b234-4610-9ebf-5295acce2d36&width=768&dpr=3&quality=100&sign=14e92547&sv=2)

## 4、填写开源资料

点击 `continue` 继续填写详细信息

  * `Optimization` 选择 yes

  * 将第1步中复制的 `源代码` 粘贴在 `Contract Solidity Source Below` 中

  * 将第1步中复制的 `构造参数` 粘贴在 `Constructor Arguments` 中


![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FaMtDAATqkz4WTXuFSeIj%252F%25E5%25BC%2580%25E6%25BA%2590%25E9%25A1%25B5%25E9%259D%25A2.png%3Falt%3Dmedia%26token%3Df2c3450c-9932-42d3-8e85-24ebc57a944a&width=768&dpr=3&quality=100&sign=16f35c7b&sv=2)

## 5、完成开源

进行谷歌人机验证，通过后点击“Verify and Publish”，等待十几秒钟，即可完成开源

![](https://help.pandatool.org/~gitbook/image?url=https%3A%2F%2F1885923539-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FnmLBiMxr5iATgeZGW8in%252Fuploads%252FamL4bx019ohXeZ8CKb2x%252F%25E5%25AE%258C%25E6%2588%2590%25E5%25BC%2580%25E6%25BA%2590.png%3Falt%3Dmedia%26token%3Dc1d6c6ad-9bd8-4aa1-8916-6efe0713d354&width=768&dpr=3&quality=100&sign=6d870650&sv=2)
