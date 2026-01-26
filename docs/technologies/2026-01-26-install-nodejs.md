---
layout: post
title: 使用NVM安装NodeJS
author: Umbra
date: 2026-01-26
parent: MacOS📚
tags: [MacOS, Node]
excerpt: Node 版本管理器（NVM）是开发人员常用的工具，可以帮助他们在单台机器上安装和管理多个版本的 Node.js。
---

## Install NVM

更新homebrew到最新版本

~~~bash
brew update
~~~

安装NVM（Node版本管理器）

~~~bash
brew install nvm
~~~

## 配置环境变量

~~~bash
nano ~/.zshrc
~~~

在~/.zshrc文件中增加以下内容

~~~bash
# NVM
export NVM_DIR="$HOME/.nvm"
[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
[ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
~~~

刷新配置

~~~bash
source ~/.zshrc
~~~

## 安装Node.JS

查看可用的node版本

~~~bash
nvm ls-remote
~~~

安装最新版本

~~~bash
nvm install node
~~~

或安装指定版本

~~~bash
nvm install 22
~~~

查看已经安装的版本

~~~bash
nvm ls
~~~

指定默认版本

~~~bash
nvm alias default 20
~~~
