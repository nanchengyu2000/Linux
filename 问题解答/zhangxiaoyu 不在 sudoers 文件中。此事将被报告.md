**通用解释：**[sudo命令](https://so.csdn.net/so/search?q=sudo命令&spm=1001.2101.3001.7020)可以让你以root身份执行命令，来完成一些我们这个账号完成不了的任务。但是并非所有用户都能够执行sudo，因为有权限的用户都在/etc/sudoers中。

解决方法如下：

**1、进入root模式，su，再输入正确密码   （输入su root也是可以的）**

**2、通过cd /etc 进入etc文件中**

**3、查看root对文件是否有读写权限（ll 文件名），没有使用chmod  u+rw 文件名来增加权限**

**4、通过vim或者vi打开sudoers并编辑**

![](../image/Snipaste_2023-07-14_15-26-17.png)

保存退出即可

**5、接下来就可以使用sodu权限进行操作了**