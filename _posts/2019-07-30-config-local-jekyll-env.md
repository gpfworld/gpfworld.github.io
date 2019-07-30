---
layout: post
title: "安装配置本地jekyll测试环境"
author: "GPF"
header-img: "img/post-bg-infinity.jpg"
header-mask: 0.3
mathjax: true
tags:
  - 计算机
  - 环境配置
---

jekyll依赖于Ruby，所有首先需要安装Ruby 和gem。

1、解决mac brew 安装很慢的问题，更改镜像源为清华源镜像
[https://my.oschina.net/Rayn/blog/2876725](https://my.oschina.net/Rayn/blog/2876725)
参考里说是替换两个，但是我只找到了一个

```
BREW_REPO = “https://github.com/Homebrew/brew“.freeze 
替换为
BREW_REPO = "https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git".freeze 
```

2、安装ruby
这里使用的是mac系统，因为系统已经有ruby和gem，但是这里最好重新安装，使用brew安装
brew install ruby

安装完后需要配置根据提示进行配置即可。

```
By default, binaries installed by gem will be placed into:
  /usr/local/lib/ruby/gems/2.6.0/bin

You may want to add this to your PATH.

ruby is keg-only, which means it was not symlinked into /usr/local,
because macOS already provides this software and installing another version in
parallel can cause all kinds of trouble.

If you need to have ruby first in your PATH run:
  echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc

For compilers to find ruby you may need to set:
  export LDFLAGS="-L/usr/local/opt/ruby/lib"
  export CPPFLAGS="-I/usr/local/opt/ruby/include"

For pkg-config to find ruby you may need to set:
  export PKG_CONFIG_PATH="/usr/local/opt/ruby/lib/pkgconfig"
```

3、更改ruby镜像源
[https://www.jianshu.com/p/879fdfa15ddf](https://www.jianshu.com/p/879fdfa15ddf)

```
#查看gem源
gem sources
#删除默认的gem源或者之前的tabao源
gem sources --remove https://rubygems.org/ 
#添加rubyChina作为gem源
gem sources -a https://gems.ruby-china.com
#查看当前gem源
gem sources
#确保只有ruby-china 源.
#清空源缓存
gem sources -c
#更新源缓存
gem sources -u
上述步骤执行完后，就可以进行ruby源安装了,此时会从rubyChina源下载gem文件
```

4、安装jekyll
gem install jekyll
配置路径，jekyll的路径
cd /usr/local/bin && ln -s /usr/local/lib/ruby/gems/2.6.0/bin/jekyll  jekyll

这样就可以使用jekyll的命令了。

5、Jekyll 常用的命令可参考官方文档

https://www.jekyll.com.cn/docs/usage/
