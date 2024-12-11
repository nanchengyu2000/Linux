1.输入inconfig 报错:—bash: [ifconfig](https://so.csdn.net/so/search?q=ifconfig&spm=1001.2101.3001.7020): command not found 说明该系统没有这个命令，需安装

2.输入yum install net-tools安装

![](../image/Snipaste_2023-07-14_10-43-52.png)

3.用service network start重启网络

4.再次输入ifconfig就行了