---
layout: post
title: "Install a new mac develop everment"
description: "每次重装电脑或者升级新装备后，配一台自己熟悉的开发环境都麻烦，本文的内容都是自己平常使用的一些工具安装配置方法，同时我也会不定期更新。"
tags: [android]
---


## Chrome  plugin
 
- [Octotree chrome 插件 github目录树](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc)

- [chromium-vim cVim](https://github.com/1995eaton/chromium-vim)

## Shadowsocks 

- [bandwagonhost](https://bandwagonhost.com/)
- [shadowsocks for Mac](https://github.com/shadowsocks/shadowsocks-iOS/releases)

## home brew

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## iTerm2

[Download iTerm2](http://www.iterm2.cn/download) 

or 

```
brew cask install iterm2
```

## zsh

```
brew install zsh
```

## oh-my-zsh

```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```


oh-my-zsh 这货可以装插件 

```
$ vim .zshrc
```

定位到如下行，括号里填入你要安装的插件 

```
plugins=(git z sublime)
```

来这里找找你想要的插件，没有的话可以自己动手写一个

(oh-my-zsh/wiki/Plugins)[https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins]

## MacDown

```
brew cask install macdown
```

## Java

```
brew cask install java
```

如果你需要安装 JDK 7 或者 JDK 6，可以使用homebrew-cask-versions：

```
brew tap caskroom/versions
brew cask install java6
```

## cheat 

```
$ cd
$ git clone https:/github.com/andyiac/cheat .cheat
$ vim .zshrc
```

set EDITOR 

```
export EDITOR="/usr/bin/vim"
```

## Android SDK

```
export PATH=${PATH}:/Users/xxxx/Library/Android/sdk/platform-tools
export PATH=${PATH}:/Users/xxxx/Library/Android/sdk/tools
```

## Genymotion 

[Genymotion Download url](http://files2.genymotion.com/genymotion/genymotion-2.5.2/genymotion-2.5.2.dmg)

## Install git flow 

```
brew install git-flow
```

## IRC shout

[shout](https://github.com/erming/shout)

## keycastr
show key click on keyboard
[keycastr](https://github.com/keycastr/keycastr)


## ssh-keygen

注意先切换到 .ssh 目录下，执行 ssh-keygen 命令

```
➜  cd
➜  cd .ssh
➜  .ssh ssh-keygen
➜  .ssh cat github_rsa.pub | pbcopy 
```


---


## links
- [awesome mac](https://github.com/jaywcjlove/awesome-mac)
- [GitHub ocds-guide-to-setting-up-mac](https://github.com/macdao/ocds-guide-to-setting-up-mac)


---

基于以上内容可以写个脚本啦

2015-11-30 15:31
