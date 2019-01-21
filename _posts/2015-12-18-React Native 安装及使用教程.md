---
layout:     post
title:     React Native 安装及使用教程
subtitle:   React Native安装
date:       2015-05-05
author:     黄鹏飞
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
- iOS
- 开源框架
---


[Facebook 对外宣布了正在开发的 React Native 框架](https://code.facebook.com/videos/786462671439502/react-js-conf-2015-keynote-introducing-react-native-/)，这个框架 可以让开发者人员 跨平台开发app 应用.目前只支持安卓和IOS
等等, 跨平台? 我们为什么要用react native ? H5做的不是很好吗?目前刚出来H5的很多框架,为什么不用H5而用react呢?
首先,可以基于 React Native使用 JavaScript 编写应用逻辑，UI 还是原生的UI ,但是,也是最重要的是 ,我们以后将没有必要和 HTML5 的 UI 做出常见的妥协. 因为react native 将会比H5更加的高效,项目越大效果越明显.
做过移动端的朋友可以发现,H5 虽然可以跨平台,一次编码,多次应用.但是web 毕竟是web, 手机的运存是有限的,不可能一次性加载太多的页面,这样会使造成大量的crash . 而且动画不明显(卡顿).
React 引入了一种与众不同的、略显激进但具备高可用性的方案来构建用户界面。长话短说，应用的 UI 简单通过一个基于应用目前状态的函数来表达。
homebrew 安装(推荐大家装,真的很好用,可以直接下载很多软件)
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
将下面两句话加到 ~/.bashrc or ~/.profile or ~/.zshrc 上.
export NVM*DIR="$HOME/.nvm" [ -s "$NVM*DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" # This loads nvm
如果找不到文件可以手动创建
touch ~/.profile
修改之后 不要忘记
source ~/.profile
安装 nvm
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.30.1/install.sh | bash
or Wget:
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.30.1/install.sh | bash
or brew:
brew install nvm
最新的5.0
nvm install 5.0
使用5.0
nvm use 5.0
or
nvm run 5.0 --version
or
nvm use 5.0
安装 watchman
brew install watchman
安装 flow
brew install flow
安装xcode
去appStore 官网下载 7.0+
quick Start
npm install -g react-native-cli$ react-native init XXX(创建的项目名称)
最后: 打开你的XXX项目 , 点击运行, Welcome to React Native!恭喜你,添加成功,这时候你就可以edit index.ios.jsPress Cmd+R to reload , Cmd +d or shake for dev menu 搞定!!!
