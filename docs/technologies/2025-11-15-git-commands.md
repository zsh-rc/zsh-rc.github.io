---
layout: post
title: 常用Git命令
author: Umbra
date: 2025-11-15
parent: 💻 Technologies
tags: [git]
excerpt: 常用Git命令（持续更新）
---

## Common used git commands

- Remote
  - Lista all remote repositories
  
    ~~~bash
      git remote -v
    ~~~
  
  - Add remote repositories

    ~~~bash
      git remote add {i.e. origin} {i.e. https://github.com/user/repo.git}
    ~~~

  - Remove remote repositories

    ~~~bash
      git remote remove {i.e. origin}
    ~~~

- Reset proxy (global)
  git config --global --unset http.proxy
  git config --global --unset https.proxy

- Commit
  git commit -m "message"
