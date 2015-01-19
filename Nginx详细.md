### Nginx架构



### Nginx配置详细



### 配置实例

##### 禁止IP访问


server {  
    listen 80;  
    server_name www.xx.com xx.com;  
    root /html;  
}  

server {  
    listen 80 default_server;  
    server_name _;  
    return 444;  
}  

##### load balance  

http {  
    
    upstream backend {  
        server ip:8080  
        server ip:8081  
    }  
    
    server {  
        ...
        location / {  
            proxy_pass http://backend;  
        }  
    }  
}  
