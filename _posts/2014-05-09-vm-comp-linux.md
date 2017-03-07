
## command linux

## UI window

### proxy list
apt-get
wget
docker

### v-1 ssh

1. sudo apt-get install openssh-server (a.load iso as cd-rom b.sudo mount -o loop  -t iso9660 /dev/cdrom /media/cdrom ) may help

home:::
sudo vi /etc/ssh/sshd_config
change port to 5431
2. sudo apt-get update

### v0 


### v1 docker
1. vmtool? later
2. https://docs.docker.com/engine/installation/linux/ubuntu/#install-from-a-package   docker install

or 

export http_proxy=http://204.40.194.129:3128      not working , need sudo to set into global?
export https_proxy=$http_proxy            not working , need sudo to set into global?
sudo apt-get update
sudo apt-get install wget
sudo wget -qO- https://get.docker.com/ | sh
sudo service docker start

--
Via ~/.wgetrc file:  working well
use_proxy=yes
http_proxy=http://204.40.194.129:3128
https_proxy=http://204.40.194.129:3128

or via -e options placed after the URL:
wget ... -e use_proxy=yes -e http_proxy=127.0.0.1:8080 ...

vi ~/.curlrc
proxy = http://204.40.194.129:3128

proxy = http://username:password@proxy-host:port
--

### v1.5 something missing
1. samba later?
2.
privallage
sudo groupadd docker
sudo usermod -aG docker andy ($USER)
ref:https://docs.docker.com/engine/installation/linux/ubuntulinux/

# ZQoPQ2g6uVJE7cy4 is a safe password
docker run -dt --name shadowsocks -p 5430:5000 mritd/shadowsocks -k ZQoPQ2g6uVJE7cy4 -w 2 -f
docker pull mritd/shadowsocks

TODO:
docker start shadowsocks           on reboot automatic

client:
https://ttt.tt/150/


-. fixed ip
sudo vi /etc/network/interfaces

# The primary network interface     --eth0 or ens33
auto ens33
iface ens33 inet static
address 192.168.1.90
gateway 192.168.1.1
netmask 255.255.255.0
dns-nameservers 8.8.8.8
#network 192.168.3.0
#broadcast 192.168.3.255

make affection
sudo /etc/init.d/networking restart

ref:http://forum.ubuntu.org.cn/viewtopic.php?f=73&t=190174

-. setup email
sudo apt-get install ssmtp
sudo cp /etc/ssmtp/ssmtp.conf /etc/ssmtp/ssmp.conf.init
sudo vi /etc/ssmtp/ssmtp.conf

root=andywang1909@gmail.com
#465 587
mailhub=smtp.gmail.com:587
rewriteDomain=gmail.com
AuthUser=andywang1909
AuthPass=yUqian12
AuthMethod=LOGIN
FromLineOverride=YES
UseTLS=YES
UseSTARTTLS=Yes

ssmtp andywang1908@gmail.com < newIp.txt for testing, may need restart


ref:
https://wiki.archlinux.org/index.php/SSMTP
http://askubuntu.com/questions/12917/how-to-send-mail-from-the-command-line

-. ip change
sudo apt install curl

----shell    chmod +x ip.sh
#!/bin/bash
cd /home/andy/ip
oldIp=$(<ip.txt)
#oldIp='12.21.12.12'
dig +short myip.opendns.com @resolver1.opendns.com > newIp.txt
newIp=$(<newIp.txt)
echo "Subject: Ip is changed to $newIp " > newIp.txt
#echo "oldIp: $oldIp"
#echo "newIp: $newIp"

if [ $oldIp != $newIp ]
then
  echo "ip is changed to $newIp"
  #/usr/sbin/ssmtp zhaojy@asiainfo.com,andywang1908@sina.com < newIp.txt
  /usr/sbin/ssmtp andywang1908@sina.com < newIp.txt
  gxpass=yUqian12
  gxuser=andywang1908
  gxyum=1h625g2778.imwork.net
  theurl="http://$gxuser:$gxpass@ddns.oray.com/ph/update?hostname=$gxyum&myip=$newIp"
  curl "$theurl"
  echo "update ip in $theurl"
  dig +short myip.opendns.com @resolver1.opendns.com > ip.txt
