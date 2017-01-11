---
layout: post
title: "Ubantu Developer VM"
date: 2016-08-15
---

Set up a ubuntu for development with windows.
	
## some tips:
1. Launch Terminal by pressing Ctrl+Alt+T
2. sudo gedit /etc/profile
2. alt+F2 run a software.

## some servise for server
1. [Mysql](#Mysql)
2. Hadoop + HBase
2. oracle
2. spark

## some servise for debug and server
1. play
2. big:::: websphere portal
2. tomcat
2. [apache](#apache)
  - [php](#php)
  - markdown

## some lib for debug and server
- [nodejs](#nodejs1)
  - angular
- java
  - scala
- [php](#php)
- phython?
- c#?

## some develop tool:
1. [git](#git)
2. [svn](#svn)
2. sublime
2. eclipse
2. big:::  RSA
2. mysql workbench
2. [activator](#activator)
2. [proxy](#proxy)

## <a name="git"></a>git

### config
```
git config --global user.name "Andy Wang"
git config --global user.email "andywang1908@gmail.com"
[ref](https://www.howtoforge.com/tutorial/install-git-and-github-on-ubuntu-14.04/)

git config --global http.proxy http://ebc%5Cwangan1:Ontario2%24@204.40.194.129:3128
git config --global http.proxy http://204.40.194.129:3128
#git config --global --unset http.proxy
```

### import reposity
```
cd ~/git
git init andywang1908.github.io
cd andywang1908.github.io
git remote add origin https://github.com/andywang1908/andywang1908.github.io
#use ssh keys
#git remote set-url origin git@gist.github.com:andywang1908/andywang1908.github.io
git pull origin master
```

[R1](https://help.github.com/articles/generating-an-ssh-key/)

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

## <a name="svn"></a>svn

### for java
```
data: https://gscbiqdcapmdw01.cihs.ad.gov.on.ca:8443/svn/SOIT_S2I_Automation
sudo apt-get install libsvn-java
sudo find / -name libsvnjavahl-1.so  get /usr/lib/x86_64-linux-gnu/jni/libsvnjavahl-1.so
next step may skip
Although the library is installed, you still have to tell Java (when used for Eclipse) where to find it. The JVM on Linux does not look in a lot of the standard locations to find the libraries. (This could obviously change in the future.) For example, 32-bit Debian/Ubuntu uses a standard location of /usr/lib/jni for libraries to be used from Java. However, the Oracle JVM does not currently look in this location. The easiest way to tell Java where to find the JavaHL library is to specify the following when starting the JVM:
-Djava.library.path=</path/to/library>
```

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

### global command
```
sudo npm install less -g
sudo npm install http-server -g
```

## <a name="proxy"></a>proxy & ubuntu apt

### ontario
```
DBEEDD eye protect color
http://proxy2.gonet.gov.on.ca:9001/proxy.pac         to  firefox
204.40.194.129:3128

sudo gedit /etc/apt/apt.conf
sudo vi /etc/apt/apt.conf
Acquire::http::Proxy "http://204.40.194.129:3128";
Acquire::http::Proxy "http://ebc\wangan1:Ontario2$@204.40.194.129:3128";
#Acquire::https::Proxy "http://204.40.194.129:3128";
sudo apt-get update      !!!!!!!!!!!!!!!!!!

list:
firefox    chrome       ::::network setting
npm   
apt
sublime
svn
```

## <a name="ssh"></a>ssh

### install
```
sudo apt install openssh-server          connect with putty
#sudo apt install vsftpd         https://help.ubuntu.com/lts/serverguide/ftp-server.html  ssh is enough so far.
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
