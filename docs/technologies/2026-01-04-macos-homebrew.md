---
layout: post
title: Homebrew加速（中国）
author: Shao Zelian
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
