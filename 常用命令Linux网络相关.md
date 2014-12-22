### 常用命令Linux网络相关


1. sudo ifconfig eth0 down/up  
关闭/开启网卡

2. 安装/卸载软件  
```apt-get install/purge git```

3. 修改主机HOSTNAME  
hostname newname
vim /etc/hostname

4. tar压缩与解压
tar -zcvf dist.tar.gz sourcedir
tar -zxvf dist.tar.gz
