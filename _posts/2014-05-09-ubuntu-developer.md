---
layout: post
title: "Ubantu Developer VM"
date: 2016-08-15
---

Set up a ubuntu for development with windows.
	
## some tips:
1. Launch Terminal by pressing Ctrl+Alt+T
2. sudo gedit /etc/profile
2. alt+F2 run a software

## some service not in develop
1. [Mysql](#Mysql)
2. Hadoop + HBase
3. oracle
4. spark

## some server and lib for debug:
1. play
2. big:::: websphere portal
2. tomcat
2. [apache](#apache)
  -. [php](#php)
  -. markdown


## some develop tool:
1. [git](#git)
2. sublime
2. eclipse
2. big:::  RSA
2. mysql workbench
2. [activator](#activator)

## compile lib:
- [nodejs](#nodejs1)
  - angular
- java
  - scala
- [php](#php)
- phython?
- c#?
- Thomas Jefferson	


## <a name="git"></a>git

### config
```
git config --global user.name "Andy Wang"
git config --global user.email "andywang1908@gmail.com"
[ref](https://www.howtoforge.com/tutorial/install-git-and-github-on-ubuntu-14.04/)

git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080
git config --global http.proxy http://204.40.194.129:3128
#git config --global --unset http.proxy
```

### import reposity
```
cd ~/git
git init andywang1908.github.io
cd andywang1908.github.io
git remote add origin https://github.com/andywang1908/andywang1908.github.io
git pull origin master
```

### export reposity
```
git add *
git commit -am "v1"
git push origin master
```

### clean local change
```
git reset --hard HEAD
git clean -f
git pull
```

### syntax
- [table](https://help.github.com/articles/organizing-information-with-tables/)
- [ref](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code)

### bulid blog with markdown
- [ref](http://jmcglone.com/guides/github-pages/)

## <a name="apache"></a>apache

### install
```
sudo apt-get install apache2
```
- [ref](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04)

## <a name="Mysql"></a>Mysql

### install
```
sudo apt-get install mysql-server
root  Xizang2$A
sudo mysql_secure_installation --close remote connect for safty
```
- [ref](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04)

## <a name="activator"></a>activator

### install
```
download to /home/andy/green/pro/activator/activator-1.3.10-minimal/bin/activator
sudo gedit /etc/profile
add 
PATH=/home/andy/green/pro/activator/activator-1.3.10-minimal/bin:$PATH
export PATH
export JAVA_OPTS="$JAVA_OPTS -Dhttp.proxyHost=204.40.194.129 -Dhttp.proxyPort=3128 -Dhttps.proxyHost=204.40.194.129 -Dhttps.proxyPort=3128 -Dhttp.proxyUser=ebc\wangan1 -Dhttp.proxyPassword=Ontario3$"
to file for path and proxy
run 
. /ect/profile to make effection
```

### usage
```
Create a new project from the command line:
activator new
then 
cd /home/andy/Documents/play2/hello
Run an existing project from its directory:
activator run
Enter the interactive cli (in project directory):
activator
To run the test
activator test
To run the Activator UI
activator ui   and visit http://localhost:8888/home
```

## <a name="nodejs1"></a>nodejs

### proxy
```
npm config set strict-ssl =false
npm config set https-proxy=https://204.40.194.129:3128
npm config set proxy=http://204.40.194.129:3128
#npm config set registry=http://registry.npmjs.org
```

## <a name="php"></a>php

### install
```
sudo apt-get install php libapache2-mod-php php-mcrypt php-mysql
sudo nano /etc/apache2/mods-enabled/dir.conf
sudo systemctl restart apache2
sudo systemctl status apache2

sudo vi /var/www/html/info.php
insert
<?php
phpinfo();
http://your_server_IP_address/info.php 
sudo rm /var/www/html/info.php  after that, romove for safety
```
- [ref](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04)


| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |


In the words of Joseph Campbell:

> [A hero is someone who has given his or her life to something bigger than oneself.](http://www.brainyquote.com/quotes/topics/topic_inspirational2.html)

<img src='/images/2016-08-04-CI.png'/>

try image

![Alt text](https://googledrive.com/host/0B-gKvP-SnWnKQ1d4cE9GSVQ5RWc/image/2016-08-04-CI.png "Optional title")
