---
title: Hello World--hexo使用方法
tags: 教程
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```
### 高阶用法

#### 添加歌单（网易云）

```
{% meting "歌单编号" "netease" "playlist" "theme:#FF4081" "mode:circulation" "mutex:true" "listmaxheight:340px" "preload:auto" %}
```
#### 单个歌曲形成歌单

```
{% aplayerlist %}
{
"narrow":false,//播放器袖珍风格
"autoplay":true,
"mode":"random",//可选：random(随机播放),single(单曲播放),circulation(循环播放),order(列表播放)
"showlrc":3,//可选：歌词显示配置项，1-3
"mutex":true,//开启时如果该页面有其他aplayer播放，该播放器会暂停
"theme":"#e6d0b2",//播放器风格色彩设置，默认为#b7daff
"preload":"metadata",//音乐文件预载入模式，可选："none","metadata","auto",默认auto
"listmaxheight":"513px",//该播放列表的最大长度
"music":[
{
"title":"CoCo",
"author":"Jeff Williams",
"url":"caffeine.mp3".
"pic":"caffeine.jpeg",
"lrc":"caffeine.txt"
}
{
"title":"アイロニ",
"author":"鹿乃",
"url":"irony.mp3",
"pic":"irony.jpg"}]
}

{% endaplayer %}

``````

#### 插入视频

粘贴以下代码：

```
{% dplayer "url=https://player.bilibili.com/player.html?aid=82685934&cid=141472427&page=1" "pic=https://i0.hdslb.com/bfs/archive/1cd3e83b65ffc53a8b20178d0fff79dc638788f5.jpg" "loop=yes" "theme=#fadfa3" "autoplay=false" "token=tokendemo" %}

```
More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
