---
layout: post
title: "Ubantu Developer VM"
date: 2016-08-15
---

Set up a ubuntu for development with windows.
	
## some tips:

1. Launch Terminal by pressing Ctrl+Alt+T
2. sudo gedit /etc/profile
2. Item2
2. Item3

## some different servcie:

## some develop tool:

1. [git](#git)
2. sublime

## compile lib:

- [php](#php)
- Another item
  - Unordered sub-list. 
- Actual numbers don't matter, just that it's a number
  - Ordered sub-list
- George Washington abc.
- John Adams
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

### bulid blog with markdown
```
[ref](http://jmcglone.com/guides/github-pages/)
```

## <a name="php"></a>php



| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |


In the words of Joseph Campbell:

> [A hero is someone who has given his or her life to something bigger than oneself.](http://www.brainyquote.com/quotes/topics/topic_inspirational2.html)

<img src='/images/2016-08-04-CI.png'/>

try image

![Alt text](https://googledrive.com/host/0B-gKvP-SnWnKQ1d4cE9GSVQ5RWc/image/2016-08-04-CI.png "Optional title")
