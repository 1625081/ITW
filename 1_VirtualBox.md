### 1_虚拟机环境

> 本教程执行过程中如果遇到网络问题，建议连接自己或者公用的VPN

#### Ubuntu 简介

Ubuntu 是一个基于 Debian 的 GNU/Linux 操作系统，
支持 X86 、64以及 PPC 架构。
Ubuntu 每隔六个月发布一个版本，即每年的四月和十月，本文使用的是
 16.04 64-bit 版本。
 Ubuntu 对于新手应该是比较友好的一个 Linux 发行版，中文本地化也做的不错，
 有开箱即用的感觉。因为 Ubuntu 近几年用户群的增加，多了很多对于新手有用的资料，
 因此不用担心遇到问题无法解决，善用搜索和提问，将使你更快速地成长。

#### 环境预设
- Windows 64-bit
- [VirtualBox5.1](https://www.virtualbox.org/)
- Ubuntu 16.04 amd64 (64-bit) ISO
[网易下载](http://mirrors.163.com/ubuntu-releases/16.04/ubuntu-16.04.3-desktop-amd64.iso)

> 如果配置较低，如32位系统，可以选择[i386](http://mirrors.163.com/ubuntu-releases/16.04)

#### Ubuntu安装

`1.` 新建与加载碟片

当你安装完 VirtualBox 后，打开你应该会看到下面这样的界面

![alt](http://www.linuxidc.com/upload/2015_08/15081716378668.png)

点击新建后会出来如下图所示的界面，一般如图填写即可，内存可酌情填写

![](http://www.linuxidc.com/upload/2015_08/15081716377585.png)

下一步将创建虚拟硬盘，如图所示，默认位置为 C 盘，
如果你不想在 C 盘创建，或者C盘空间不足，请确保你选择的盘格式为NTFS

![](http://www.linuxidc.com/upload/2015_08/15081716375635.png)

![](http://ofnfnmmn0.bkt.clouddn.com/lecture_1/1.PNG)

创建完成后，请点 设置 如图加载 ISO 文件

![](http://www.linuxidc.com/upload/2015_08/15081716378797.png)

为了防止出现无法上网的BUG，建议如下配置自己的虚拟机，
当然，界面名称和芯片根据不同电脑会有不同

![](http://ofnfnmmn0.bkt.clouddn.com/lecture_1/2.PNG)

`2.` 安装Ubuntu

点击启动 ，会开机，进入如下界面

![](http://www.linuxidc.com/upload/2015_08/15081716386045.png)

开始安装

![](http://www.linuxidc.com/upload/2015_08/15081716384749.png)

这里请注意，本教程使用虚拟机，强烈建议选择 **清除整个磁盘并安装 Ubuntu** ，
但如果你之后打算装到实体机与 Windows 形成双系统时，请选择 其他选项 ，这要求你对 Linxu 有一定的了解且具备一定的基础进行分区操作，注意不要覆盖 Windows 的 C 盘，此处由于篇幅原因，不再详述。

![](http://www.linuxidc.com/upload/2015_08/15081716407202.png)

如图，进行用户设定，计算机名 是主机名，用户名 是登录时用的账户名称，密码 则是你所设 用户名 的登录密码，请务必记牢。

![](http://www.linuxidc.com/upload/2015_08/15081716402366.png)

这一步之后会选择时区，直接点下一步即可，键盘选择如下图

![](http://www.linuxidc.com/upload/2015_08/15081716404109.png)

配置选择已完成，接下来请耐心等待安装过程，如图，请不要点击 SKIP

![](http://www.linuxidc.com/upload/2015_08/15081716407283.png)

耐心等待安装完成，然后会重启进入系统，用你上面配置的用户名和密码登录，请注意最好不要登录 root ，你可以用 sudo 命令来获取相应的权限，下图是展示成果：

![](http://www.linuxidc.com/upload/2015_08/15081716412607.png)

BUG List：
1. 64-bit电脑强制建立32-bit虚拟机

[解决VirtualBox只能安装32位系统的问题](http://www.cnblogs.com/52php/p/5677864.html)

#### Ruby环境
Ruby is...
A dynamic, open source programming language with a focus on simplicity and productivity. It has an elegant syntax that is natural to read and easy to write.

**Ruby 安装**

RVM 是一个命令行工具，可以提供一个便捷的多版本 Ruby 环境的管理和切换。

https://rvm.io/

如果你打算学习 Ruby / Rails, RVM 是必不可少的工具之一。

这里所有的命令都是再用户权限下操作的，任何命令最好都不要用 sudo.

```bash
$ gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
$ \curl -sSL https://get.rvm.io | bash -s stable
$ source ~/.bashrc
$ source ~/.bash_profile
```
修改 RVM 的 Ruby 安装源到 Ruby China 的 Ruby 镜像服务器，这样能提高安装速度
```bash
$ echo "ruby_url=https://cache.ruby-china.org/pub/ruby" > ~/.rvm/user/db
```

列出已知版本：

```bash
rvm list known
```
安装一个 Ruby 版本
```bash
rvm install 2.2.2
```
切换 Ruby 版本
```bash
rvm use 2.2.2
```
如果想设置为默认版本，这样一来以后新打开的控制台默认的 Ruby 就是这个版本
```bash
rvm use 2.2.2 --default
```
查询已经安装的ruby
```bash
rvm list
```
卸载一个已安装版本
```bash
rvm remove 1.8.7
```

有关Nginx的内容，以后会讲到，不过这里讲的略简单，故也不做要求。
作为选做作业，大家可以自行查看：[rvm使用教程](https://ruby-china.org/wiki/rvm-guide)

可以通过`ruby -v 和 rvm -v`查看是否安装成功，如果没有成功，可以按照下列步骤补救一下：

在终端->右键->配置文件->命令->以登陆shell方式运行命令

**Ruby On Rails安装（作业）**

在此之前，请先按照教程更新一下[gem源](https://gems.ruby-china.org/)

```bash
$ gem install rails
```
