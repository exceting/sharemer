![blockchain](https://raw.githubusercontent.com/exceting/sharemer/master/business/api/master/src/main/resources/static/image/logo.png "ShareMer")
### 一个音乐分享社区网站的代码
访问本站：首先你要有一副黑框眼镜，其次你的裤腰带要够到你的胳肢窝，然后你的姿势水平要足够高，最后你要会念诗:）
### 前言
这个ReadMe更新于停止维护该项目的半年后（2019-03-09，突然发疯，想要写一下）

### 网站是做什么的？
音乐分享和视频分享

### 本站涉及的语言、框架、db等
模块|技术
:--|:--
语言|java
框架|Spring Boot、Mybatis
DB|mysql（池：Druid）
nosql|Memcached、Redis
CDN|七牛云
构建工具|gradle

### 主要功能

功能点|功能描述
:--|:--
音频分享|站外音频分享，支持爬取关键信息（仅支持网易云音乐）
视频分享|站外视频分享，到目前为止支持用户拉取BiliBili（B站）、AcFun（A站）、MissEvan（M站）、<br/>音悦台上的视频信息（同下面爬虫）以及播放器
投稿|用户自主投稿，支持审核流程，稿件分为小视频&音频
弹幕|弹幕功能只对站内投稿生效，不支持对外站资源发弹幕
评论系统|提供全站统一的评论系统，任意一个页面下面均可简单的接入
收藏&收藏单|站内收藏，收藏单里包含用户站内收藏的音频、视频、稿件三块内容。
爬虫|在网站初期数据量不大时，可以通过爬虫后台进行伪造用户分享数据<br/>（支持上述提到的网站的信息爬取，包含标题、封面、播放源、原up主等关键信息）
博客|每个用户的个人空间都是自己的博客首页，里面有时间轴、博客、相册、<br/>收藏（与主站互通）等功能。
世界|世界功能是一个很关键的功能，支持全站用户在任意资源（音视频、收藏单、博客）<br/>下点击分享按钮，选择世界频道，发送出去，世界频道是个即时<br/>的聊天窗口，用户打开对应频道的世界窗口后，<br/>站内任意用户分享的动态可以即时发现。

### 运行效果及功能简介
项目一共分为两个重要模块，分别点击进入即可查看功能介绍及效果图：<br/>
- [Sharemer主站](https://github.com/exceting/sharemer/blob/master/business/api/master/README.md)
- [Sharemer爬虫后台](https://github.com/exceting/sharemer/tree/master/business/manager/master/README.md)
