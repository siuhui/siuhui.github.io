---
title: "Hello World"
date: 2024-09-02T17:11:13+08:00
draft: false
tags: ["blog"]
# description: ""
showToc: false
TocOpen: false
hidemeta: false
hideSummary: false
canonicalURL: "https://siuhui.github.io/post/hello-world"
searchHidden: false
ShowReadingTime: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
cover:
    image: "" # image path/url
    alt: "" # alt text
    caption: "" # display caption under cover
    hidden: false # only hide on current single page
---

重建了博客，用的还是 [hugo](https://gohugo.io/)，主题还是 [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 。原来还想着自己写主题的，但是现在看来，在之后很长的一段时间都不会去做了，暂时也不会花太多时间学习前端。

<!--more-->

放一张之前的博客图片纪念一下😃
![old-blog](/images/old-blog.png)

之前的博客是用 hugo 生成静态网页后，再把生成的文件夹（public）里的内容上传到 Github 仓库进行部署的，感觉这个流程挺麻烦的，而且主题的配置文件和 md 文件没有用 git 来管理，这不是一个好的流程。现在这个只需要写 md 文件，推送到仓库，Github Action 自动使用 hugo 生成静态网页并部署，这个流程应该才是人们常用的，在 Github 上看到一些仓库也是这样的。

目前博客的图片是直接放在 Github 仓库里的，加载可能会比较慢，本来想搞下 Cloudflare R2 来做图床的，但是银行卡没有验证成功，暂时就先这样吧，看的人应该也不多，加了 google analytics，之后可以看看访问量。

之前的博客没怎么用起来，没写过什么东西，希望现在这个不要过于闲置。😇

### 记录一下遇到的问题和解决方法以及对主题做的修改

**WordCount 字数统计不支持中文：**

这个是 hugo 配置导致的问题，hugo 默认认为内容是英文，在配置文件中加 `hasCJKLanguage: true` 即可解决。

**不支持 LaTex：**

抄了[这个教程](https://kiwamizamurai.github.io/posts/2022-03-06/)

**导行栏菜单改成了响应式的：**

手机上，导航栏菜单一行排不下，放到第二排去了，看着不怎么顺眼，所以就改成响应式的了，屏幕小的话菜单就收起来。

参考了[这个仓库](https://github.com/solamarpreet/PaperMod-Responsive)
