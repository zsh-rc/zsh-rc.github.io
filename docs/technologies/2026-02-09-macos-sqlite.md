---
layout: post
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
