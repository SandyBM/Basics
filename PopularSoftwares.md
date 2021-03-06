#常用软件列表

#网络应用

## 网络浏览器

### Chrome

**介绍**：可能是世界上最好的浏览器

**下载位置**：

[Download](http://www.google.cn/intl/zh-CN/chrome/browser/)

**安装方法**：

    wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
    sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
    sudo apt-get update
    sudo apt-get install google-chrome-stable

**卸载方法**：

    sudo apt-get purge google-chrome-stable
    sudo rm -rf /etc/apt/sources.list.d/google.list'

### Firefox

**介绍**：自由、拓展性强大的浏览器

**下载位置**：

[Download](http://www.firefox.com.cn/download/)

[PPA ubuntu-mozilla-daily](https://code.launchpad.net/~ubuntu-mozilla-daily/+archive/ubuntu/ppa)

**安装方法**：

    # 1. Firefox
    sudo apt-get install firefox firefox-locale-zh-hans

    # 2. Firefox PPA
    sudo add-apt-repository ppa:ubuntu-mozilla-daily/ppa
    sudo apt-get update
    sudo apt-get install firefox-trunk

**卸载方法**：

    # 1. Firefox
    sudo apt-get purge firefox firefox-locale-zh-hans

    # 2. Firefox PPA
    sudo add-apt-repository -r ppa:ubuntu-mozilla-daily/ppa
    sudo apt-get update

**备注**：

如果你是Debian或Kali，你的系统自带的浏览器不是Firefox，而是Iceweasel。

### Iceweasel

**介绍**：Iceweasel是一个网络浏览器，是Mozilla Firefox浏览器的Debian再发布版。

**下载位置**：

[Download](https://packages.debian.org/sid/iceweasel)

**安装方法**：

    sudo apt-get install iceweasel

**卸载方法**：

    sudo apt-get purge iceweasel

### Chromium

**介绍**：Chrome浏览器的开源版本

**下载位置**：

[Download](http://www.chromium.org/getting-involved/download-chromium)

[PPA chromium-daily](https://launchpad.net/~chromium-daily/+archive/ubuntu/stable)

**安装方法** ：

    # 1. Chromium
    sudo apt-get install chromium

    # 2. Chromium PPA
    sudo add-apt-repository  ppa:chromium-daily/stable  #
    sudo apt-get update
    sudo apt-get install chromium-browser

**卸载方法**：

    # 1. Chromium
    sudo apt-get purge chromium

    # 2. Chromium PPA
    sudo add-apt-repository -r ppa:chromium-daily/stable  #
    sudo apt-get update

### Maxthon

**介绍**：功能丰富、界面简洁的浏览器

**下载位置**：

[Download](http://www.maxthon.cn/)

**安装方法**：

    sudo gdebi maxthon-browser-stable_1.0.5.3_amd64.deb

**卸载方法**：

    sudo dpkg -r maxthon-browser-stable

### Opera

**介绍**：来自挪威的浏览器

**下载位置**：

[Download](http://www.opera.com/computer/linux)

**安装方法**：

	# 1. Add source in /etc/apt/sources.list
	sudo add-apt-repository 'deb https://deb.opera.com/opera-stable/ stable non-free'
    wget -qO- https://deb.opera.com/archive.key | sudo apt-key add -
    sudo apt-get update
	sudo apt-get install opera-stable

	# 2. Add source in /etc/apt/sources.list.d/opera.list
    sudo sh -c 'echo "deb https://deb.opera.com/opera-stable/ stable non-free" >> /etc/apt/sources.list.d/opera.list'
    wget -qO- https://deb.opera.com/archive.key | sudo apt-key add -
    sudo apt-get update
	sudo apt-get install opera-stable

**卸载方法**：

    # 1. Add source in /etc/apt/sources.list
	sudo apt-get purge opera-stable
	sudo add-apt-repository -r 'deb https://deb.opera.com/opera-stable/ stable non-free'
    sudo apt-get update


	# 2. Add source in /etc/apt/sources.list.d/opera.list
	sudo apt-get purge opera-stable
    sudo rm -rf /etc/apt/sources.list.d/opera.list
    sudo apt-get update

## 邮件客户端

### Thunderbird

**介绍** : 专注于电子邮件管理的强大邮件客户端

**下载位置**：

[Download](https://www.mozilla.org/zh-CN/thunderbird/)

**安装方法**：

    # 1. Thunderbird
    sudo apt-get install thunderbird

    # 2. Thunderbird PPA
    sudo add-apt-repository ppa:ubuntu-mozilla-daily/ppa
    sudo apt-get update
    sudo apt-get install thunderbird-trunk

**卸载方法**：

    # 1. Thunderbird
    sudo apt-get purge thunderbird

    # 2. Thunderbird PPA
    sudo add-apt-repository -r ppa:ubuntu-mozilla-daily/ppa
    sudo apt-get update

**备注**：
如果你是Debian或Kali，你的系统默认的邮件客户端不是Thunderbird，而是Icedove。

### Icedove

**介绍**：Icedove是一个邮件客户端，是Mozilla Thunderbird客户端的Debian再发布版。

**下载位置**：

[Download](https://packages.debian.org/sid/icedove)

**安装方法**：

    sudo apt-get install icedove

**卸载方法**：

    sudo apt-get purge icedove

### Evolution

**介绍**：提供邮件收发、日历和通讯录的个人信息解决方案

**下载位置**：

[Download](https://wiki.gnome.org/Apps/Evolution)

**安装方法**：

    sudo apt-get install evolution

**卸载方法**：

    sudo apt-get purge evolution

### Mutt

**介绍**：类Unix系统下基于文本的邮件客户端

**下载位置**：

[Download](http://www.mutt.org/)

**安装方法**：

    sudo apt-get install mutt

**卸载方法**：

    sudo apt-get install mutt

## 即时聊天

###QQ

**介绍**：支持在线聊天、视频电话、点对点断点续传文件的强大聊天软件。

**安装方法**:

	暂缺。。。

### Skype

**介绍**：最清晰的免费网络电话，提供文字、声音和视频聊天。

**下载位置**：

[Download CN](http://skype.gmw.cn/)  
[Download EN](http://www.skype.com/)  
[Download DEB](http://archive.canonical.com/pool/partner/s/skype/)

**安装方法**：

    # Ubuntu，LinuxMint
    sudo apt-get install skype

	# Debian : downloading from Download DEB,save it as skype.deb
    sudo gdebi skype.deb

**卸载方法**：

    # Ubuntu,LinuxMint
    sudo apt-get purge skype

    # Debian
    sudo dpkg -r skype

**备注**：
skype来自于 Ubuntu partner库。  
对于Ubuntu，这个库是默认安装的，所以可以直接install和purge的;  
对于LinuxMint，默认使用Ubuntu partner库，所以也是可以直接install和purge的;  
对于Debian来说，最简单的安装方法就是使用下载的deb包。关于复杂的安装方法，我会在后面进行介绍。

### Empathy

**介绍**：支持多协议的强大聊天软件。

**下载位置**：

[Download](https://wiki.gnome.org/action/show/Apps/Empathy?action=show&redirect=Empathy)

[Github Empathy](https://github.com/GNOME/empathy)

**安装方法**：

    sudo apt-get install empathy

**卸载方法**：

    sudo apt-get purge empathy

### Pidgin

**介绍**：跨平台、支持多种协议的聊天软件。

**下载位置**：

[Download](https://pidgin.im/download/linux/)

**安装方法**：

    sudo apt-get install pidgin

**卸载方法**：

    sudo apt-get purge pidgin

### XChat

**介绍** :跨平台的IRC聊天软件。

**下载位置** : 

[Download](http://xchat.org/download/)

**安装方法**：

	sudo apt-get install xchat

**卸载方法**：

	sudo apt-get purge xchat

### 阿里旺旺

**介绍**：原为阿里内部使用的聊天软件。网盘在外国，访问速度非常慢

**下载位置**：

[Download](http://ge.tt/8sPpGIA)

**安装方法**：

    sudo gdebi aliwangwang_1.00-00_amd64.deb

**卸载方法**：

    sudo dpkg -r aliwangwang

## 文件传输

### XwareDesktop

**介绍**：迅雷在Linux上的原生开源方案

**下载位置**：

[Download](https://github.com/Xinkai/XwareDesktop)

**安装方法**：

    源码编译

### FlareGet

**介绍**：支持多协议，多线程的下载软件。

**下载位置**：

[Download](https://flareget.com/download)

**安装方法**：

    sudo gdebi flareget_4.3-95_amd64.deb

**卸载方法**：

    sudo dpkg -r flareget

### UGet

**介绍**：轻量级的全能下载管理器

**下载位置**：

[Download](http://ugetdm.com/downloads)

**安装方法**：

    sudo apt-get install transmission

**卸载方法**：

    sudo apt-get purge transmission

### Wget

**介绍**：运行在命令行下的多协议下载软件

**下载位置**：

[Download](http://www.gnu.org/software/wget/)

**安装方法**：

    sudo apt-get install wget

**卸载方法**：

    sudo apt-get purge wget

### Transmission

**介绍**：一种BitTorrent客户端，特点是一个跨平台的后端和其上的简洁的用户界面

**下载位置**：

[Download](http://www.transmissionbt.com/download/)

**安装方法**：

    sudo apt-get install transmission

**卸载方法**：

    sudo apt-get purge transmission

### Aria2

**介绍**：运行在命令行下的轻量级下载软件

**下载位置**：

[Download](http://sourceforge.net/projects/aria2/files/stable/aria2-1.15.2/)

**安装方法**：

    sudo apt-get install aria2

**卸载方法**：

    sudo apt-get purge aria2

### Filezilla

**介绍**：免费、开源的最强FTP客户端软件

**下载位置**：

[Download](https://filezilla-project.org/)

**安装方法**：

    sudo apt-get install filezilla

**卸载方法**：

    sudo apt-get purge filezilla

## 云存储

### bcloud

百度网盘的linux桌面客户端  
[bcloud源码](https://github.com/LiuLang/bcloud)  
[bcloud安装包](https://github.com/LiuLang/bcloud-packages)

##网络支付

## 视频软件

# 图像影音

## 音乐播放

### kwplayer

酷我音乐盒的linux客户端  
[kwplayer源码](https://github.com/LiuLang/kwplayer)  
[kwplayer安装包](https://github.com/LiuLang/kwplayer-packages)

### FeelUOwn

网易云音乐的linux客户端 [FeelUOwn源码](https://github.com/cosven/FeelUOwn)  

## 视频播放

### SMPlayer

**介绍**：一个基于mplayer2的视频播放器，可能是Linux下最方便的视频播放器。

**下载位置**：

[Download](http://smplayer.sourceforge.net/)

**安装方法**：

    sudo apt-get install smplayer

**卸载方法**：

    sudo apt-get purge smplayer

### VLC

**介绍**：全平台的自由多媒体解决方案。

**官方网站**：

[Official website](http://www.videolan.org/)

**安装方法**：

    sudo apt-get install vlc

**卸载方法**：

    sudo apt-get purge vlc

### mpv

**介绍**：专注与视频播放质量和体验。GUI？我们不需要，配置文件更高效。

**官方网站**：

[Official website](https://mpv.io/)
[GitHub](https://github.com/mpv-player/mpv)

**安装方法**：

    sudo apt-get install mpv

**卸载方法**：

    sudo apt-get purge mpv

### KODI(原XBMC)

**介绍**：全平台的媒体库解决方案，插件丰富是它的最大特点。

**下载位置**：

[Download](http://kodi.tv/download/)  

**安装方法**：

    sudo apt-get install software-properties-common
    sudo add-apt-repository ppa:team-xbmc/ppa
    sudo apt-get update
    sudo apt-get install kodi

**卸载方法**：

    sudo apt-get purge kodi
    
**中文插件**：
    [xbmc-addons-chinese](https://github.com/taxigps/xbmc-addons-chinese)

## 图像浏览

# 游戏娱乐

## 游戏平台

## 小游戏

### gnome-2048

gnome 2048 小游戏

# 文件管理

## 文件管理

## 压缩打包

# 办公应用

## 输入法

### fcitx + (sunpinyin, googlepinyin, sogoupinyin)

## 文档阅读

## 办公套件

## 笔记记事

### Google Keep
记事和清单

### WizNote

为知笔记 [linux版源代码](https://github.com/WizTeam/WizQTClient)

# 教育科学

## 教育软件

## 科学软件

# 虚拟化

## 虚拟机

# 监视和控制

## 硬件查询

## 系统监视

## 系统安全

## 远程控制

# 系统工具

## 终端模拟器

linux 的终端就是控制台，是用户与内核交互的平台，通过输入指令来控制内核完成任务操作。

### Gnome Terminal
 
**介绍**：Gnome Terminal 是 Gnome 桌面环境中的终端模拟软件。

**官方网站**：

[Official Website](https://help.gnome.org/users/gnome-terminal/stable/index.html.en)
[GitHub](https://github.com/GNOME/gnome-terminal)

**安装方法**：

    sudo apt-get install gnome-terminal

**卸载方法**：

    sudo apt-get purge gnome-terminal

### Terminator

**介绍**：Terminator 是一个程序，它可让用户自由地排布多个 GNOME 终端，而不用通过窗口管理器来实现，比较适合需要同时打开多个终端的用户。

**官方网站**：

[Official Website](http://gnometerminator.blogspot.com/p/introduction.html)

**安装方法**：

    sudo apt-get install terminator

**卸载方法**：

    sudo apt-get purge terminator

### tmux

**介绍**：GNU screen 类似的程序，可作为后者的替代品使用。

**官方网站**：

[Official Website](http://sourceforge.net/projects/tmux/)

**安装方法**：

    sudo apt-get install tmux

**卸载方法**：

    sudo apt-get purge tmux

## Shell

# 系统管理

## 配置工具

### Tweak Tool

# 程序开发

## 版本控制

## 本文编辑器

### Sublime Text

## 集成开发环境
