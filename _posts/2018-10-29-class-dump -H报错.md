---
layout:     post                    # 使用的布局（不需要改）
title:      关于class-dump -H时报错               # 标题 
subtitle:   用于查看头文件    #副标题
date:       2018-10-29              # 时间
author:     梅洛                      # 作者
header-img: img/post-bg-github-cup.jpg    #这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               #标签
    - iOS
---

#### ipa来自？
找ipa？下载个pp助手，搜索app下载即可。右击ipa -> 打开方式 -> 归档实用工具 -> Payload -> xxx.app(.app是隐藏扩展名)。
终端cd到xxx.app所在目录即可。

#### class-dump -H 报错
class-dump -H时报错，可能是因为该项目是用OC和Swift混编。
Error: Cannot find offset for address 0x580000000100bcd8 in stringAtAddress: 错误。

#### 更新class-dump
下载个新的class-dump，链接 <a  href ="https://pan.baidu.com/s/128q6WLPUsrPYZN9NQJudSA">百度云下载</a> 密码:mxoc

前往文件夹，/usr/local/bin，拷贝进去。
至于在终端执行class-dump -H XXX.app，提示没有权限的，执行sudo class-dump -H XXX.app，然后输入你电脑密码即可。

class-dump文件来源：
<a  href ="https://github.com/AloneMonkey/MonkeyDev.git">感谢AloneMonkey提供</a>


