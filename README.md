ZH-Ch Only ADB Toolkit Repo

# Android-Debug-Bridge-Toolkit

5/30下午发布最后一个bat版的ADB Toolkit

以后这个repo都不会再更新

另外我会在这两天内做出Toolkit的生成器

只需要简单配置一些信息 即可直接安装 这可以取代现在的东西

等到一段时间后 会有使用Visual Studio编写的C# ADB Toolkit Repo新增

功能和开放性会比这个bat版本的repo更加强大 但 如果我真的能做到的话...

下载时无需进入Release进行下载 那是一些很多问题的版本了 过一段时间会全部删掉(不包含运行库)

所以要想下载的话直接Download Zip即可 但前提是运行库那些都搞好了 不然就真的是个UI程序了（）

该项目使用全中文(除日志记录外)作为原生语言  该工具包含的内容实在是太多了 ~~而且我英语很渣~~

所以看不懂中文的人很可能要配合*翻译*来使用这个工具。~~虽说很困难~~(所以可能在某一天单独出一个En的repo 如果我真的有时间的话)

使用这个工具需要使用一些运行库`ADB(Included adb.exe&fastboot)&ADB Interface`

都不能缺少安装 少了一样都不能正常使用~~(也许只是不能完全使用而已)~~

我收集而来的这些运行库 装起来是没有问题的

为了方便大家下载 已released一个叫做The Runtime的版本放在最下面

还能怎么调教看各位Developer的本事了

新版中加入了日志记录功能 如果在运行时出现了sm问题

可以通过查找 对应出错时间 将过程或那一段的内容发给我

或许我能解决~~(也说不定)~~

~~还有各位记得清理log 这东西放久了我都打不开~~



### ADB&Fastboot配置方法

右键此电脑 单击属性 

→高级系统设置(如果有开了UAC的记得允许权限)

下方有个环境变量 单击

上面的是用户 下方的是系统 只需要用户变量即可

点击新建 变量名填 adb 值就是文件位置(就是adb.exe的程序位置)

确定 确定 然后退出

win+r 输入 %adb% 查看是否会出现一大串信息

有即代表配置完成

(想配置fastboot 新建fastboot变量名 后面位置即可 还是以上面的操作进行)

* 设置fastboot.exe为环境变量与设置adb.exe为环境变量相同

  

### ADB Interface配置方法

右键此电脑 单击管理 转到设备管理器

在其他设备里找到出错的ADB Interface

双击它 点击下方的更新驱动程序

到了搜索驱动程序软件时 单击 浏览计算机以查找驱动程序软件

单击 从计算机的设备驱动程序列表中选择

点击下一步 再从磁盘安装

单击浏览 找到adb interface的文件夹目录 然后双击 android_winusb.inf 文件

之后下一步 如有提示windows无法验证不兼容也不要在意 是即可

等待安装 完成后会提示 Windows已经成功地更新驱动程序文件

安装即完成



## 使用的一些文章链接(Thanks)

<u>*https://blog.csdn.net/sinat_27672523/article/details/88748398*</u>

<u>*https://blog.csdn.net/qq_36327203/article/details/79469576*</u>

<u>*https://blog.csdn.net/riyuexingchen1204/article/details/84594061</u>*

## 问题

工具内文字全乱码(找到该出错的bat 编辑 另存为编码ANSI 即可解决)

~~静默批量安装应用并不是那么稳定~~

## 修改时间

-Lastest Edited 2020/6/12 21:47

Archive Now
