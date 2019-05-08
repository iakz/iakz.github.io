---
title: hexo设置个人域名
date: 2019-05-07 14:48:13
tags:
- hexo
comments: 
permalink:
categories:
- hexo
---
现在你的个人网站的地址是 yourname.github.io，如果觉得这个网址逼格不太够，这就需要你设置个人域名了。但是需要花钱。

注册一个阿里云账户,在阿里云上买一个域名，我买的是 fangzh.top，各个后缀的价格不太一样，比如最广泛的.com就比较贵，看个人喜好咯。

你需要先去进行实名认证,然后在域名控制台中，看到你购买的域名。

点解析进去，添加解析。

其中，192.30.252.153 和 192.30.252.154 是GitHub的服务器地址。
注意，解析线路选择默认，不要像我一样选境外。这个境外是后面来做国内外分流用的,在后面的博客中会讲到。记得现在选择默认！！

登录GitHub，进入之前创建的仓库，点击settings，设置Custom domain，输入你的域名fangzh.top

然后在你的博客文件source中创建一个名为CNAME文件，不要后缀。写上你的域名。

最后，在gitbash中，输入

hexo clean
hexo g
hexo d
过不了多久，再打开你的浏览器，输入你自己的域名，就可以看到搭建的网站啦！

接下来你就可以正式开始写文章了。

hexo new newpapername
然后在source/_post中打开markdown文件，就可以开始编辑了。当你写完的时候，再

hexo clean
hexo g
hexo d
就可以看到更新了。
