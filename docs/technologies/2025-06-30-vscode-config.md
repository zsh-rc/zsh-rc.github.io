---
layout: post
title: VSCode编辑器配置
author: Shao Zelian
date: 2025-06-30
parent: 💻 Technologies
tags: [tools]
excerpt: VSCode是编程人员最常用的IDE工具之一
---

## 常用的插件安装

| 插件名称                  | 用途说明                                                   |
| ------------------------- | ---------------------------------------------------------- |
| Github Copilot            | AI Pair Programming                                        |
| Markdown All in One       | 适合用Markdown文章编写，可以提供Markdown Formatter等功能。 |
| Rainbow CSV               | 用不同颜色显示不同的Column，以方便识别不同列值。           |
| Prettier - Code formatter | Code formatter                                             |

## 中英文等宽字体设置

[下载Ubuntu Mono字体文件](https://github.com/powerline/fonts/tree/master/UbuntuMono)

- Ubuntu Mono derivative Powerline Bold Italic.ttf
- Ubuntu Mono derivative Powerline Bold.ttf
- Ubuntu Mono derivative Powerline Italic.ttf
- Ubuntu Mono derivative Powerline.ttf

配置VSCode

1. 打开VSCode -> "Settings" -> "Text Editor" -> "Font"
2. 找到"Font Family"配置，在已有字体名称前增加“'Ubuntu Mono derivative Powerline'（必须与系统字体文件名称一致）。
   例如：'Ubuntu Mono derivative Powerline', Consolas, 'Courier New', monospace
3. 设置完毕后，重启VSCode。
