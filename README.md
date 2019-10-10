
博客的搭建教程修改自 [BY](https://github.com/qiubaiying/qiubaiying.github.io) 

>
### [查看博客戳这里 👆](http://serenaxxsun.github.io)



## 使用

* 开始
	* [环境](#环境)
	* [开始](#开始)
	* [撰写博文](#撰写博文)
* 组件
	* [侧边栏](#侧边栏)
	* [迷你关于我](#mini-about-me)
	* [推荐标签](#featured-tags)
	* [好友链接](#friends)



### 环境

如果你安装了 [jekyll](http://jekyllcn.com/)，那你只需要在命令行输入`jekyll serve` 或 `jekyll s`就能在本地浏览器中输入`http://127.0.0.1:4000/`预览主题，对主题的修改也能实时展示（需要强刷浏览器）。



### 开始

你可以通用修改 `_config.yml`文件来轻松的开始搭建自己的博客:

```
# Site settings
title: SERENA's Blog                    # 你的博客网站标题
SEOTitle: serena的博客		            # SEO 标题
description: "Hello Blog"	   	                # 随便说点，描述一下

# Build settings
# paginate: 10              # 一页你准备放几篇文章
```

Jekyll官方网站还有很多的参数可以调，比如设置文章的链接形式...网址在这里：[Jekyll - Official Site](http://jekyllrb.com/) 中文版的在这里：[Jekyll中文](http://jekyllcn.com/).

### 撰写博文

要发表的文章一般以 **Markdown** 的格式放在这里`_posts/`，你只要看看这篇模板里的文章你就立刻明白该如何设置。

### 侧边栏

设置是在 `_config.yml`文件里面的`Sidebar settings`那块。

```
# Sidebar settings
sidebar: true  #添加侧边栏
sidebar-about-description: "简单的描述一下你自己"
sidebar-avatar: /img/avatar-serena.jpg     #你的大头贴，请使用绝对地址.注意：名字区分大小写！后缀名也是
```

侧边栏是响应式布局的，当屏幕尺寸小于992px的时候，侧边栏就会移动到底部。具体请见bootstrap栅格系统 <http://v3.bootcss.com/css/>


### Mini About Me

Mini-About-Me 这个模块将在你的头像下面，展示你所有的社交账号。这个也是响应式布局，当屏幕变小时候，会将其移动到页面底部，只不过会稍微有点小变化，具体请看代码。

### Featured Tags

看到这个网站 [Medium](http://medium.com) 的推荐标签非常的炫酷，所以我将他加了进来。
这个模块现在是独立的，可以呈现在所有页面，包括主页和发表的每一篇文章标题的头上。

```
# Featured Tags
featured-tags: true  
featured-condition-size: 1     # A tag will be featured if the size of it is more than this condition value
```

唯一需要注意的是`featured-condition-size`: 如果一个标签的 SIZE，也就是使用该标签的文章数大于上面设定的条件值，这个标签就会在首页上被推荐。
 
内部有一个条件模板 `{% if tag[1].size > {{site.featured-condition-size}} %}` 是用来做筛选过滤的.

### Social-media Account

在下面输入的社交账号，没有的添加的不会显示在侧边框中。新加入了[简书](https:/www.jianshu.com)链接, <http://www.jianshu.com/u/e71990ada2fd>

	# SNS settings
	RSS: false
	jianshu_username: 	jianshu_id 
	zhihu_username:     username
	facebook_username:  username
	github_username:    username
	# weibo_username:   username
	
	

![](http://ww4.sinaimg.cn/large/006tKfTcgy1fgrgbgf77aj308i02v748.jpg)

### Friends

好友链接部分。这会在全部页面显示。

设置是在 `_config.yml`文件里面的`Friends`那块，自己加吧。

```
# Friends
friends: [
    {
        title: "Serena Blog",
        href: "https://serenaxxsun.github.io/"
    },
    {
        title: "Apple",
        href: "https://apple.com/"
    }
]
```

## 致谢

1. 这个模板是从这里 [BY](https://github.com/qiubaiying/qiubaiying.github.io) fork 的, 感谢这个作者。 
2. 感谢 Jekyll、Github Pages 和 Bootstrap!

## License

遵循 MIT 许可证。有关详细,请参阅 [LICENSE](https://github.com/serenaxxsun/serenaxxsun.github.io/blob/master/LICENSE)。

