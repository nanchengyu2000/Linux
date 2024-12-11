1.先查看是否已安装，命令：rpm -[qa](https://so.csdn.net/so/search?q=qa&spm=1001.2101.3001.7020) | grep vim

发现只装了部分包，缺少安装。

![img](https://img-blog.csdnimg.cn/5df3c59f192543ddae4a26e5a8a4d49d.png)

2.按需下载vim包比如 yum -y install vim-enhanced

差不多就下面这些包了

vim-common-7.4.629-8.el7_9.x86_64
vim-filesystem-7.4.629-8.el7_9.x86_64
vim-X11-7.4.629-8.el7_9.x86_64
vim-minimal-7.4.629-8.el7_9.x86_64
vim-enhanced-7.4.629-8.el7_9.x86_64

 3.也可以直接重新安装

yum -y install vim*