else
  newIp='12.21.12.12'
  echo "ip is not changed"
fi

---
ref:
http://unix.stackexchange.com/questions/22615/how-can-i-get-my-external-ip-address-in-a-shell-script

sudo crontab -e
*/2 * * * * . /etc/profile; /home/andy/ip/ip.sh
#*/2 * * * * . $HOME/.profile; . /etc/profile; /home/andy/ip/ip.sh


### v2 slim

#### no need remove andy

### try to green build

#### java scala

sudo apt-add-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer

update-java-alternatives --list
sudo update-java-alternatives --set /path/to/java/version
update-java-alternatives is a convenience tool that uses Debian's alternatives system (update-alternatives) to set a bunch of links to the specified java version (e.g. java, javac?????!!!!!!, ...).

this is good
sudo update-alternatives --config java

#### node

```
nvm is hard behind proxy , but is stonger

sudo apt-get install npm
npm -v

npm config set strict-ssl =false
npm config set proxy "http://ebc%5Cwangan1:Ontario6%24@204.40.194.129:3128"
npm config set https-proxy "https://ebc%5Cwangan1:Ontario6%24@204.40.194.129:3128"
npm config set registry=http://registry.npmjs.org

sudo npm install -g n
sudo n stable  (may need curl proxy, or try sudo export)
node -v
```

[ref](http://askubuntu.com/questions/426750/how-can-i-update-my-nodejs-to-the-latest-version)
[nvm(nvmw) vs n ](http://www.mattpalmerlee.com/2013/03/23/installing-and-switching-between-multiple-versions-of-node-js-n-vs-nvm/)
[nvm is better](http://taobaofed.org/blog/2015/11/17/nvm-or-n/)

##### multi version

[n  and nvm](https://www.kancloud.cn/iwzh/wzhquestion/218860)
[virtualenv 是 lib 级别的隔离，如果需要python解释器的隔离，可以直接用, pathon and node all need think of lib and sdk version]()

#### python

### green code

1. use linux samba or just local temp file
2. git
2. svn

#### git

修改前

    [remote "origin"]
    url = https://github.com/humingx/humingx.github.io.git
    fetch = +refs/heads/*:refs/remotes/origin/*

修改后

    [remote "origin"]
    url = git@github.com:humingx/humingx.github.io.git
    fetch = +refs/heads/*:refs/remotes/origin/*
[git ssh](https://segmentfault.com/a/1190000002645623)

hen in your git bash you have to write the following line:
git config --global core.excludesfile ~/.gitignore_global
If the respository already exists then you have to do the following:

1)git rm -r --cached .
2)git add .
3)git commit -m ".gitignore is now working"
If the step 2 doesn´t work then you should write the hole route of the files that you would like to add.


[ignore](http://stackoverflow.com/questions/4308610/how-to-ignore-certain-files-in-git)


#### svn with x-windows

[JavaHL](http://subclipse.tigris.org/wiki/JavaHL)
[proxy](http://askubuntu.com/questions/109673/how-to-use-apt-get-via-http-proxy-like-this)
[JavaHL](http://stackoverflow.com/questions/9303293/subclipse-and-javahl-installation-headache)

### green IDE

#### selenium

#### eclipse

```
7z x "F:\blue\java\eclipse\eclipse-jee-neon-2-win32-x86_64.zip" -y -aos -o"C:\green\dev\java\eclipse\neon"
```

#### eclipse workspace

```
utf-8
Window > Preferences > General > Content Types, set UTF-8 as the default encoding for all content types.
Window > Preferences > General > Workspace, set "Text file encoding" to "Other : UTF-8".

84 86 215 + font size 18

4 spaces

for each installation (but this may vary for multi-user installations), in files stored in: <eclipse_home>/eclipse/configuration/.settings/
for each workspace, in files stored in <workspace>/.metadata/.plugins/org.eclipse.core.runtime/.settings .

https://github.com/andywang1908/java-spring
jetty:run
tomcat7:run
http://localhost:8080/cempedak-web/helloWorld/hello?type=a
```

### big branch

#### RSA

#### IDEA (useless)

#### office (useless)

[download](http://www.eclipse.org/downloads/packages/release/Neon/2)

## no need for UI linux, Mac

## component eclipse (no time for IDEA)

## component sublime
