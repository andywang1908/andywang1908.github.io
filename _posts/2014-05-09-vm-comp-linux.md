
## command linux

## UI window

### v-1 in local

1. unplug internet use mary as admin
2. create normal user mary  netplwiz use this to login
3. disable update

### v0 

1. using advanced mood with station not player, choose vm9 format so far.
2. 12G/8G NAT  in on NAT can be actived
2. if server 2008 , choose standard version
2. if server 2012 , be careful of memory leak
2. use andy to be first(admin) user, no need to create normal user

### v1
1. vmtool
2. netplwiz admin
2. NO HD MEMORY   PROGRAM FIRST
2. setup 7z manually
2. http://proxy2.gonet.gov.on.ca:9001/proxy.pac
2. turn off firewall        command quick edit      taskbar not combine
3. turn off update
2. no active...
2. allow remote desktop later?

### v1.5 something missing

1. rem disk
2. some green pro for pdf,screen,putty,winscp

### v2 slim

#### no need remove andy

#### delete big space , need change owner to administrators first

1. C:\Windows\Help (66.7M) windows 7的說明檔，不看的話可以刪掉。
2. C:\Windows\IME\IMEJP10 日文輸入法(37.8M)。
2. C:\Windows\winsxs\Backup 
2. remove usb dirver to another place????
2. something in winsxs by packing KB2852386 , but there is no file in brand-new system
https://support.appliedi.net/kb/a110/how-to-enable-the-disk-cleanup-tool-on-windows-server-2008-r2.aspx
https://technet.microsoft.com/en-us/library/ff630161(WS.10).aspx

[ref](http://save-coco.blogspot.ca/2010/05/windows-7.html)

#### service

### try to green build

#### java scala

```
setx JAVA_HOME "C:\green\dev\java\jdk\jdk1.8.0_101" /M
setx M2_HOME "C:\green\dev\java\mvn\apache-maven-3.2.5" /M
setx MAVEN_HOME "C:\green\dev\java\mvn\apache-maven-3.2.5" /M
mvn –version
java -version

SETX /M Path "C:\green\pro\7-Zip;%M2_HOME%\bin\;%JAVA_HOME%\bin\;%Path%;" //  /M means to set PATH value on machine level, but not working well for %%
C:\green\pro\7-Zip;%JAVA_HOME%\bin\;%M2_HOME%\bin\;%NODE_HOME%\;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
```

[ref](https://ss64.com/nt/setx.html)
[ref](https://www.mkyong.com/maven/how-to-install-maven-in-windows/)

#### node

```
## C:\Users\WangAn1\AppData\Roaming\npm is used for install program
7z x "C:\green\dev\node\npm\node-v6.9.5-win-x64.zip" -y -aos -o"C:\green\dev\node\npm\v6.9.5"
setx NODE_HOME "C:\green\dev\node\npm\v6.9.5" /M

SETX /M Path "%Path%;%NODE_HOME%\;"   -- not working well for NODE_HOME

npm config set strict-ssl =false
npm config set proxy "http://ebc%5Cwangan1:Ontario6%24@204.40.194.129:3128"
npm config set https-proxy "https://ebc%5Cwangan1:Ontario6%24@204.40.194.129:3128"
npm config set registry=http://registry.npmjs.org
```

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
