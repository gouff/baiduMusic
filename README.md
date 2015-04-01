# baiduMusic
免费下载百度音乐无损歌曲

有些朋友可能在[百度音乐](http://music.baidu.com/)希望下载无损音乐，这需要百度白金VIP。可能网上有的教程有下载高品质音乐的方法：


**加入红心收藏，然后再下载** 

(参考:http://jingyan.baidu.com/article/870c6fc3365e84b03fe4bed4.html)

但对于无损音乐，

![vip](vip.png)

你还是无法下载。


## SAE上的演示
**已经部署在新浪 SAE **: http://bbmusic.sinaapp.com/ ，并参见[使用说明帮助](http://bbmusic.sinaapp.com/help.html)。


##介绍
本项目可以解决这一问题。

当然有三个前提：

- 该音乐有无损版本
- 已经登陆
- 加入了红心收藏


**已经部署在新浪 SAE **: http://bbmusic.sinaapp.com/  



主要代码在index.html的JS部分，很简单，就是一个**拼接字符串的过程**。如果你希望用户**免登陆，且不需要直接加入收藏，直接提供地址即可**，只需要一个**已知账号收收藏了足够多的音乐即可**。

##Future work

因为在百度音乐里面，我们实际上可得到这样的URL:

```
http://yinyueshiting.baidu.com/data2/music/124383622/124380645248400320.mp3?xcode=bb35db5d5dd35676c522735f06c5d744c9b81aee76f357c2
```

(这是《匆匆那年》320kbps超高音质的)

这样的URL不需要用户登录。
我们可以发现这个URL是始终生效的。即使我们把124380645248400320.mp3部分改成其他参数。

目前对Xcode的值了解得不够。作者发现混淆使用xcode的值有时可以凑效的。


我们可以设想，如果大家把一些信息能共享，就能构建一个庞大的音乐库。


有更多需求，欢迎Email联系，会考虑对其再次开发。

email : 18789482356@163.com

##版权问题
如果涉及版权问题，项目将立刻关闭。
