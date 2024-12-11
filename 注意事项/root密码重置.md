平常自己维护的主机，忘记密码的情况比较多，特别是root用户的密码，一般比较复杂，或者因为其他原因，找不到密码，这种情况都会发生，最近在网上看到过帖子，测试可以用，特此分享，仅供大家参考：
![root用户忘记密码的重置方法](F:/360MoveData/Users/zhangyu/Pictures/图片/img)
在虚拟机上做了个RHEL7进行操作，具体操作如下：
第一步：开机后再内核上敲击“e”
![root用户忘记密码的重置方法](F:/360MoveData/Users/zhangyu/Pictures/图片/img)
敲击完“e”出现如下界面，按向下箭头，在linux16这一行的ro改为让rw init=/sysroot/bin/sh
![root用户忘记密码的重置方法](F:/360MoveData/Users/zhangyu/Pictures/图片/img)
![root用户忘记密码的重置方法](F:/360MoveData/Users/zhangyu/Pictures/图片/img)
第二步：并敲击”ctrl+x“进入到系统紧急救援模式（单用户模式启动）
![root用户忘记密码的重置方法](F:/360MoveData/Users/zhangyu/Pictures/图片/img)

第三步：依次输入以下命令：
chroot /sysroot 访问根系统
passwd root  修改root密码（如果不好用，直接输入passwd命令进行修改）
touch /.autorelabel   更新系统信息
exit 退出
reboot 重启

![root用户忘记密码的重置方法](F:/360MoveData/Users/zhangyu/Pictures/图片/img)

至此密码修改完成重启即可登录