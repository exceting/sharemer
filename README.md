![blockchain](https://raw.githubusercontent.com/exceting/sharemer/master/business/api/master/src/main/resources/static/image/logo.png "ShareMer")
### 一个小众的音乐分享社区
访问本站：首先你要有一副黑框眼镜，其次你的裤腰带要够到你的胳肢窝，然后你的姿势水平要足够高，最后你要会念诗（开玩笑的，活着挺好）
### 前言
这个ReadMe更新于停止维护该项目的半年后（2019-03-09，突然发疯，想要写一下）
>这个网站停停做做搞了很久，后面还是放弃了，放弃的原因有很多，总结了有以下几点吧：<br/>
>- 自己一个人搞一个系统，太单调，又太难，没有人愿意一起交流技术和方案，时间久了，容易自闭:）
>- 就算上线，针对目前这个移动互联网时代，娱乐向的web端网站已经很难很难吸引到任何流量了。
>- 穷，养不起一个网站，无人问津的小网站也不行（#滑稽）
>- 觉得自己技术太菜，需要给自己充充电，有的人嘛，就是觉醒的太晚成熟的太晚吧，不想为了一个产品形态都不成熟的网站耽搁更多时间。
>项目虽然烂尾了，不过还是想在这里展示下效果和功能，毕竟一个项目业余时间做了那么久，算是有点感情吧~

### 网站是做什么的？
网站以音乐分享和视频分享为主要功能，因为作者本人很喜欢听音乐，也很喜欢一些音乐主旋律视频，一直以来想做一个小众的音乐共享平台，提供更多的人分享自己发现的优秀音乐和音乐视频，鼓励用户自己上传原创音频或者搬运音频，供站内更多人分享。

### 网站涉及的语言、框架、db等
本网站基于java语言，采用Spring boot、Mybatis框架，使用Gradle搭建及开发，其次采用Memcached做底层数据缓存、Redis做数据结构缓存，Mysql为底层持久化数据库，Druid作它的连接池，CDN采用七牛云存储。

### 主要功能
功能点|功能描述
-------|:--
音频分享&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|站外音频分享，支持爬取关键信息（仅支持网易云音乐）
视频分享&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|站外视频分享，到目前为止支持用户拉取BiliBili（B站）、AcFun（A站）、MissEvan（M站）、音悦台上的视频信息（同下面爬虫）以及播放器
投稿|用户自主投稿，支持审核流程，稿件分为小视频&音频
弹幕|弹幕功能只对站内投稿生效，不支持对外站资源发弹幕
收藏&收藏单&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|站内收藏，收藏单里包含用户站内收藏的音频、视频、稿件三块内容。
爬虫|在网站初期数据量不大时，可以通过爬虫后台进行伪造用户分享数据（支持上述提到的网站的信息爬取，包含标题、封面、播放源、原up主等关键信息）
博客|每个用户的个人空间都是自己的博客首页，里面有时间轴、博客、相册、收藏（与主站互通）等功能。
世界|世界功能是一个很关键的功能，支持全站用户在任意资源（音视频、收藏单、博客）下点击分享按钮，选择世界频道，发送出去，世界频道是个即时的聊天窗口，用户打开对应频道的世界窗口后，站内任意用户分享的动态可以即时发现。

### 运行效果及功能简介
项目一共分为两个重要模块，分别点击进入即可查看功能介绍及效果图：<br/>
- [Sharemer主站](https://github.com/exceting/sharemer/blob/master/business/api/master/README.md)
- [Sharemer爬虫后台](https://github.com/exceting/sharemer/tree/master/business/manager/master/README.md)
