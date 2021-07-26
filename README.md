# pierced
钉钉内网穿透

TCP 穿透需要在数据库里面执行：
GRANT ALL PRIVILEGES ON *.* TO root@'%' IDENTIFIED BY '123456';
FLUSH PRIVILEGES;
数据库连接命令：
mysql -h vaiwan.com -u root -p -P 1234 //端口号地址

==================================2021-7-23===============================
# 进入可以运行ding.exe文件的目录（windows_64目录）
cd X:xxx/windows_64

# 运行ding.exe文件，参数-subdomain后面的weydo代表 一会儿域名访问的前缀，80代表我要代理的本地端口
ding.exe -config=./ding.cfg -subdomain=weydo 8888

ding.exe -config=./ding.cfg -subdomain=weydoapi 8999

==================================2021-7-23===============================
     Tunnel Status                 online   
	 Version                       1.7/1.7    
	 Forwarding                    http://taxapi.vaiwan.com -> 127.0.0.1:8080  
	 Forwarding                    https://taxapi.vaiwan.com -> 127.0.0.1:8080   
	 Web Interface                 127.0.0.1:4040                                 
	 # Conn                        2                                             
	 Avg Conn Time                 60720.29ms                                                                                                                             