---
title: 一些mac端好用端插件分享
date: 2017-05-05 13:28:27
tags:
---
<div align="center">
想要生活变得更好？来看看这些插件吧！
</div>
![](http://osoa5juml.bkt.clouddn.com/image/site/1499949422354.png)
<!-- more -->



[TOC]



-----

# 百度云限速？试试Mac神器Aria2

<br/>
使用Tampermonkey插件 + “百度网盘直接下载助手”脚本（2017-03-20更新）

在Chrome上安装Tampermonkey插件。

安装“百度网盘直接下载助手”脚本。

# 会在百度云下载页面原来”下载”按钮旁边多出一个”下载助手”的按钮。



点击“直接下载”会使用浏览器默认下载器进行下载。点击“显示链接”，可复制链接放入aria2进行下载。

------

# 添加sitemap和feed插件
<br/>




切换到你本地的hexo，

```
npm install hexo-generator-feed -save
npm install hexo-generator-sitemap -save
```

修改_config.yml，增加以下内容

```
# ExtensionsPlugins:
- hexo-generator-feed
- hexo-generator-sitemap

 #Feed Atomfeed:
  type: atom
  path: atom.xml
  limit: 20#sitemapsitemap:
  path: sitemap.xml
```


再执行以下命令，部署服务端
hexo d -g

配完之后，就可以访问 https://gdutxiaoxu.github.io/atom.xml 和 https://gdutxiaoxu.github.io/sitemap.xml ，发现这两个文件已经成功生成了。









------

# 制作404页面

<br/>



{% codeblock  404.html lang:html  http://www.runoob.com/java/java-tutorial.html html%}<!DOCTYPE HTML>
<html>
<head>
  <meta http-equiv="content-type" content="text/html;charset=utf-8;"/>
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
  <meta name="robots" content="all" />
  <meta name="robots" content="index,follow"/>
</head>
<body>

<script type="text/javascript" src="http://www.qq.com/404/search_children.js" charset="utf-8" homePageUrl="your site url " homePageName="回到我的主页"></script>

</body>
</html>
{% endcodeblock  %}





# 其他一些好用的插件

{% blockquote %}
hexo可视化后台管理，很方便 - [hexo-hey](https://github.com/nihgwu/hexo-hey)  
在 hexo 中无痛使用本地图片 - [hexo-asset-image](https://github.com/CodeFalling/hexo-asset-image)
备份整个博客包括主题 - [hexo-git-backup](https://github.com/coneycode/hexo-git-backup)


{% endblockquote %}

