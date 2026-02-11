---
layout: post
<<<<<<< Updated upstream
title: SQLite
author: Umbra
date: 2026-02-09
parent: MacOS📚
tags: [MacOS, Database]
excerpt: SQLite is a small, fast, self-contained, high-reliability, full-featured, SQL database engine. SQLite is the most used database engine in the world. SQLite is built into all mobile phones and most computers ...
---

## SQLite Links

- [Official SQLite Website](https://sqlite.org/)
- [DB Browser for SQLite](https://sqlitebrowser.org/)

## Installation (MacOS)

- Check if SQLite is already installed?
  
    ~~~bash
    sqlite3 --version
    ~~~

- Install SQLite using Homebrew

    ~~~bash
    brew install sqlite
    ~~~

- Install DB Browser for SQLite

    Download and install DB Browser for SQLite from [the official website](https://sqlitebrowser.org/dl/) or use Homebrew:

    ~~~bash
    brew install db-browser-for-sqlite
    ~~~

## Backup (MacOS)

Navigate to the folder where the database is located. Run the following backup command.

~~~bash

    sqlite3 your_database.db ".backup 'your_database_backup.db'"

~~~
=======
title: Homebrew加速（中国）
author: Umbra
date: 2026-01-04
parent: MacOS📚
tags: [MacOS, Homebrew]
excerpt: 执行brew命令默认会自动从 https://formulae.brew.sh/api/formula.jws.json 下载最新的JSON api文件, 使用国内的镜像会解决速度慢的问题。
---

## 在～/.zshrc文件中设置环境变量如下。

    ~~~bash

    ####### brew安装镜像加速

    #
    # 阿里: https://mirrors.aliyun.com/homebrew
    # tuna: https://mirrors.tuna.tsinghua.edu.cn
    # ustc: https://mirrors.ustc.edu.cn
    #

    export HOMEBREW_BREW_GIT_REMOTE="https://mirrors.ustc.edu.cn/brew.git"
    export HOMEBREW_CORE_GIT_REMOTE="https://mirrors.ustc.edu.cn/homebrew-core.git"
    export HOMEBREW_BOTTLE_DOMAIN="https://mirrors.ustc.edu.cn/homebrew-bottles"
    # brew4.x API加速
    export HOMEBREW_API_DOMAIN="https://mirrors.ustc.edu.cn/homebrew-bottles/api"
    # hide
    export HOMEBREW_NO_ENV_HINTS="1"

    ~~~

## 刷新配置令其生效

    ~~~bash
        source ~/.zshrc
    ~~~
>>>>>>> Stashed changes
