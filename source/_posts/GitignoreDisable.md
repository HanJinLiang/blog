---
title: .gitignore修改无效
date: 2020-12-24 18:50:48
updated: 2020-12-24 18:50:48
cover: https://cdn.jsdelivr.net/gh/jerryc127/CDN@latest/cover/default_bg.png
---

## .gitignore修改无效问题
记录一次.gitignore修改无效问题解决

### 问题原因
先提交到了git目录，文件目录已经被track
### 解决
把需要忽略的文件从已经track状态修改为未被track，.gitignore就会生效
```
git rm -r --cached fileName 
```
