---
title: Bash-空值判断
top: false
cover: false
toc: true
mathjax: false
date: 2023-03-15 17:36:42
author:
img:
coverImg:
password:
summary:
tags:
categories:
---

1.  空值判断
```bash
name=
if [ $name ];then
echo "not null"
else
echo "is null"
else> fi
# is null
```

2. 转换成字符串
```bash
name=
if [ "$name"="" ];then
echo "is null"
else
echo "not null"
fi
#is null
```

3.  -n：不等于
```bash
name=
if [ ! -n "$name" ];then  
echo "is null"
else
echo "not null"
fi
#is null
```

4. -z: 空
```bash
name=
if [ -z "$name" ];then # 变量可不带 双引号
echo "is null"
else
echo "not null"
fi
#is null
```
