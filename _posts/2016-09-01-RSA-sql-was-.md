
## install

### linux

cd /opt/IBM/InstallationManager/eclipse

sudo /opt/IBM/InstallationManager/eclipse/launcher

## config

### workspace setting
- compile 1.6
- Window -> Preferences -> General -> Workspace : Text file encoding UTF-8
- font size
- xml space
- disable autostart was  
server double click auto restart after publish
- DBEEDD eye protect color: 
Hue = 84 Sat = 86 Lum = 215  or  Red = 219 Green = 238 Blue = 221

### install was7 and was8 together , avoiding port conflict

change port http://www.ibm.com/support/knowledgecenter/SS7JFU_7.0.0/com.ibm.websphere.migration.express.iseries.doc/info/iseriesexp/ae/rmig_portnumber.html
for was 7 serverindex.xml and virtualhosts.xml
 9080-->9081  9100-->9101   2809-->2810  9060->9061  9043->9044  9443->9444  2810-->2811

It will be a better way to install 8 first ,and install 7 , installation will change port automaticlly.


### svn

In Eclipse IDE (Helios version), top menu, select “Help” –> “Install New Software…”. And puts http://subclipse.tigris.org/update_1.6.x in the “work with” textbox and click on the “Add” button. Select all components and install it.
[Ref](http://www.mkyong.com/eclipse/how-to-enable-subversion-svn-in-eclipse-ide/)

## install was

it is better to intall secondly, so port will change to 9081 from 9080, so it will be avoid conflict.

```
http://192.168.10.129:9060/ibm/console
https://192.168.10.129:9043/ibm/console

https://192.168.10.130:9044/ibm/console
https://10.160.200.76:9044/ibm/console


http://192.168.10.130:9081

sudo /opt/IBM/WebSphere/AppServer_1/bin/startServer.sh server1
sudo /opt/IBM/WebSphere/AppServer_1/bin/stopServer.sh server1

cd ~
tar -czvf WebSphere8.tar.gz /opt/IBM/WebSphere8

sudo fdisk -l

/dev/sdb1            2048 450562047 450560000 214.9G  7 HPFS/NTFS/exFAT
/dev/sdb2       450562048 976769023 526206976 250.9G  7 HPFS/NTFS/exFAT

sudo mkdir /media/exfat
sudo mount -t exfat /dev/sdb2 /media/exfat1
sudo mkdir /media/ntfs-ext
sudo mount -t ntfs /dev/sdb1 /media/ntfs-ext
sudo umount /dev/sdb1 

sudo mkdir /opt/IBM/WebSphere8
sudo tar -xzvf WebSphere8.tar.gz -C /opt/IBM/WebSphere8
sudo mv /opt/IBM/WebSphere8/opt/IBM/WebSphere8/AppServer /opt/IBM/WebSphere8


sudo /opt/IBM/WebSphere8/AppServer/bin/startServer.sh server1


sudo /opt/IBM/InstallationManager/eclipse/IBMIM

TODO how to call profile management tool
```

## usage

### how to create wsdl in RSA from service interface or impl
- in RSA , right mouse button on ServiceImpl
- levle middel + was7 rpc
- select my own interface
- trim wsdl name as same as interface

### generate ws client
```
ws client
C:\Users\andy\Music>wsimport -keep -verbose -extension http://hscziqdcapwas01.cihs.gov.on.ca:13133/SOIACWSProject/IACCleanWSService/WEB-INF/wsdl/IACCleanWSService.wsdl
how to run fileupload only in server36
seperate class to different log level
```

### webservice can not call, or something lib can not be loaded or called

1.server double click property file             choose "Run server with resource on Server"
 
so can change ear property in admin console
 
2.select ear in console
 
set    class loading and update detection      ->  class loader order    to   parent last
 
   and   manage module   ->   choose ear   ->   class loader    to   parent last

Ps:Put wsdl in proper position

### package

Make sure there is no default virtual host
 
/WebContent/WEB-INF/ibm-web-bnd.xml
 
Delete
   <virtual-host name="default_host" />

## sql

### mysql backup:

CREATE TABLE oc_product_2016 LIKE oc_product;
INSERT oc_product_2016 SELECT * FROM oc_product;

you can test to change on oc_product_2016 first
update oc_product_2016 set price=(price-10)*0.5;



## rss
[ibm](http://www-01.ibm.com/support/docview.wss?uid=swg27012924)

## idea

[安装配置Portal 6.0 和优化性能并减少资源消耗的方法](http://www.lai18.com/content/2897576.html)
[RAD V7进行开发安装和配置WebSphere Portal V6.0 优化小窍门](http://www.lotuschina.net/Document/detail/tid/2423)
[Integrating-Eclipse-and-WebSphere-Portal-7](http://www.theserverside.com/tip/Integrating-Eclipse-and-WebSphere-Portal-7)

## common mistake

[R1](https://www.toptal.com/nodejs/top-10-common-nodejs-developer-mistakes)

[R2](https://www.airpair.com/node.js/posts/top-10-mistakes-node-developers-make)

[3 Common node.js design patterns that are misused](https://www.appneta.com/blog/3-common-node-js-design-patterns-that-are-misused/)

[Node.js Best Practices](https://blog.risingstack.com/node-js-best-practices/)

[Advanced Error Handling in Node.js With Best Practices](https://www.linkedin.com/pulse/advanced-error-handling-nodejs-best-practices-sandip-das?articleId=7819533121517654217)

## anti pattern

## interview question
[R1](https://www.toptal.com/nodejs/interview-questions)
[Ref](http://stackoverflow.com/questions/1480528/what-is-the-difference-between-a-portlet-and-a-servlet/8927313#8927313)

## hello

[ref](http://www.programgo.com/article/44571892898/)


