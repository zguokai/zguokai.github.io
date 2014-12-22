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


