# 服务器环境搭建
- 系统： ubuntu18.04
 
        root: dh19901.     zephyr: dh1990

- 软件源修改成国内源
    
      1.输入命令修改sources.list文件;
        sudo vim /etc/apt/sources.list
      2.在文件开头加入如下源
        deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
        deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
        deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
        deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
        deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
        deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
        deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse
        deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse
        deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-proposed main restricted universe multiverse
        deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-proposed main restricted universe multiverse
      3.root ssh登陆 sudo vim /etc/ssh/sshd_config
    4.swap [大小修改](https://blog.lovexu.cc/archives/402)

## java

## maven

## gradel 

## redis

安装命令：

`sudo  apt-get install redis-server`

查看tcp 连接

`netstat -ap | grep  6379`

启动：

服务：`redis-server`      

客户端： `redis-cli`

 

修改 配置文件允许局域网内的其他电脑连接redis 
文件位置：`/etc/redis/redis.conf` 如果无法编辑或者无法保存  请先修改权限
## elasticsearch

http://blog.itpub.net/31077337/viewspace-2212771/

## mysql 

`sudo apt-get install mysql-server`
 
`apt-get isntall mysql-client`
 
`sudo apt-get install libmysqlclient-dev`

    1. 给root账户添加密码
       sudo mysqladmin -u root -p password dh1990
    2.添加用户
        
## mongodb

`sudo apt-get install mongodb`
配置文件`/etc/mongodb.conf`

[添加用户和密码登陆](http://www.cnblogs.com/mengyu/p/9071371.html)