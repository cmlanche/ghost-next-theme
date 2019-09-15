# Ghost-Next-Theme

我此前的个人博客cmlanche.com是用hexo next主题制作的，但由于要写博客特别依赖本地环境，也就是说没有我本地那个电脑发布文章是不可能的，另外我也想围绕ghost生态做点事情（就是写写主题等），同时基于对next简洁风格的喜爱，我重写了ghost版本。

### 效果

##### 首页

![screenshot-desktop_meitu_1](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/x4xwm.jpg)

##### 作者页面

![WX20190915-133947@2x_meitu_2](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/je9br.jpg)

##### 标签页

![WX20190915-134119@2x_meitu_3](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/cish9.jpg)

##### 文章页

左侧是作者的基本信息，包含一个头像、标题还有个人描述，还有3个链接，分别是个人网站链接、微信和微博主页。

![WX20190915-134249@2x_meitu_4](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/36r5i.jpg)

​	微信是鼠标放在logo上就回出现微信二维码，可以让别人扫码添加好友。

![WX20190915-134534@2x_meitu_5](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/rlbab.jpg)

### 如何使用

##### 下载主题

ghost主题使用很简单，不需要编译啥的，直接下载源码zip包上传到ghost后台就行，我已经[release版本](https://github.com/cmlanche/ghost-next-theme/releases)了，可以去这里下载。

##### 上传主题

打开你的ghost网站的后台，找到【Design】-【Upload a theme】，如下图，然后上传下载的zip主题包，然后点击Active激活。

![WX20190915-135029@2x_meitu_6](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/fx6lz.jpg)

##### 设置（可选）

1. 设置微信、微博相关信息

如果你想让你的微信和微博生效，那么在ghost后台的【Code injection】-【Site Header】中添加如下代码：

```javascript
<script>
this.theme = {
	"cmlanche": {
		"weixin": "https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/weh85.png",
		"weibo": "https://www.weibo.com/574811002"
	}
}
</script>
```

> todo：其中cmlanche暂时写死的，你不用改成你的用户名，之后更新版本会修改这一点，因为一个ghost博客是支持多用户的，不同的用户可以配置不同的微信微博信息。

2. 设置个人相关信息

找到【Staff】，在列表中找到你的用户，编辑即可。

![WX20190915-135855@2x_meitu_7](https://indiehackers-1251406926.cos.ap-chengdu.myqcloud.com/hackers/lxq1r.jpg)