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

5. CentOS开启端口  
往/etc/sysconfig/iptables中添加以下行，然后重起iptables服务  
-A INPUT -p tcp --dport 80 -j ACCEPT  
-A INPUT -p tcp --dport 8080 -j ACCEPT  
-A INPUT -p tcp --dport 3306 -j ACCEPT 
service iptables restart  

非永久性生效用以下命令：  
iptables -I INPUT -p tcp --dport 80 -j ACCEPT  

6. CentOS设置IP  
在/etc/sysconfig/...下设置IP
在/etc/resolve.conf中设置nameserver 223.5.5.5  


### 常用命令Rpm详解  

－ivh：安装显示安装进度--install--verbose--hash
－Uvh：升级软件包--Update；
－qpl：列出RPM软件包内的文件信息[Query Package list]；
－qpi：列出RPM软件包的描述信息[Query Package install package(s)]；
－qf：查找指定文件属于哪个RPM软件包[Query File]；
－Va：校验所有的RPM软件包，查找丢失的文件[View Lost]；
－e：删除包






