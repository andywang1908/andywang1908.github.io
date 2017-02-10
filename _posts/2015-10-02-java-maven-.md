
## tip

- maven update project(alt+F5)
- clean: server project(eclipse) maven(command clean) 
- webapp war: if can not update directly , delete and save first , reopen setting and add, be careful to confirm the webapp fold location
- import as project:mvn eclipse:eclipse    or   mvn eclipse:eclipse -Dwtpversion=1.0  ,otherwise import as maven
- if fail, check built war or web-inf *.xml

## proxy
the big action is delete all resposity for some lib is missinng at first

.m2 settings.xml

```
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                      http://maven.apache.org/xsd/settings-1.0.0.xsd">
  <localRepository/>
  <interactiveMode/>
  <usePluginRegistry/>
  <offline/>
  <pluginGroups/>
  <servers/>
  <mirrors/>
  <proxies>
    <proxy>
      <id>myproxy</id>
      <active>true</active>
      <protocol>http</protocol>
      <host>204.40.194.129</host>
      <port>3128</port>
      <username>EBC\WangAn1</username>
      <password>Ontario5$</password>
      <nonProxyHosts>localhost,127.0.0.1</nonProxyHosts>
    </proxy>
  </proxies>
  <profiles/>
  <activeProfiles/>
</settings>
```

## multi spring boot

[Ref](http://m.blog.csdn.net/article/details?id=50068985)(multiple-Spring Boot-MVC-java config.pdf)

## multi pom project

[best](http://www.blogjava.net/fancydeepin/archive/2015/06/27/maven-modules.html)(maven 多模块项目 - fanlychie - BlogJava.pdf)


## myeclipse , learn some more detail, detail < new < job

[ref](http://blog.csdn.net/gebitan505/article/details/51861800)(myeclipse+maven实现多模块项目struts+spring+mybatis - AndyLizh的专栏)
