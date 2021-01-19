---
title: el-table hover背景颜色去除
date: 2021-01-19 11:27:05
tags:
---

## el-table hover背景颜色去除

```
 /deep/ .el-table tbody tr { pointer-events:none; }
```
但是当存在有点击的cell时候，会无法响应。
## 最后解决方案

```
 /deep/.el-table__body tr.hover-row>td{
    background-color: transparent;
  }
```
