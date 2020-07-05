---
title: 解决hexo图床问题
date: 2020-06-10 22:21:16
categories: 编程
tags:
   - Blog
   - Hexo
author: 唐川
avatar: https://cdn.jsdelivr.net/gh/JLUtangchuan/picBed@dev/img/20200704232008.jpg
authorLink: 
authorAbout: 
authorDesc: 
comments: true
keywords: 
description: 
photos: https://cdn.jsdelivr.net/gh/JLUtangchuan/picBed@dev/img/01a3f4589ea315a801219c77c63f72.jpg@1280w_1l_2o_100sh.jpg
---

# {{ title }}

目前采用的是typora+picgo+github图床的方式，在github中创建一个repo链接到picgo，新版typora支持使用picGo上传图片，比较方便，具体方式可在网上找。

<img src="https://raw.githubusercontent.com/JLUtangchuan/picBed/dev/image-20200610222252489.png" alt="image-20200610222252489" style="zoom:50%;" />

![](https://raw.githubusercontent.com/JLUtangchuan/picBed/dev/image-20200610222402695.png)

使用后可能存在一个问题：如果不挂VPN仍然显示不出图片，这是因为`raw.githubusercontent.com`的IP地址找不到，需要手动在host文件中添加其地址，Win10中host文件位置

```
C:\Windows\System32\drivers\etc
```

`raw.githubusercontent.com`的IP地址如下（可以ping一下或者在[IPAddress](https://www.ipaddress.com/)中搜索）

```
199.232.68.133 raw.githubusercontent.com
```

