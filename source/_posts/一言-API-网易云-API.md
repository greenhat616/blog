---
title: 一言 API & 网易云 API
tags: [ "apis", "api", "hitokoto", "netease"]
permalink: teng-koa
id: 14
updated: '2018-01-31 00:59:49'
date: 2018-02-19 16:11:47
cover: https://piccdn.freejishu.com/images/2016/07/18/59fe422cee6a2b825e4521ace38cc8b0.jpg!/format/jpg
toc: true
---

### 何为 一言？
  
>  动漫也好、小说也好、网络也好，不论在哪里，我们总会看到有那么一两个句子能穿透你的心。我们把这些句子汇聚起来，形成一言网络，以传递更多的感动。如果可以，我们希望我们没有停止服务的那一天。  
> 简单来说，一言指的就是一句话，可以是动漫中的台词，也可以是网络上的各种小段子。  

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="330" height="86" src="https://cdn.a632079.me/163music.html?playlist=492926375" style="margin:0"></iframe>

### 何为 网易云？
Emmmm, 我想这个没啥好说的。

### 使用
> 项目实际是个 Live Demo，所以仅保证可用，不保证速度。  
> 项目基于 Teng-koa (https://github.com/a632079/teng-koa) 还望使用之余给个 Star~

#### 状态统计
访问： https://api.a632079.me/status  
#### 一言
> 一言数据基于 `Hitokoto.cn`, 已经过授权。由于 API 本身是基于 v1 的再设计，所以预计在下月初就能将原有框架更新完毕。 

接口： `https://api.a632079.me`   
支持的参数: `http://hitokoto.cn/api`    
与目前的接口不同，我们目前还支持提供 `JSONP` 返回。  
以下是一个调用例子：  
https://api.a632079.me?callback=poi&encode=text


#### 网易云
接口: `https://api.a632079.me/nm`  
支持一下 8 个功能：  
* 搜索曲目 - `https://api.a632079.me/nm/search/:name`  
* 获得歌单 - `https://api.a632079.me/nm/playlist/:id`  
* 获得曲图 - `https://api.a632079.me/nm/picture/:id/:height?`  
* 获得作者 - `https://api.a632079.me/nm/artist/:id`  
* 获得专辑 - `https://api.a632079.me/nm/album/:id`  
* 获得歌词 - `https://api.a632079.me/nm/lyric/:id`  
* 获得歌曲 - `https://api.a632079.me/nm/url/:id`   
* 获得细节 - `https://api.a632079.me/nm/detail/:id`  
* 获得概要 - `https://api.a632079.me/nm/summary/:id`
  * 启用歌词 - `https://api.a632079.me/nm/summary/:id?lyric=true`
* 重定向
  * 歌曲 - `https://api.a632079.me/nm/redirect/music/:id`
  * 图片 - `https://api.a632079.me/nm/redirect/picture/:id`
