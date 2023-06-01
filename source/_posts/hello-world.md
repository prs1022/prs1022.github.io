---
title: Hello World
categories:
- Hexo
tags:
- 首篇文章
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).
更多主题可以在 [hexo主题](https://hexo.io/themes/)中找到，个人喜欢简洁风格，所以当前博客主题用的是[next](https://theme-next.js.org/),修改主题的方法我放在下面了。


## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### 修改主题

找到对应主题的github地址

``` bash
git clone https://github.com/next-theme/hexo-theme-next themes/next
```
执行后next主题会放在themes目录下；

打开 Hexo配置文件_config.yml 修改 theme变量为 next

``` bash
theme: next
```

一般主题一个月会更新一次，所以想要体验最新主题，可以cd 到next目录下，git pull即可。

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

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)


