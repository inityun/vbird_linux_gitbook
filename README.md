# 目录及概述

这本书的所有内容是学习Linux的基础，这些内容是基础中的基础，如果您能将其中的文字都看完并且消化过，那么未来在管理 Linux主机以及架设网站方面，就能够达到“事半功倍”的成效，请不要忽略这些内容了！否则，再怎么讨论都是枉然的啦！^\_^。 Linux的资料非常的多，每份资料彼此的相关性都很强，要单独的一项一项讲解并不容易， 那么这本书件该怎么看呢？建议先按照顺序将内容大致浏览过一次，看不懂的地方也可以先略过不要紧。 全部看完之后，再从头开始“仔细”的实际操作过一遍，那应该就能够进入Linux的世界啰～

另外，每个章节下面的日期，指的是重大改版日期而非最新日期，最新日期请以该章节结束部分的工作日志为主的喔！


> [!NOTE]
> 此项目是基于gitbook创建的, 但是没有gitbook的相关插件和配置文件, 只有最基础的内容md文件   
> 此项目中所有的md文件来源都是pdf版本转换过来, 难免有错误的地方, 可fork项目后自行更改, 要是顺带告知下我是最佳  


## 第一部分 Linux 的规划与安装


常常听到Linux具有非常优良的血统，所以具有相当良好的多用户多任务环境，可以方便程序设计师来开发软件。 此外，Linux本身是不用钱的“自由软件”，使用上面并没有所谓的“盗版”问题。但是，为什么Linux不用钱？ 随便修改或发布Linux为什么不会被罚？为什么Linux有这么多的版本？包括Fedora, SuSE, CentOS, Debian等等？ 这个都是我们必须要来了解的部分！了解这些部分，你才会对Linux有一个正确的理解，才能够跟你的同事、同学、 上司说明，为什么使用Linux具有很多优点与好处！ ^\_^
Linux并不好学习，鸟哥也是“重伤”过好几次才能对Linux有一些基础的认知。那么到底应该如何学习Linux呢？关键在实作。 既然要实作就得要实际的安装一部Linux，那么Linux要安装前需要熟悉哪些基础观念？计算机概论是非常重要的一环！ 因为Linux与硬件的关系还不小～此外，打造一台Windows/Linux共存的主机也是很有用的， 至少对于需要多平台但又缺乏空间与金钱的朋友来说，这样的处理是非常有用的！

在第一篇里面，我们会由计算机概论谈起，再讲到Linux的历史渊源与自由软件的关系，然后重点在于如何规划硬件与Linux安装， 最后谈到如何登陆与使用Linux图形/命令行的环境。本篇数据较多，第一次接触Linux的新朋友， 很多数据若看不懂可以先略过，等到后续文章都读完了再回来看，才会有帮助喔！ ^\_^

### 第零章 计算机概论

鸟哥在大专院校的教学经验中发现到，由于对 Linux 有兴趣的朋友很多可能并非信息相关专业出身， 因此对于计算机硬件及计算机方面的概念不熟。然而操作系统这种咚咚跟硬件.....2015/04/16

-   [0.1 电脑：辅助人脑的好工具](/chapter_0/0.1电脑-辅助人脑的好工具.md)
    -   [0.1.1 计算机硬件的五大单元](/chapter_0/0.1电脑-辅助人脑的好工具.md)
    -   [0.1.2 一切设计的起点：CPU 的架构, RISC与ARM, CISC与x86](/chapter_0/0.1电脑-辅助人脑的好工具.md)
    -   [0.1.3 其他单元的设备](/chapter_0/0.1电脑-辅助人脑的好工具.md)
    -   [0.1.4 运行流程](/chapter_0/0.1电脑-辅助人脑的好工具.md)
    -   [0.1.5 电脑按用途分类](/chapter_0/0.1电脑-辅助人脑的好工具.md)
    -   [0.1.6 电脑上面常用的计算单位 （容量、速度等）](/chapter_0/0.1电脑-辅助人脑的好工具.md)
-   [0.2 个人电脑架构与相关设备元件](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.1 执行脑袋运算与判断的 CPU：CPU的工作频率,32位与64位,CPU等级, 超线程](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.2 内存：多通道, DRAM与SRAM, ROM](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.3 显卡：PCIe 规格](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.4 硬盘与储存设备：物理组成,盘片与扇区,传输接口（SATA,SAS,USB..）,SSD,购买与运行](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.5 扩展卡与接口](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.6 主板](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.7 电源供应器](/chapter_0/0.2个人电脑架构与相关设备元件.md)
    -   [0.2.8 选购须知](/chapter_0/0.2个人电脑架构与相关设备元件.md)
-   [0.3 数据表示方式](chapter_0/0.3数据表示方式.md)
    -   [0.3.1 数字系统](chapter_0/0.3数据表示方式.md)
    -   [0.3.2 文字编码系统](chapter_0/0.3数据表示方式.md)
-   [0.4 软件程序运行](chapter_0/0.4软件程序运行.md)
    -   [0.4.1 机器程序与编译程序](chapter_0/0.4软件程序运行.md)
    -   [0.4.2 操作系统](chapter_0/0.4软件程序运行.md)
    -   [0.4.3 应用程序](chapter_0/0.4软件程序运行.md)
-   [0.5 重点回顾](chapter_0/0.5重点回顾.md)
-   [0.6 本章习题](chapter_0/0.6本章习题.md)
-   [0.7 参考资料与延伸阅读](chapter_0/0.7参考资料与延伸阅读.md)

### 第一章 Linux是什么/如何学习

众所皆知的，Linux的核心原型是1991年由托瓦兹（Linus Torvalds）写出来的，但是托瓦兹为何可以写出Linux这个操作系统？ 为什么他要选择386的计算机来开发？为什么Linux的发展可以这么迅速？又为什么Linux是免费的？.....2015/04/23

-   [1.1 Linux是什么](chapter_1/1.1Linux是什么.md)
    -   [1.1.1 Linux是什么？操作系统/应用程序？](chapter_1/1.1Linux是什么.md)
    -   [1.1.2 Linux之前，Unix的历史](chapter_1/1.1Linux是什么.md)
    -   [1.1.3 关于GNU计划、自由软件与开放源代码](chapter_1/1.1Linux是什么.md)
-   [1.2 Torvalds的Linux发展](chapter_1/1.2Torvalds的Linux发展.md)
    -   [1.2.1 与Minix之间](chapter_1/1.2Torvalds的Linux发展.md)
    -   [1.2.2 对386硬件的多任务测试](chapter_1/1.2Torvalds的Linux发展.md)
    -   [1.2.3 初次释出Linux 0.02](chapter_1/1.2Torvalds的Linux发展.md)
    -   [1.2.4 Linux的发展：虚拟团队的产生](chapter_1/1.2Torvalds的Linux发展.md)
    -   [1.2.5 Linux 的核心版本](chapter_1/1.2Torvalds的Linux发展.md)
    -   [1.2.6 Linux distributions](chapter_1/1.2Torvalds的Linux发展.md)
-   [1.3 Linux当前应用的角色](chapter_1/1.3Linux当前应用的角色.md)
    -   [1.3.1 企业环境的利用](chapter_1/1.3Linux当前应用的角色.md)
    -   [1.3.2 个人环境的使用](chapter_1/1.3Linux当前应用的角色.md)
    -   [1.3.3 云端运用](chapter_1/1.3Linux当前应用的角色.md)
-   [1.4 Linux 该如何学习](chapter_1/1.4Linux该如何学习.md)
    -   [1.4.1 从头学习Linux基础](chapter_1/1.4Linux该如何学习.md)
    -   [1.4.2 选择一本易读的工具书](chapter_1/1.4Linux该如何学习.md)
    -   [1.4.3 实作再实作](chapter_1/1.4Linux该如何学习.md)
    -   [1.4.4 发生问题怎么处理啊？建议流程是这样...](chapter_1/1.4Linux该如何学习.md)
    -   [1.4.5 鸟哥的建议（重点在solution的学习）](chapter_1/1.4Linux该如何学习.md)
-   [1.5 重点回顾](chapter_1/1.5重点回顾.md)
-   [1.6 本章习题](chapter_1/1.6本章习题.md)
-   [1.7 参考资料与延伸阅读](chapter_1/1.7参考资料与延伸阅读.md)

### 第二章 主机规划与磁盘分区

事实上，要安装好一部Linux主机并不是那么简单的事情，你必须要针对distributions的特性、服务器的软件能力、 未来的升级需求、硬件扩充性需求等等来考虑，还得要知道磁盘分区、文件系统.....2015/04/28

-   [2.1 Linux与硬件的搭配](chapter_2/2.1Linux与硬件的搭配.md)
    -   [2.1.1 认识计算机的硬件配备](chapter_2/2.1Linux与硬件的搭配.md)
    -   [2.1.2 选择与Linux搭配的主机配备： 硬件支持相关网站](chapter_2/2.1Linux与硬件的搭配.md)
    -   [2.1.3 各硬件设备在Linux中的文件名](chapter_2/2.1Linux与硬件的搭配.md)
    -   [2.1.4 使用虚拟机学习](chapter_2/2.1Linux与硬件的搭配.md)
-   [2.2 磁盘分区](chapter_2/2.2磁盘分区.md)
    -   [2.2.1 磁盘连接的方式与设备文件名的关系](chapter_2/2.2磁盘分区.md)
    -   [2.2.2 MSDOS（MBR） 与 GPT 磁盘分区表（partition table）](chapter_2/2.2磁盘分区.md)
    -   [2.2.3 开机流程中的 BIOS 与 UEFI 开机检测程序](chapter_2/2.2磁盘分区.md)
    -   [2.2.4 Linux安装模式下，磁盘分区的选择（极重要）](chapter_2/2.2磁盘分区.md)
-   [2.3 安装Linux前的规划](chapter_2/2.3安装Linux前的规划.md)
    -   [2.3.1 选择适当的distribution](chapter_2/2.3安装Linux前的规划.md)
    -   [2.3.2 主机的服务规划与硬件的关系](chapter_2/2.3安装Linux前的规划.md)
    -   [2.3.3 主机硬盘的主要规划（partition）](chapter_2/2.3安装Linux前的规划.md)
    -   [2.3.4 鸟哥的两个实际案例](chapter_2/2.3安装Linux前的规划.md)
-   [2.4 重点回顾](chapter_2/2.4重点回顾.md)
-   [2.5 本章习题](chapter_2/2.5本章习题.md)
-   [2.6 参考资料与延伸阅读](chapter_2/2.6参考资料与延伸阅读.md)

### 第三章 安装CentOS 7.x与多重开机技巧

Linux distributions越作越成熟，所以在安装方面也越来越简单！虽然安装非常的简单， 但是刚刚前一章所谈到的基础认知还是需要了解的，包括MBR, partition, boot loader, mount, software的.....2015/05/06

-   [3.1 本练习机的规划--尤其是分区参数](chapter_3/3.1本练习机的规划-尤其是分区参数.md)
-   [3.2 开始安装CentOS 7](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.1 调整开机媒体（BIOS）与虚拟机创建流程](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.2 选择安装模式与开机：inst.gpt 参数](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.3 在地设置之时区、语系与键盘配置](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.4 安装来源设置与软件选择](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.5 磁盘分区与文件系统设置](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.6 核心管理与网络设置](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.7 开始安装、设置 root 密码与新增可切换身份之一般用户](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.8 准备使用系统前的授权同意](chapter_3/3.2开始安装CentOS_7.md)
    -   [3.2.9 其他功能：RAM testing, 安装笔记本电脑的核心参数（Option）](chapter_3/3.2开始安装CentOS_7.md)
-   [3.3 多重开机安装流程与管理（Option）](chapter_3/3.3多重开机安装流程与管理.md)
    -   [3.3.1 安装 CentOS 7.x + windows 7 的规划](chapter_3/3.3多重开机安装流程与管理.md)
    -   [3.3.2 进阶安装 CentOS 7.x 与 Windows 7](chapter_3/3.3多重开机安装流程与管理.md)
    -   [3.3.3 救援 MBR 内的开机管理程序与设置多重开机菜单](chapter_3/3.3多重开机安装流程与管理.md)
-   [3.4 重点回顾](chapter_3/3.4重点回顾.md)
-   [3.5 本章习题](chapter_3/3.5本章习题.md)
-   [3.6 参考资料与延伸阅读](chapter_3/3.6参考资料与延伸阅读.md)

### 第四章 首次登陆与线上求助 man page

终于可以开始使用Linux这个有趣的系统了！由于Linux系统使用了非同步的磁盘/内存数据传输模式， 同时又是个多用户多任务的环境，所以你不能随便的不正常关机，关机有一定的程序喔！错误的关机方法.....2015/06/02

-   [4.1 首次登陆系统](chapter_4/4.1首次登录系统.md)
    -   [4.1.1 首次登陆CentOS 7.x图形接口](chapter_4/4.1首次登录系统.md)
    -   [4.1.2 GNOME的操作与登出,应用程序,文件资源管理器,中文输入法,登出窗口,快速重启 X](chapter_4/4.1首次登录系统.md)
    -   [4.1.3 X Window与文字模式的切换, startx](chapter_4/4.1首次登录系统.md)
    -   [4.1.4 在终端接口登陆linux](chapter_4/4.1首次登录系统.md)
-   [4.2 文字模式下指令的下达](chapter_4/4.2文字模式下指令的下达.md)
    -   [4.2.1 开始下达指令, 语系的支持](chapter_4/4.2文字模式下指令的下达.md)
    -   [4.2.2 基础指令的操作, cal, bc](chapter_4/4.2文字模式下指令的下达.md)
    -   [4.2.3 重要的几个热键\[Tab\], \[ctrl\]-c, \[ctrl\]-d, \[shift\]+\[UP/DOWN\]](chapter_4/4.2文字模式下指令的下达.md)
    -   [4.2.4 错误讯息的查看](chapter_4/4.2文字模式下指令的下达.md)
-   [4.3 Linux系统的线上求助man page与info page](chapter_4/4.3Linux系统的线上求助man_page与info_page.md)
    -   [4.3.1 指令的 --help 求助说明](chapter_4/4.3Linux系统的线上求助man_page与info_page.md)
    -   [4.3.2 man page, mandb/makewhatis](chapter_4/4.3Linux系统的线上求助man_page与info_page.md)
    -   [4.3.3 info page](chapter_4/4.3Linux系统的线上求助man_page与info_page.md)
    -   [4.3.4 其他有用的文件（documents）](chapter_4/4.3Linux系统的线上求助man_page与info_page.md)
-   [4.4 超简单文书编辑器： nano](chapter_4/4.4超简单文字编辑器-nano.md)
-   [4.5 正确的关机方法: sync, shutdown, reboot, halt, poweroff, systemctl](chapter_4/4.5正确的关机方法.md)
-   [4.6 重点回顾](chapter_4/4.6重点回顾.md)
-   [4.7 本章习题](chapter_4/4.7本章习题.md)
-   [4.8 参考资料与延伸阅读](chapter_4/4.8参考资料与延伸阅读.md)

## 第二部分 Linux 文件、目录与磁盘格式

安装完了 Linux 之后，接着下来自然就是要使用他了！我们在 [开机与关机及简易指令操作]()的方式， 因此您可以轻易的使用命令行界面来进行诸多的动作与工作。那么接着下来呢？当然就是想要知道 Linux 里面有什么东西啰，所以，在这一个部分当中，我们将介绍 Linux 最基本的文件权限概念， 与每个文件目录所带有的意涵。

当然啰，要了解权限的概念，那么对于不同的“身份”就需要了解一下才行， 不同的身份的人，所创建的或拥有的文件是否会相同呢？例如系统管理员与一般身份使用者的文件？ 当然不太一样！除此之外，如果您的硬盘空间不足，需要增加硬盘时，应该要如何新增呢？ 还有，内存不足的情况下，有没有增进虚拟内存容量的方法？在接下来的几个章节之中，我们将介绍 Linux 主要的文件架构、以及磁盘在 Linux 当中该如何使用及挂载等问题。

### 第五章 Linux文件权限与目录配置

Linux最优秀的地方之一，就在于他的多用户多任务的环境。而为了让各个使用者具有较保密的文件数据， 因此文件的权限管理就变的很重要了。 Linux一般将文件可存取的身份分为三个类别，分别是 owner/group/other， 且三种身份各有read/write/execute.....2015/06/03

-   [5.1 使用者与群组](chapter_5/5.1使用者与群组.md)
-   [5.2 Linux文件权限概念](chapter_5/5.2Linux文件权限概念.md)
    -   [5.2.1 Linux文件属性, 改变语系的 locale](chapter_5/5.2Linux文件权限概念.md)
    -   [5.2.2 如何改变文件属性与权限：chgrp, chown, chmod](chapter_5/5.2Linux文件权限概念.md)
    -   [5.2.3 目录与文件之权限意义：, 数据夹与抽屉,各项动作所需最小权限](chapter_5/5.2Linux文件权限概念.md)
    -   [5.2.4 Linux文件种类与扩展名](chapter_5/5.2Linux文件权限概念.md)
-   [5.3 Linux目录配置](chapter_5/5.3Linux目录配置.md)
    -   [5.3.1 Linux目录配置的依据--FHS：/, /usr, /var](chapter_5/5.3Linux目录配置.md)
    -   [5.3.2 目录树（directory tree）](chapter_5/5.3Linux目录配置.md)
    -   [5.3.3 绝对路径与相对路径](chapter_5/5.3Linux目录配置.md)
    -   [5.3.4 CentOS 的观察：lsb_release](chapter_5/5.3Linux目录配置.md)
-   [5.4 重点回顾](chapter_5/5.4重点回顾.md)
-   [5.5 本章练习](chapter_5/5.5本章习题.md)
-   [5.6 参考资料与延伸阅读](chapter_5/5.6参考资料与延伸阅读.md)

### 第六章 Linux文件与目录管理

在第五章我们认识了Linux系统下的文件权限概念以及目录的配置说明。 在这个章节当中， 我们就直接来进一步的操作与管理文件与目录吧！包括在不同的目录间变换、 创建与删除目录、创建与删除文件， 还有寻找文件、查阅文件内容.....2015/06/16

-   [6.1 目录与路径](chapter_6/6.1目录与路径.md)
    -   [6.1.1 相对路径与绝对路径](chapter_6/6.1目录与路径.md)
    -   [6.1.2 目录的相关操作： cd, pwd, mkdir, rmdir](chapter_6/6.1目录与路径.md)
    -   [6.1.3 关于可执行文件路径的变量： \$PATH](chapter_6/6.1目录与路径.md)
-   [6.2 文件与目录管理](chapter_6/6.2文件与目录管理.md)
    -   [6.2.1 文件与目录的检视： ls](chapter_6/6.2文件与目录管理.md)
    -   [6.2.2 复制、删除与移动： cp, mv](chapter_6/6.2文件与目录管理.md)
    -   [6.2.3 取得路径的文件名称与目录名称](chapter_6/6.2文件与目录管理.md)
-   [6.3 文件内容查阅](chapter_6/6.3文件内容查阅.md)
    -   [6.3.1 直接检视文件内容： cat, tac, nl](chapter_6/6.3文件内容查阅.md)
    -   [6.3.2 可翻页检视： more, less](chapter_6/6.3文件内容查阅.md)
    -   [6.3.3 数据撷取： head, tail](chapter_6/6.3文件内容查阅.md)
    -   [6.3.4 非纯文本文件： od](chapter_6/6.3文件内容查阅.md)
    -   [6.3.5 修改文件时间与创建新文件： touch](chapter_6/6.3文件内容查阅.md)
-   [6.4 文件与目录的默认权限与隐藏权限](chapter_6/6.4文件与目录的默认权限与隐藏权限.md)
    -   [6.4.1 文件默认权限：umask](chapter_6/6.4文件与目录的默认权限与隐藏权限.md)
    -   [6.4.2 文件隐藏属性：chattr, lsattr](chapter_6/6.4文件与目录的默认权限与隐藏权限.md)
    -   [6.4.3 文件特殊权限：SUID, SGID,SBIT, 权限设置](chapter_6/6.4文件与目录的默认权限与隐藏权限.md)
    -   [6.4.4 观察文件类型：file](chapter_6/6.4文件与目录的默认权限与隐藏权限.md)
-   [6.5 指令与文件的搜寻](chapter_6/6.5指令与文件的搜寻.md)
    -   [6.5.1 指令文件名的搜寻：which](chapter_6/6.5指令与文件的搜寻.md)
    -   [6.5.2 文件文件名的搜寻：whereis,locate / updatedb, find](chapter_6/6.5指令与文件的搜寻.md)
-   [6.6 极重要的复习！权限与指令间的关系](chapter_6/6.6极重要的复习-权限与指令间的关系.md)
-   [6.7 重点回顾](chapter_6/6.7重点回顾.md)
-   [6.8 本章习题](chapter_6/6.8本章习题.md)
-   [6.9 参考资料与延伸阅读](chapter_6/6.9参考资料与延伸阅读.md)

### 第七章 Linux 磁盘与文件系统管理

系统管理员很重要的任务之一就是管理好自己的磁盘文件系统，每个分区不可太大也不能太小，太大会造成磁盘容量的浪费， 太小则会产生文件无法储存的困扰。此外，我们在前面几章谈到的文件权限与属性中， 这些权限与属性分别记录在.....2015/06/26

-   [7.1 认识 Linux 文件系统](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.1 磁盘组成与分区的复习](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.2 文件系统特性： 索引式文件系统](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.3 Linux 的 EXT2 文件系统（inode）: data block, superblock,dumpe2fs](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.4 与目录树的关系](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.5 EXT2/EXT3 文件的存取与日志式文件系统的功能](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.6 Linux 文件系统的运行](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.7 挂载点的意义 （mount point）](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.8 其他 Linux 支持的文件系统与 VFS](chapter_7/7.1认识Linux文件系统.md)
    -   [7.1.9 XFS 文件系统简介： xfs_info](chapter_7/7.1认识Linux文件系统.md)
-   [7.2 文件系统的简单操作](chapter_7/7.2文件系统的简单操作.md)
    -   [7.2.1 磁盘与目录的容量：df, du](chapter_7/7.2文件系统的简单操作.md)
    -   [7.2.2 实体链接与符号链接：ln](chapter_7/7.2文件系统的简单操作.md)
-   [7.3 磁盘的分区、格式化、检验与挂载](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
    -   [7.3.1 观察磁盘分区状态：, parted](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
    -   [7.3.2 磁盘分区 gdisk/fdisk：gdisk, fdisk](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
    -   [7.3.3 磁盘格式化（创建文件系统）：mkfs.xfs, mkfs.xfs for raid,mkfs.ext4, mkfs](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
    -   [7.3.4 文件系统检验：xfs_repair, fsck.ext4](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
    -   [7.3.5 文件系统挂载与卸载： mount, umount](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
    -   [7.3.6 磁盘/文件系统参数修订： mknod, xfs_admin, tune2fs](chapter_7/7.3磁盘的分区-格式化-检验与挂载.md)
-   [7.4 设置开机挂载](chapter_7/7.4设置开机挂载.md)
    -   [7.4.1 开机挂载 /etc/fstab 及 /etc/mtab](chapter_7/7.4设置开机挂载.md)
    -   [7.4.2 特殊设备 loop 挂载（镜像文件不烧录就挂载使用）： 挂载DVD,大型文件, dd](chapter_7/7.4设置开机挂载.md)
-   [7.5 内存交换空间（swap）之创建](chapter_7/7.5内存交换空间swap创建.md)
    -   [7.5.1 使用实体分区创建swap：mkswap, free, swapon, swapoff](chapter_7/7.5内存交换空间swap创建.md)
    -   [7.5.2 使用文件创建swap](chapter_7/7.5内存交换空间swap创建.md)
-   [7.6 文件系统的特殊观察与操作](chapter_7/7.6文件系统的特殊观察与操作.md)
    -   [7.6.1 磁盘空间之浪费问题](chapter_7/7.6文件系统的特殊观察与操作.md)
    -   [7.6.2 利用 GNU 的 parted 进行分区行为 （Optional）](chapter_7/7.6文件系统的特殊观察与操作.md)
-   [7.7 重点回顾](chapter_7/7.7重点回顾.md)
-   [7.8 本章习题 - 第一题一定要做](chapter_7/7.8本章习题.md)
-   [7.9 参考资料与延伸阅读](chapter_7/7.9参考资料与延伸阅读.md)

### 第八章 文件的压缩与打包

在 Linux 下面有相当多的压缩指令可以运行喔！这些压缩指令可以让我们更方便从网络上面下载大型的文件呢！ 此外，我们知道在 Linux 下面的扩展名是没有什么很特殊的意义的，不过，针对这些压缩指令所做出来的压缩文件， 为了方便记忆.....2015/07/16

-   [8.1 压缩文件的用途与技术](chapter_8/8.1压缩文件的用途与技术.md)
-   [8.2 Linux 系统常见的压缩指令](chapter_8/8.2Linux系统常见的压缩指令.md)
    -   [8.2.1 gzip, zcat/zmore/zless/zgrep](chapter_8/8.2Linux系统常见的压缩指令.md)
    -   [8.2.2 bzip2, bzcat/bzmore/bzless/bzgrep](chapter_8/8.2Linux系统常见的压缩指令.md)
    -   [8.2.3 xz, xzcat/xzmore/xzless/xzgrep](chapter_8/8.2Linux系统常见的压缩指令.md)
-   [8.3 打包指令:tar, 解压后的 SELinux 课题](chapter_8/8.3打包指令-tar.md)
-   [8.4 XFS 文件系统的备份与还原](chapter_8/8.4XFS文件系统的备份与还原.md)
    -   [8.4.1 XFS 文件系统备份 xfsdump](chapter_8/8.4XFS文件系统的备份与还原.md)
    -   [8.4.2 XFS 文件系统还原 xfsrestore](chapter_8/8.4XFS文件系统的备份与还原.md)
-   [8.5 光盘写入工具](chapter_8/8.5光盘写入工具.md)
    -   [8.5.1 mkisofs：创建镜像文件： isoinfo](chapter_8/8.5光盘写入工具.md)
    -   [8.5.2 cdrecord：光盘烧录工具](chapter_8/8.5光盘写入工具.md)
-   [8.6 其他常见的压缩与备份工具](chapter_8/8.6其他常见的压缩与备份工具.md)
    -   [8.6.1 dd](chapter_8/8.6其他常见的压缩与备份工具.md)
    -   [8.6.2 cpio](chapter_8/8.6其他常见的压缩与备份工具.md)
-   [8.7 重点回顾](chapter_8/8.7重点回顾.md)
-   [8.8 本章习题](chapter_8/8.8本章习题.md)
-   [8.9 参考资料与延伸阅读](chapter_8/8.9参考资料与延伸阅读.md)

## 第三部分：学习 Shell 与 Shell scripts

了解了基本的 Linux 文件属性与目录的配置之后，在进入更深入的 Linux 世界之前，有几个课题还是一定要知道的，那就是我们所使用的这个文字模式接口，也就是所谓的“Shell”这个咚咚。在 Linux 的世界中，使用的是 GNU 发展出来的强化的第二代 shell ，称为 BASH Shell ，他有什么特异功能呢？简单的说，我们之前下达的几个指令都是 bash 管理的，除此之外， 他还可以记录指令、文件或命令的补全功能、环境变量的使用等等，还有很多功能等着你去发掘呢！

在知道了部分的 bash 功能后，在接着下来，我们还得了解一下什么是数据流重导向？还有常规表达式等等的问题， 这都是未来我们系统管理员在管理主机上面，一个不可缺乏的利器！当然啰，要将这些功能整合起来运用的话， 就不能不学习一下所谓的脚本“ shell scripts ”，他具有基础的程序能力（ Program ），当真是个管理系统的好帮手呢！

再来，在未来的建站设置当中，常会使用到文字编辑器来编辑参数配置文件，这个时候， 系统管理员至少务必要熟悉一套命令行下的文书编辑软件，当然不限制哪一套软件啦，但是 vi 是最标准的 Unix-Like 的命令行之文书处理软件，所以，我们几乎一定可以在每部 Unix-Like 上面发现他的踪迹，所以，就来了解他一下吧，这也是挺重要的工作呢！

### 第九章 vim程序编辑器

系统管理员的重要工作就是得要修改与设置某些重要软件的配置文件， 因此至少得要学会一种以上的命令行的文书编辑器。 在所有版本的 Linux 上头都会有的一套文书编辑器就是 vi ，而且很多软件.....2015/07/07

-   [9.1 vi 与 vim](chapter_9/9.1vi与vim.md)
    -   [9.1.1 为何要学 vim](chapter_9/9.1vi与vim.md)
-   [9.2 vi 的使用](chapter_9/9.2vi的使用.md)
    -   [9.2.1 简易执行范例](chapter_9/9.2vi的使用.md)
    -   [9.2.2 按键说明](chapter_9/9.2vi的使用.md)
    -   [9.2.3 一个案例的练习](chapter_9/9.2vi的使用.md)
    -   [9.2.4 vim 的暂存盘、救援回复与打开时的警告讯息](chapter_9/9.2vi的使用.md)
-   [9.3 vim 的额外功能]chapter_9/9.3vim的额外功能.md)
    -   [9.3.1 区块选择（Visual Block）](chapter_9/9.3vim的额外功能.md)
    -   [9.3.2 多文件编辑](chapter_9/9.3vim的额外功能.md)
    -   [9.3.3 多窗口功能](chapter_9/9.3vim的额外功能.md)
    -   [9.3.4 vim 的挑字补全功能](chapter_9/9.3vim的额外功能.md)
    -   [9.3.5 vim 环境设置与记录： \~/.vimrc, \~/.viminfo](chapter_9/9.3vim的额外功能.md)
    -   [9.3.6 vim 常用指令示意图](chapter_9/9.3vim的额外功能.md)
-   [9.4 其他 vim 使用注意事项](chapter_9/9.4其他vim使用注意事项.md)
    -   [9.4.1 中文编码的问题](chapter_9/9.4其他vim使用注意事项.md)
    -   [9.4.2 DOS 与 Linux 的断行字符： dos2unix,unix2dos](chapter_9/9.4其他vim使用注意事项.md)
    -   [9.4.3 语系编码转换： iconv](chapter_9/9.4其他vim使用注意事项.md)
-   [9.5 重点回顾](chapter_9/9.5重点回顾.md)
-   [9.6 本章习题](chapter_9/9.6本章习题.md)
-   [9.7 参考资料与延伸阅读](chapter_9/9.7参考资料与延伸阅读.md)

### 第十章 认识与学习 BASH

在 Linux 的环境下，如果你不懂 bash 是什么，那么其他的东西就不用学了！ 因为前面几章我们使用终端机下达指令的方式， 就是通过 bash 的环境来处理的喔！ 所以说，他很重要吧！bash 的东西非常的多，包括变量.....2015/07/09

-   [10.1 认识 BASH 这个 Shell](chapter_10/10.1认识bash这个shell.md)
    -   [10.1.1 硬件、核心与 Shell](chapter_10/10.1认识bash这个shell.md)
    -   [10.1.2 为何要学命令行的 shell](chapter_10/10.1认识bash这个shell.md)
    -   [10.1.3 系统的合法 shell 与 /etc/shells 功能](chapter_10/10.1认识bash这个shell.md)
    -   [10.1.4 Bash shell 的功能](chapter_10/10.1认识bash这个shell.md)
    -   [10.1.5 查询指令是否为 Bash shell 的内置命令： type](chapter_10/10.1认识bash这个shell.md)
    -   [10.1.6 指令的下达与快速编辑按钮](chapter_10/10.1认识bash这个shell.md)
-   [10.2 Shell 的变量功能](chapter_10/10.2shell的变量功能.md)
    -   [10.2.1 什么是变量？](chapter_10/10.2shell的变量功能.md)
    -   [10.2.2 变量的取用与设置：echo, 变量设置规则, unset](chapter_10/10.2shell的变量功能.md)
    -   [10.2.3 环境变量的功能：env 与常见环境变量说明, set, export](chapter_10/10.2shell的变量功能.md)
    -   [10.2.4 影响显示结果的语系变量 （locale）](chapter_10/10.2shell的变量功能.md)
    -   [10.2.5 变量的有效范围](chapter_10/10.2shell的变量功能.md)
    -   [10.2.6 变量键盘读取、阵列与宣告： read, declare, array](chapter_10/10.2shell的变量功能.md)
    -   [10.2.7 与文件系统及程序的限制关系： ulimit](chapter_10/10.2shell的变量功能.md)
    -   [10.2.8 变量内容的删除、取代与替换 （Optional）：删除与取代,测试与替换](chapter_10/10.2shell的变量功能.md)
-   [10.3 命令别名与历史命令](chapter_10/10.3命令别名与历史命令.md)
    -   [10.3.1 命令别名设置： alias, unalias](chapter_10/10.3命令别名与历史命令.md)
    -   [10.3.2 历史命令： history, HISTSIZE](chapter_10/10.3命令别名与历史命令.md)
-   [10.4 Bash shell 的操作环境](chapter_10/10.4BashShell的操作环境.md)
    -   [10.4.1 路径与指令搜寻顺序](chapter_10/10.4BashShell的操作环境.md)
    -   [10.4.2 bash 的进站与欢迎讯息： /etc/issue, /etc/motd](chapter_10/10.4BashShell的操作环境.md)
    -   [10.4.3 环境配置文件:login, non-login shell, /etc/profile, \~/.bash_profile, source, \~/.bashrc](chapter_10/10.4BashShell的操作环境.md)
    -   [10.4.4 终端机的环境设置： stty, set](chapter_10/10.4BashShell的操作环境.md)
    -   [10.4.5 万用字符与特殊符号](chapter_10/10.4BashShell的操作环境.md)
-   [10.5 数据流重导向 （Redirection）](chapter_10/10.5数据流重导向.md)
    -   [10.5.1 何谓数据流重导向？](chapter_10/10.5数据流重导向.md)
    -   [10.5.2 命令执行的判断依据： ; , &&, \|\|](chapter_10/10.5数据流重导向.md)
-   [10.6 管线命令 （pipe）](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.1 撷取命令：cut, grep](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.2 排序命令：sort, uniq, wc](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.3 双向重导向：tee](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.4 字符转换命令：tr, col, join, expand](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.5 分区命令： split](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.6 参数代换： xargs](chapter_10/10.6管线命令-pipe.md)
    -   [10.6.7 关于减号 - 的用途](chapter_10/10.6管线命令-pipe.md)
-   [10.7 重点回顾](chapter_10/10.7重点回顾.md)
-   [10.8 本章习题](chapter_10/10.8本章习题.md)
-   [10.9 参考资料与延伸阅读](chapter_10/10.9参考资料与延伸阅读.md)

### 第十一章 正则表达式与文件格式化处理

正则表达式 （Regular Expression, RE, 或称为常规表达式）是通过一些特殊字符的排列， 用以“搜寻/取代/删除”一列或多列文字字串， 简单的说， 正则表达式就是用在字串的处理上面的一项“表示式”。正则表达式并.....2015/07/14

-   [11.1 开始之前：什么是正则表达式](chapter_11/11.1开始之前-什么是正则表达式.md)
-   [11.2 基础正则表达式](chapter_11/11.2基础正则表达式.md)
    -   [11.2.1 语系对正则表达式的影响](chapter_11/11.2基础正则表达式.md)
    -   [11.2.2 grep 的一些进阶选项](chapter_11/11.2基础正则表达式.md)
    -   [11.2.3 基础正则表达式练习](chapter_11/11.2基础正则表达式.md)
    -   [11.2.4 基础正则表达式字符汇整（characters）](chapter_11/11.2基础正则表达式.md)
    -   [11.2.5 sed 工具：行的新增/删除, 行的取代/显示,搜寻并取代, 直接改档](chapter_11/11.2基础正则表达式.md)
-   [11.3 延伸正则表达式](chapter_11/11.3延伸正则表达式.md)
-   [11.4 文件的格式化与相关处理](chapter_11/11.4文件的格式化与相关处理.md)
    -   [11.4.1 printf： 格式化打印](chapter_11/11.4文件的格式化与相关处理.md)
    -   [11.4.2 awk：好用的数据处理工具](chapter_11/11.4文件的格式化与相关处理.md)
    -   [11.4.3 文件比对工具：, cmp, patch](chapter_11/11.4文件的格式化与相关处理.md)
    -   [11.4.4 文件打印准备工具： pr](chapter_11/11.4文件的格式化与相关处理.md)
-   [11.5 重点回顾](chapter_11/11.5重点回顾.md)
-   [11.6 本章习题](chapter_11/11.6本章习题.md)
-   [11.7 参考资料与延伸阅读](chapter_11/11.7参考资料与延伸阅读.md)

### 第十二章 学习 shell scripts

如果你真的很想要走信息这条路，并且想要好好的管理好属于你的主机，那么，别说鸟哥不告诉你， 可以自动管理你的系统的好工具： Shell scripts 真的是得要好好学习学习的！ 基本上， shell script 有点像是早期的批处理文件，亦即是.....2015/07/17

-   [12.1 什么是 Shell Script](chapter_12/12.1什么是ShellScripts.md)
    -   [12.1.1 干嘛学习 shell scripts](chapter_12/12.1什么是ShellScripts.md)
    -   [12.1.2 第一支 script 的撰写与执行](chapter_12/12.1什么是ShellScripts.md)
    -   [12.1.3 撰写 shell script 的良好习惯创建](chapter_12/12.1什么是ShellScripts.md)
-   [12.2 简单的 shell script 练习](chapter_12/12.2简单的ShellScript练习.md)
    -   [12.2.1 简单范例： 对谈式脚本, 随日期变化, 计算 pi](chapter_12/12.2简单的ShellScript练习.md)
    -   [12.2.2 script 的执行方式差异 （source, sh script, ./script）](chapter_12/12.2简单的ShellScript练习.md)
-   [12.3 善用判断式](chapter_12/12.3善用判断式.md)
    -   [12.3.1 利用 test 指令的测试功能](chapter_12/12.3善用判断式.md)
    -   [12.3.2 利用判断符号 \[ \]](chapter_12/12.3善用判断式.md)
    -   [12.3.3 Shell script 的默认变量（\$0, \$1...）： shift](chapter_12/12.3善用判断式.md)
-   [12.4 条件判断式](chapter_12/12.4条件判断式.md)
    -   [12.4.1 利用 if .... then： 单层简单条件,多重复杂条件, 网络状态,退伍](chapter_12/12.4条件判断式.md)
    -   [12.4.2 利用 case ..... esac 判断](chapter_12/12.4条件判断式.md)
    -   [12.4.3 利用 function 功能](chapter_12/12.4条件判断式.md)
-   [12.5 循环 （loop）](chapter_12/12.5循环loop.md)
    -   [12.5.1 while...do...done, until...do...done （不定循环）](chapter_12/12.5循环loop.md)
    -   [12.5.2 for...do...done （固定循环）： 帐号检查,网络状态 \$（seq ）](chapter_12/12.5循环loop.md)
    -   [12.5.3 for...do...done 的数值处理](chapter_12/12.5循环loop.md)
    -   [12.5.4 搭配乱数与阵列的实验](chapter_12/12.5循环loop.md)
-   [12.6 shell script 的追踪与 debug](chapter_12/12.6ShellScript的追踪与debug.md)
-   [12.7 重点回顾](chapter_12/12.7重点回顾.md)
-   [12.8 本章习题](chapter_12/12.8本章习题.md)

## 第四部分：Linux 使用者管理

好了！终于要到了管理 Linux 帐号的时刻了！对于 Linux 有一定的熟悉度之后，再来就是要管理连上 Linux 的帐号问题了！这个帐号的问题可大可小啦！大到可以限制他使用 Linux 主机的各项资源，小到甚至一般帐号的密码订定规则都可以进行规定！端看您对于安全的需求啦！ 此外，如果站在资源平均分配的角度上，那么 Linux 主机上面有限的资源当然是平均分配给大家比较好！这个时候就得来规定一下“谁可以使用多少的硬盘空间？”那就是 Quota 喔！呵呵！厉害吧！

在订定完了一些帐号的规则之后，那么我们就继续来管理一下主机的系统与程序的管理吧！ 这个包括了观察每个程序 （Process） 与工作调度及工作管理 （ jobs control ），这些也都是很重要的工作呢！

### 第十三章 Linux 帐号管理与 ACL 权限控制

要登陆 Linux 系统一定要有帐号与密码才行，否则怎么登陆，您说是吧？不过， 不同的使用者应该要拥有不同的权限才行吧？我们还可以通过 user/group 的特殊权限设置，来规范出不同的群组开发专案呢.....2015/07/22

-   [13.1 Linux 的帐号与群组](chapter_13/13.1Linux的账户与群组.md)
    -   [13.1.1 使用者识别码： UID 与 GID](chapter_13/13.1Linux的账户与群组.md)
    -   [13.1.2 使用者帐号：/etc/passwd 文件结构, /etc/shadow 文件结构](chapter_13/13.1Linux的账户与群组.md)
    -   [13.1.3 关于群组： /etc/group 文件结构,有效与初始群组, groups, newgrp, /etc/gshadow](chapter_13/13.1Linux的账户与群组.md)
-   [13.2 帐号管理](chapter_13/13.2账号管理.md)
    -   [13.2.1 新增与移除使用者： useradd, useradd 参考档, passwd, chage, userdel](chapter_13/13.2账号管理.md)
    -   [13.2.2 使用者功能：id, finger,chfn, chsh](chapter_13/13.2账号管理.md)
    -   [13.2.3 新增与移除群组：groupadd, groupmod, groupdel,gpasswd 群组管理员](chapter_13/13.2账号管理.md)
    -   [13.2.4 帐号管理实例](chapter_13/13.2账号管理.md)
    -   [13.2.5 使用外部身份认证系统](chapter_13/13.2账号管理.md)
-   [13.3 主机的细部权限规划：ACL 的使用](chapter_13/13.3主机的细部权限规划-ACL的使用.md)
    -   [13.3.1 什么是 ACL 与如何支持启动 ACL](chapter_13/13.3主机的细部权限规划-ACL的使用.md)
    -   [13.3.2 ACL 的设置技巧：setfacl, getfacl,ACL 的设置（user, group mask, default）](chapter_13/13.3主机的细部权限规划-ACL的使用.md)
-   [13.4 使用者身份切换](chapter_13/13.4使用者身份切换.md)
    -   [13.4.1 su](chapter_13/13.4使用者身份切换.md)
    -   [13.4.2 sudo： sudo 指令, visudo （/etc/sudoers）（帐号, 限制指令, 别名, 配合 su）](chapter_13/13.4使用者身份切换.md)
-   [13.5 使用者的特殊 shell 与 PAM 模块](chapter_13/13.5使用者的特殊shell和PAM模块.md)
    -   [13.5.1 特殊的 shell :/sbin/nologin, nologin.txt](chapter_13/13.5使用者的特殊shell和PAM模块.md)
    -   [13.5.2 PAM 模块简介](chapter_13/13.5使用者的特殊shell和PAM模块.md)
    -   [13.5.3 PAM 模块设置语法：验证类别（type）、控制标准（flag）、模块与参数](chapter_13/13.5使用者的特殊shell和PAM模块.md)
    -   [13.5.4 常用模块简介： securetty,nologin, pam_pwquality,login流程](chapter_13/13.5使用者的特殊shell和PAM模块.md)
    -   [13.5.5 其他相关文件： limits.conf](chapter_13/13.5使用者的特殊shell和PAM模块.md)
-   [13.6 Linux 主机上的使用者讯息传递](chapter_13/13.6Linux主机上的使用者讯息传递.md)
    -   [13.6.1 查询使用者： w, who, last, lastlog](chapter_13/13.6Linux主机上的使用者讯息传递.md)
    -   [13.6.2 使用者对谈： write, mesg, wall](chapter_13/13.6Linux主机上的使用者讯息传递.md)
    -   [13.6.3 使用者邮件信箱： mail](chapter_13/13.6Linux主机上的使用者讯息传递.md)
-   [13.7 CentOS 7 环境下大量创建帐号的方法](chapter_13/13.7CentOS7环境下大量创建账号的方法.md)
    -   [13.7.1 一些帐号相关的检查工具：pwck, pwconv, chpasswd](chapter_13/13.7CentOS7环境下大量创建账号的方法.md)
    -   [13.7.2 大量创建帐号范本（适用 passwd --stdin 选项）](chapter_13/13.7CentOS7环境下大量创建账号的方法.md)
-   [13.8 重点回顾](chapter_13/13.8重点回顾.md)
-   [13.9 本章习题](chapter_13/13.9本章习题.md)
-   [13.10 参考资料与延伸阅读](chapter_13/13.10参考资料与延伸阅读.md)

### 第十四章 磁盘配额（Quota）与进阶文件系统管理

如果您的 Linux 服务器有多个用户经常存取数据时，为了维护所有使用者在硬盘容量的公平使用，磁盘配额 （Quota） 就是一项非常有用的工具！另外，如果你的用户常常抱怨磁盘容量不够用，那么更进阶的文件系统就得要学习学习.....2015/07/28

-   [14.1 磁盘配额 （Quota） 的应用与实作](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.1 什么是 Quota：一般用途, 限制, 规范 （inode/block, soft/hard, grace time）](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.2 一个 XFS 文件系统的 Quota 的实作范例](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.3 实作 Quota 流程-1：文件系统的支持与观察（/etc/fstab, /etc/mtab）](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.4 实作 Quota 流程-2：观察 Quota 报告数据（xfs_quota,print, df, report, state）](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.5 实作 Quota 流程-3：限制值设置方式](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.6 实作 Quota 流程-4：project 的限制 （针对目录限制） （Optional）](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.7 XFS quota 的管理与额外指令对照表](chapter_14/14.1磁盘配额Quota的应用与实作.md)
    -   [14.1.8 不更动既有系统的 Quota 实例](chapter_14/14.1磁盘配额Quota的应用与实作.md)
-   [14.2 软件磁盘阵列 （Software RAID）](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
    -   [14.2.1 什么是 RAID： RAID-0, RAID-1,RAID1+0, Spare disk](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
    -   [14.2.2 software, hardware RAID](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
    -   [14.2.3 软件磁盘阵列的设置： mdadm --create](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
    -   [14.2.4 仿真 RAID 错误的救援模式： mdadm --manage](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
    -   [14.2.5 开机自动启动 RAID 并自动挂载](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
    -   [14.2.6 关闭软件 RAID（重要！）](chapter_14/14.2软件磁盘阵列SoftwareRAID.md)
-   [14.3 逻辑卷轴管理员 （Logical Volume Manager）](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
    -   [14.3.1 什么是 LVM： PV, PE, VG, LV 的意义](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
    -   [14.3.2 LVM 实作流程： PV 阶段, VG 阶段,LV 阶段, 文件系统阶段](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
    -   [14.3.3 放大 LV 容量： xfs_growfs](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
    -   [14.3.4 使用 LVM thin Volume 让 LVM 动态自动调整磁盘使用率](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
    -   [14.3.5 LVM 的磁盘快照： 创建传统快照, 以快照还原,用于测试环境](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
    -   [14.3.6 LVM 相关指令汇整与 LVM 的关闭](chapter_14/14.3逻辑卷轴管理员LogicalVolumeManager.md)
-   [14.4 重点回顾](chapter_14/14.4重点回顾.md)
-   [14.5 本章习题](chapter_14/14.5本章习题.md)
-   [14.6 参考资料与延伸阅读](chapter_14/14.6参考资料与延伸阅读.md)

### 第十五章 例行性工作调度 （crontab）

学习了基础篇也一阵子了，你会发现到为什么系统常常会主动的进行一些任务？ 这些任务到底是谁在设置工作的？ 如果你想要让自己设计的备份程序可以自动的在系统下面执行，.....2015/07/31

-   [15.1 什么是例行性工作调度](chapter_15/15.1什么是例行性工作调度.md)
    -   [15.1.1 Linux 工作调度的种类： at, crontab](chapter_15/15.1什么是例行性工作调度.md)
    -   [15.1.2 CentOS Linux 系统上常见的例行性工作](chapter_15/15.1什么是例行性工作调度.md)
-   [15.2 仅执行一次的工作调度](chapter_15/15.2仅执行一次的工作调度.md)
    -   [15.2.1 atd 的启动与 at 运行的方式： /etc/at.deny](chapter_15/15.2仅执行一次的工作调度.md)
    -   [15.2.2 实际运行单一工作调度： at,atq & atrm, batch](chapter_15/15.2仅执行一次的工作调度.md)
-   [15.3 循环执行的例行性工作调度](chapter_15/15.3循环执行的例行性工作调度.md)
    -   [15.3.1 使用者的设置： /etc/cron.deny, crontab](chapter_15/15.3循环执行的例行性工作调度.md)
    -   [15.3.2 系统的配置文件： /etc/crontab, /etc/cron.d/\*](chapter_15/15.3循环执行的例行性工作调度.md)
    -   [15.3.3 一些注意事项](chapter_15/15.3循环执行的例行性工作调度.md)
-   [15.4 可唤醒停机期间的工作任务](chapter_15/15.4可唤醒停机期间的工作任务.md)
    -   [15.4.1 什么是 anacron](chapter_15/15.4可唤醒停机期间的工作任务.md)
    -   [15.4.2 anacron 与 /etc/anacrontab](chapter_15/15.4可唤醒停机期间的工作任务.md)
-   [15.5 重点回顾](chapter_15/15.5重点回顾.md)
-   [15.6 本章习题](chapter_15/15.6本章习题.md)

### 第十六章 程序管理与 SELinux 初探

一个程序被载入到内存当中运行，那么在内存内的那个数据就被称为程序（process）。程序是操作系统上非常重要的概念， 所有系统上面跑的数据都会以程序的型态存在。那么系统的程序有哪些状态.....2015/08/08

-   [16.1 什么是程序 （Process）](chapter_16/16.1什么是程序process.md)
    -   [16.1.1 程序与程序 （process & program）：子程序与父程序, fork-and-exec,系统服务](chapter_16/16.1什么是程序process.md)
    -   [16.1.2 Linux 的多用户多任务环境](chapter_16/16.1什么是程序process.md)
-   [16.2 工作管理 （job control）](chapter_16/16.2工作管理JobControl.md)
    -   [16.2.1 什么是工作管理](chapter_16/16.2工作管理JobControl.md)
    -   [16.2.2 job control 的管理：&, \[ctrl\]-z, jobs, kill](chapter_16/16.2工作管理JobControl.md)
    -   [16.2.3 离线管理问题： nohup](chapter_16/16.2工作管理JobControl.md)
-   [16.3 程序管理](chapter_16/16.3程序管理.md)
    -   [16.3.1 程序的观察： ps -l,ps aux, top,pstree](chapter_16/16.3程序管理.md)
    -   [16.3.2 程序的管理： signal, kill, killall](chapter_16/16.3程序管理.md)
    -   [16.3.3 关于程序的执行顺序： priority, nice, renice](chapter_16/16.3程序管理.md)
    -   [16.3.4 系统资源的观察： free, uname, uptime, netstat, vmstat](chapter_16/16.3程序管理.md)
-   [16.4 特殊文件与程序](chapter_16/16.4特殊文件与程序.md)
    -   [16.4.1 具有 SUID/SGID 权限的指令执行状态](chapter_16/16.4特殊文件与程序.md)
    -   [16.4.2 /proc/\* 代表的意义](chapter_16/16.4特殊文件与程序.md)
    -   [16.4.3 查询已打开文件或已执行程序打开之文件： fuser, lsof, pidof](chapter_16/16.4特殊文件与程序.md)
-   [16.5 SELinux 初探](chapter_16/16.5SELinux初探.md)
    -   [16.5.1 什么是 SELinux： 目标, DAC,MAC](chapter_16/16.5SELinux初探.md)
    -   [16.5.2 SELinux 的运行模式： 元件, 安全性本文,domain/type](chapter_16/16.5SELinux初探.md)
    -   [16.5.3 SELinux 三种模式的启动、关闭与观察： getenforce,sestatus, setenforce](chapter_16/16.5SELinux初探.md)
    -   [16.5.4 SELinux 政策内的规则管理： getsebool, seinfo, sesearch, setsebool](chapter_16/16.5SELinux初探.md)
    -   [16.5.5 SELinux 安全本文的修改：chcon, restorecon,semanage](chapter_16/16.5SELinux初探.md)
    -   [16.5.6 一个网络服务案例及登录文件协助：所需服务, FTP 实例, 匿名者范例, 一般用户主文件夹, 非正规目录, 非正规 port](chapter_16/16.5SELinux初探.md)
-   [16.6 重点回顾](chapter_16/16.6重点回顾.md)
-   [16.7 本章习题](chapter_16/16.7本章习题.md)
-   [16.8 参考资料与延伸阅读](chapter_16/16.8参考资料与延伸阅读.md)

## 第五部分：Linux 系统管理员

嗯！终于来到系统管理员 （ root ） 要注意的工作事项之篇幅了！各位准系统管理员心理准备好了吗？ 我们要管理机器啰，呵呵！那么管理员的工作是什么？看报喝茶？！没错！管理员最大的享受就是看报喝茶了。 一个好的系统管理员，平时不会希望挂载网站上面一再不断的查询、检查漏洞等等的， 因为果真如此的话，那么就表示“机器一定有问题了！”。为了让我们的 Linux 机器跑得更稳更顺畅，好让我这个管理员有更多的时间去看报喝茶，哈哈！ 更深入的了解系统是需要的！所以，这一篇我们由开机关机的整体流程谈起，好了解一下 Linux 在开机的过程中到底做了哪些事情，这样才能知道我们在什么时候应该做什么事情呐！

此外，由于“没有一个套件是永远安全的！”，所以套件管理是相当重要的一部份，这里我们以 RPM 与 Tarball 来介绍一下如何管理你系统上面的套件。再来，你知道你的系统上面跑了多少数据吗？ 虽然知道什么是 ps 来查询程序，但是总是得知道我的系统有哪些服务吧！嘿嘿！ 来看看先?不但如此，还得针对登录文件进行解析，以及对于系统进行备份。呵呵！ 管理员的工作还真多那。不止不止，还要进行核心的管理呢！哇！果然是忙毙了！无论如何， 还是得要了解呐！

### 第十七章 认识系统服务（daemon）

在 Unix-Like 的系统中，你常常听到 daemon 这个字眼！那么什么是传说中的 daemon 呢？这些 daemon 放在什么地方？他的功能是什么？该如何启动这些 daemon ？又如何有效的将这些 daemon 管理妥当.....2015/08/14

-   [17.1 什么是 daemon 与服务 （service）](chapter_17/17.1什么是daemon与服务service.md)
    -   [17.1.1 早期 Systemp V 的 init 管理行为中 daemon 的主要分类](chapter_17/17.1什么是daemon与服务service.md)
    -   [17.1.2 systemd 使用的 unit 分类](chapter_17/17.1什么是daemon与服务service.md)
-   [17.2 通过 systemctl 管理服务](chapter_17/17.2通过systemctl管理服务.md)
    -   [17.2.1 通过 systemctl 管理单一服务 （service unit） 的启动/开机启动与观察状态](chapter_17/17.2通过systemctl管理服务.md)
    -   [17.2.2 通过 systemctl 观察系统上所有的服务](chapter_17/17.2通过systemctl管理服务.md)
    -   [17.2.3 通过 systemctl 管理不同的操作环境 （target unit）](chapter_17/17.2通过systemctl管理服务.md)
    -   [17.2.4 通过 systemctl 分析各服务之间的相依性](chapter_17/17.2通过systemctl管理服务.md)
    -   [17.2.5 与 systemd 的 daemon 运行过程相关的目录简介：/etc/services](chapter_17/17.2通过systemctl管理服务.md)
    -   [17.2.6 关闭网络服务](chapter_17/17.2通过systemctl管理服务.md)
-   [17.3 systemctl 针对 service 类型的配置文件](chapter_17/17.3systemctl针对service类型的配置文件.md)
    -   [17.3.1 systemctl 配置文件相关目录简介](chapter_17/17.3systemctl针对service类型的配置文件.md)
    -   [17.3.2 systemctl 配置文件的设置项目简介](chapter_17/17.3systemctl针对service类型的配置文件.md)
    -   [17.3.3 两个 vsftpd 运行的实例](chapter_17/17.3systemctl针对service类型的配置文件.md)
    -   [17.3.4 多重的重复设置方式：以 getty 为例](chapter_17/17.3systemctl针对service类型的配置文件.md)
    -   [17.3.5 自己的服务自己作](chapter_17/17.3systemctl针对service类型的配置文件.md)
-   [17.4 systemctl 针对 timer 的配置文件](chapter_17/17.4systemctl针对timer的配置文件.md)
-   [17.5 CentOS 7.x 默认启动的服务简易说明](chapter_17/17.5CentOS7.x默认启动的服务简易说明.md)
-   [17.6 重点回顾](chapter_17/17.6重点回顾.md)
-   [17.7 本章习题](chapter_17/17.7本章习题.md)
-   [17.8 参考资料与延伸阅读](chapter_17/17.8参考资料与延伸阅读.md)

### 第十八章 认识与分析登录文件

当你的 Linux 系统出现不明原因的问题时，很多人都告诉你，你要查阅一下登录文件才能够知道系统出了什么问题了， 所以说，了解登录文件是很重要的事情呢。登录文件可以记录系统在什么时间、哪个主机、哪个服务.....2015/08/20

-   [18.1 什么是登录文件](chapter_18/18.1什么是登录文件.md)：
    -   [18.1.1 CentOS 7 登录文件简易说明：重要性, 常见文件名,服务与程序,systemd-journald](chapter_18/18.1什么是登录文件.md)
    -   [18.1.2 登录文件内容的一般格式](chapter_18/18.1什么是登录文件.md)
-   [18.2 rsyslog.service ：记录登录文件的服务](chapter_18/18.2rsyslog.service-记录登录文件的服务.md)
    -   [18.2.1 rsyslog.service 的配置文件： /etc/rsyslog.conf, 默认的 rsyslog.conf 内容](chapter_18/18.2rsyslog.service-记录登录文件的服务.md)
    -   [18.2.2 登录文件的安全性设置](chapter_18/18.2rsyslog.service-记录登录文件的服务.md)
    -   [18.2.3 登录文件服务器的设置](chapter_18/18.2rsyslog.service-记录登录文件的服务.md)
-   [18.3 登录文件的轮替 （logrotate）](chapter_18/18.3登录文件的轮替logrotate.md)
    -   [18.3.1 logrotate 的配置文件](chapter_18/18.3登录文件的轮替logrotate.md)
    -   [18.3.2 实际测试 logrotate 的动作](chapter_18/18.3登录文件的轮替logrotate.md)
    -   [18.3.3 自订登录文件的轮替功能](chapter_18/18.3登录文件的轮替logrotate.md)
-   [18.4 systemd-journald.service 简介](chapter_18/18.4systemd-journald.service简介.md)：
    -   [18.4.1 使用 journalctl 观察登录信息](chapter_18/18.4systemd-journald.service简介.md)
    -   [18.4.2 logger 指令的应用](chapter_18/18.4systemd-journald.service简介.md)
    -   [18.4.3 保存 journal 的方式](chapter_18/18.4systemd-journald.service简介.md)
-   [18.5 分析登录文件](chapter_18/18.5分析登录文件.md)
    -   [18.5.1 CentOS 默认提供的 logwatch](chapter_18/18.5分析登录文件.md)
    -   [18.5.2 鸟哥自己写的登录文件分析工具：](chapter_18/18.5分析登录文件.md)
-   [18.6 重点回顾](chapter_18/18.6重点回顾.md)
-   [18.7 本章习题练习](chapter_18/18.7本章习题.md)
-   [18.8 参考资料与延伸阅读](chapter_18/18.8参考资料与延伸阅读.md)

### 第十九章 开机流程、模块管理与 loader

系统开机其实是一项非常复杂的程序，因为核心得要侦测硬件并载入适当的驱动程序后， 接下来则必须要调用程序来准备好系统运行的环境，以让使用者能够顺利的操作整部主机系统。 如果你能够理解开机的原理.....2015/08/31

-   [19.1 Linux 的开机流程分析](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.1 开机流程一览](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.2 BIOS, boot loader 与 kernel 载入：lsinitrd](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.3 第一支程序 systemd 及使用 default.target 进入开机程序分析](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.4 systemd 执行 sysinit.target 初始化系统、basic.target 准备系统](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.5 systemd 启动 multi-user.target 下的服务：相容的 rc.local,getty.target 启动](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.6 systemd 启动 graphical.target 下面的服务](chapter_19/19.1Linux的开机流程分析.md)
    -   [19.1.7 开机过程会用到的主要配置文件](chapter_19/19.1Linux的开机流程分析.md)
-   [19.2 核心与核心模块](chapter_19/19.2核心与核心模块.md)
    -   [19.2.1 核心模块与相依性： depmod](chapter_19/19.2核心与核心模块.md)
    -   [19.2.2 核心模块的观察： lsmod, modinfo](chapter_19/19.2核心与核心模块.md)
    -   [19.2.3 核心模块的载入与移除：insmod, modprobe, rmmod](chapter_19/19.2核心与核心模块.md)
    -   [19.2.4 核心模块的额外参数设置：/etc/modprobe.d/\*conf](chapter_19/19.2核心与核心模块.md)
-   [19.3 Boot loader: Grub2](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.1 boot loader 的两个 stage](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.2 grub2 的配置文件 /boot/grub2/grub.cfg 初探： 磁盘代号, grub.cfg](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.3 grub2 配置文件维护 /etc/default/grub 与 /etc/grub.d：grub,40_custom](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.4 initramfs 的重要性与创建新 initramfs 文件： dracut/mkinitrd](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.5 测试与安装 grub2： grub2-install](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.6 开机前的额外功能修改](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.7 关于开机画面与终端机画面的图形显示方式](chapter_19/19.3BootLoader-Grub2.md)
    -   [19.3.8 为个别菜单加上密码： grub2-mkpasswd-pbkdf2](chapter_19/19.3BootLoader-Grub2.md)
-   [19.4 开机过程的问题解决](chapter_19/19.4开机过程的问题解决.md)
    -   [19.4.1 忘记 root 密码的解决之道](chapter_19/19.4开机过程的问题解决.md)
    -   [19.4.2 直接开机就以 root 执行 bash 的方法](chapter_19/19.4开机过程的问题解决.md)
    -   [19.4.3 因文件系统错误而无法开机](chapter_19/19.4开机过程的问题解决.md)
-   [19.5 重点回顾](chapter_19/19.5重点回顾.md)
-   [19.6 本章习题](chapter_19/19.6本章习题.md)
-   [19.7 参考资料与延伸阅读](chapter_19/19.7参考资料与延伸阅读.md)

### 第二十章 网络设置与备份策略

新的 CentOS 7 有针对不同的服务提供了相当大量的命令行设置模式，因此过去那个 setup 似乎没有什么用了！ 取而代之的是许多加入了 bash-complete 提供了不少参数补全的设置工具！甚至包括网络设置也是通过这个机制哩！ 我们这个小章.....2015/09/03

-   [20.1 系统基本设置](chapter_20/20.1系统基本设置.md)
    -   [20.1.1 网络设置 （手动设置与DHCP自动取得）：手动,自动,改主机名称](chapter_20/20.1系统基本设置.md)
    -   [20.1.2 日期与时间设置](chapter_20/20.1系统基本设置.md)
    -   [20.1.3 语系设置](chapter_20/20.1系统基本设置.md)
    -   [20.1.4 防火墙简易设置](chapter_20/20.1系统基本设置.md)
-   [20.2 服务器硬件数据的收集](chapter_20/20.2服务器硬件数据的收集.md)
    -   [20.2.1 以系统内置 dmidecode 解析硬件配备](chapter_20/20.2服务器硬件数据的收集.md)
    -   [20.2.2 硬件资源的收集与分析： lspci, lsusb,iostat...](chapter_20/20.2服务器硬件数据的收集.md)
    -   [20.2.3 了解磁盘的健康状态](chapter_20/20.2服务器硬件数据的收集.md)
-   [20.3 备份要点](chapter_20/20.3备份要点.md)
    -   [20.3.1 备份数据的考虑](chapter_20/20.3备份要点.md)
    -   [20.3.2 哪些 Linux 数据具有备份的意义](chapter_20/20.3备份要点.md)
    -   [20.3.3 备份用储存媒体的选择](chapter_20/20.3备份要点.md)
-   [20.4 备份的种类、频率与工具的选择](chapter_20/20.4备份的种类和频率与工具的选择.md)
    -   [20.4.1 完整备份之累积备份 （Incremental backup）,使用软件](chapter_20/20.4备份的种类和频率与工具的选择.md)
    -   [20.4.2 完整备份之差异备份 （Differential backup）](chapter_20/20.4备份的种类和频率与工具的选择.md)
    -   [20.4.3 关键数据备份](chapter_20/20.4备份的种类和频率与工具的选择.md)
-   [20.5 VBird 的备份策略与 scripts](chapter_20/20.5鸟哥的备份策略.md)
    -   [20.5.1 每周系统备份的 script](chapter_20/20.5鸟哥的备份策略.md)
    -   [20.5.2 每日备份数据的 script](chapter_20/20.5鸟哥的备份策略.md)
    -   [20.5.3 远端备援的 script](chapter_20/20.5鸟哥的备份策略.md)
-   [20.6 灾难复原的考虑](chapter_20/20.6灾难复原的考虑.md)
-   [20.7 重点回顾](chapter_20/20.7重点回顾.md)
-   [20.8 本章习题](chapter_20/20.8本章习题.md)
-   [20.9 参考资料与延伸阅读](chapter_20/20.9参考资料与延伸阅读.md)

### 第二十一章 软件安装：源代码与 Tarball

我们在第一章、Linux是什么当中提到了 GNU 计划与 GPL 授权所产生的自由软件与开放源码等咚咚。 不过，前面的章节都还没有提到真正的开放源码是什么的讯息！在这一章当中，我们将借由 Linux 操作系统里面的可执行文件.....2015/09/06

-   [21.1 开放源码的软件安装与升级简介](chapter_21/21.1开源代码的软件安装与升级简介.md)
    -   [21.1.1 什么是开放源码、编译器与可可执行文件](chapter_21/21.1开源代码的软件安装与升级简介.md)
    -   [21.1.2 什么是函数库](chapter_21/21.1开源代码的软件安装与升级简介.md)
    -   [21.1.3 什么是 make 与 configure](chapter_21/21.1开源代码的软件安装与升级简介.md)
    -   [21.1.4 什么是 Tarball 的软件](chapter_21/21.1开源代码的软件安装与升级简介.md)
    -   [21.1.5 如何安装与升级软件](chapter_21/21.1开源代码的软件安装与升级简介.md)
-   [21.2 使用传统程序语言进行编译的简单范例](chapter_21/21.2使用传统程序语言进行编译的简单范例.md)
    -   [21.2.1 单一程序：印出 Hello World](chapter_21/21.2使用传统程序语言进行编译的简单范例.md)
    -   [21.2.2 主、副程序链接：副程序的编译](chapter_21/21.2使用传统程序语言进行编译的简单范例.md)
    -   [21.2.3 调用外部函数库：加入链接的函数库](chapter_21/21.2使用传统程序语言进行编译的简单范例.md)
    -   [21.2.4 gcc 的简易用法 （编译、参数与链结）](chapter_21/21.2使用传统程序语言进行编译的简单范例.md)
-   [21.3 用 make 进行宏编译](chapter_21/21.3用make进行宏编译.md)
    -   [21.3.1 为什么要用 make](chapter_21/21.3用make进行宏编译.md)
    -   [21.3.2 makefile 的基本语法与变量](chapter_21/21.3用make进行宏编译.md)
-   [21.4 Tarball 的管理与建议](chapter_21/21.4Tarball的管理与建议.md)
    -   [21.4.1 使用源代码管理软件所需要的基础软件](chapter_21/21.4Tarball的管理与建议.md)
    -   [21.4.2 Tarball 安装的基本步骤](chapter_21/21.4Tarball的管理与建议.md)
    -   [21.4.3 一般 Tarball 软件安装的建议事项 （如何移除？升级？）](chapter_21/21.4Tarball的管理与建议.md)
    -   [21.4.4 一个简单的范例、利用 ntp 来示范](chapter_21/21.4Tarball的管理与建议.md)
    -   [21.4.5 利用 patch 更新源代码](chapter_21/21.4Tarball的管理与建议.md)
-   [21.5 函数库管理](chapter_21/21.5函数库管理.md)
    -   [21.5.1 动态与静态函数库](chapter_21/21.5函数库管理.md)
    -   [21.5.2 ldconfig 与 /etc/ld.so.conf](chapter_21/21.5函数库管理.md)
    -   [21.5.3 程序的动态函数库解析： ldd](chapter_21/21.5函数库管理.md)
-   [21.6 检验软件的正确性](chapter_21/21.6检验软件正确性.md)
    -   [21.6.1 md5sum / sha1sum / sha256sum](chapter_21/21.6检验软件正确性.md)
-   [21.7 重点回顾](chapter_21/21.7重点回顾.md)
-   [21.8 课后练习](chapter_21/21.8本章习题.md)
-   [21.9 参考资料与延伸阅读](chapter_21/21.9参考资料与延伸阅读.md)

### 第二十二章 软件安装：RPM, SRPM 与 YUM 功能

虽然使用源代码进行编译可以进行客制化的设置，但对于 Linux distribution 的原本发布商来说， 则有软件管理不易的问题， 毕竟不是每个人都会进行源代码编译的。 如果能够将软件预先在相同的硬件与操作系统上面编译好才发布的话.....2015/09/09

-   [22.1 软件管理员简介](chapter_22/22.1软件管理员简介.md)
    -   [22.1.1 Linux 界的两大主流: RPM 与 DPKG](chapter_22/22.1软件管理员简介.md)
    -   [22.1.2 什么是 RPM 与 SRPM](chapter_22/22.1软件管理员简介.md)
    -   [22.1.3 什么是 i386, i586, i686, noarch, x86_64](chapter_22/22.1软件管理员简介.md)
    -   [22.1.4 RPM 的优点](chapter_22/22.1软件管理员简介.md)
    -   [22.1.5 RPM 属性相依的克服方式： YUM 线上升级](chapter_22/22.1软件管理员简介.md)
-   [22.2 RPM 软件管理程序： rpm](chapter_22/22.2RPM软件管理程序-rpm.md)
    -   [22.2.1 RPM 默认安装的路径](chapter_22/22.2RPM软件管理程序-rpm.md)
    -   [22.2.2 RPM 安装 （install）](chapter_22/22.2RPM软件管理程序-rpm.md)
    -   [22.2.3 RPM 升级与更新 （upgrade/freshen）](chapter_22/22.2RPM软件管理程序-rpm.md)
    -   [22.2.4 RPM 查询 （query）](chapter_22/22.2RPM软件管理程序-rpm.md)
    -   [22.2.5 RPM 验证与数码签章 （Verify/signature）](chapter_22/22.2RPM软件管理程序-rpm.md)
    -   [22.2.6 RPM 反安装与重建数据库 （erase/rebuilddb）](chapter_22/22.2RPM软件管理程序-rpm.md)
-   [22.3 YUM 线上升级机制](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.1 利用 yum 进行查询、安装、升级与移除功能](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.2 yum 的配置文件](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.3 yum 的软件群组功能](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.4 EPEL/ELRepo 外挂软件以及自订配置文件](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.5 全系统自动升级](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.6 管理的抉择：RPM 还是 Tarball](chapter_22/22.3YUM线上升级机制.md)
    -   [22.3.7 基础服务管理：以 Apache 为例](chapter_22/22.3YUM线上升级机制.md)
-   [22.4 SRPM 的使用： rpmbuild （Optional）](chapter_22/22.4SRPM的使用-rpmbuild.md)
    -   [22.4.1 利用默认值安装 SRPM 文件 （--rebuid/--recompile）](chapter_22/22.4SRPM的使用-rpmbuild.md)
    -   [22.4.2 SRPM 使用的路径与需要的软件](chapter_22/22.4SRPM的使用-rpmbuild.md)
    -   [22.4.3 配置文件的主要内容 （\*.spec）](chapter_22/22.4SRPM的使用-rpmbuild.md)
    -   [22.4.4 SRPM 的编译指令 （-ba/-bb）](chapter_22/22.4SRPM的使用-rpmbuild.md)
    -   [22.4.5 一个打包自己软件的范例](chapter_22/22.4SRPM的使用-rpmbuild.md)
-   [22.5 重点回顾](chapter_22/22.5重点回顾.md)
-   [22.6 本章习题](chapter_22/22.6本章习题.md)
-   [22.7 参考资料与延伸阅读](chapter_22/22.7参考资料与延伸阅读.md)

### 第二十三章 X Window 设置介绍

在 Linux 上头的图形接口我们称之为 X Window System，简称为 X 或 X11 啰！为何称之为系统呢？这是因为 X 窗口系统又分为 X server 与 X client ，既然是 Server/Client （主从架构） 这就表示其实 X 窗口系统是可以跨网络且跨平台的.....2015/09/19

-   [23.1 什么是 X Window System](chapter_23/23.1什么是XWindowSystem.md)
    -   [23.1.1 X Window 的发展简史](chapter_23/23.1什么是XWindowSystem.md)
    -   [23.1.2 主要元件： X Server/X Client/Window Manager/Display Manager](chapter_23/23.1什么是XWindowSystem.md)
    -   [23.1.3 X Window 的启动流程：startx, xinit](chapter_23/23.1什么是XWindowSystem.md)
    -   [23.1.4 X 启动流程测试](chapter_23/23.1什么是XWindowSystem.md)
    -   [23.1.5 我是否需要启用 X Window System](chapter_23/23.1什么是XWindowSystem.md)
-   [23.2 X Server 配置文件解析与设置](chapter_23/23.2XServer配置文件解析与设置.md)
    -   [23.2.1 解析 xorg.conf 设置](chapter_23/23.2XServer配置文件解析与设置.md)
    -   [23.2.2 字体管理](chapter_23/23.2XServer配置文件解析与设置.md)
    -   [23.2.3 显示器参数微调](chapter_23/23.2XServer配置文件解析与设置.md)
-   [23.3 显卡驱动程序安装范例](chapter_23/23.3显卡驱动程序安装范例.md)
    -   [23.3.1 NVidia](chapter_23/23.3显卡驱动程序安装范例.md)
    -   [23.3.2 AMD （ATI）](chapter_23/23.3显卡驱动程序安装范例.md)
    -   [23.3.3 Intel](chapter_23/23.3显卡驱动程序安装范例.md)
-   [23.4 重点回顾](chapter_23/23.4重点回顾.md)
-   [23.5 本章习题](chapter_23/23.5本章习题.md)
-   [23.6 参考资料与延伸阅读](chapter_23/23.6参考资料与延伸阅读.md)

### 第二十四章 核心编译

我们说的 Linux 其实指的就是核心 （kernel） 而已。这个核心控制你主机的所有硬件并提供系统所有的功能， 所以说，他重不重要啊！我们开机的时候其实就是利用开机管理程序载入这个核心文件来侦测硬件， 在核心载入适当的驱动程序后.....2015/10/20

-   [24.1 编译前的任务：认识核心与取得核心源代码](chapter_24/24.1编译前的任务-认识核心与取得核心源代码.md)
    -   [24.1.1 什么是核心 （Kernel）](chapter_24/24.1编译前的任务-认识核心与取得核心源代码.md)
    -   [24.1.2 更新核心的目的](chapter_24/24.1编译前的任务-认识核心与取得核心源代码.md)
    -   [24.1.3 核心的版本](chapter_24/24.1编译前的任务-认识核心与取得核心源代码.md)
    -   [24.1.4 核心源代码的取得方式：distributions 默认、最新、patch](chapter_24/24.1编译前的任务-认识核心与取得核心源代码.md)
    -   [21.1.5 核心源代码的解压缩/安装/观察](chapter_24/24.1编译前的任务-认识核心与取得核心源代码.md)
-   [24.2 核心编译的前处理与核心功能选择](chapter_24/24.2核心编译的前处理与核心功能选择.md)
    -   [24.2.1 硬件环境检视与核心功能要求](chapter_24/24.2核心编译的前处理与核心功能选择.md)
    -   [24.2.2 保持干净源代码： make mrproper](chapter_24/24.2核心编译的前处理与核心功能选择.md)
    -   [24.2.3 开始挑选核心功能： make XXconfig](chapter_24/24.2核心编译的前处理与核心功能选择.md)
    -   [24.2.4 核心功能细项选择](chapter_24/24.2核心编译的前处理与核心功能选择.md)
-   [24.3 核心的编译与安装](chapter_24/24.3核心的编译与安装.md)
    -   [24.3.1 编译核心与核心模块](chapter_24/24.3核心的编译与安装.md)
    -   [24.3.2 实际安装模块](chapter_24/24.3核心的编译与安装.md)
    -   [24.3.3 开始安装新核心与多重核心菜单 （grub）](chapter_24/24.3核心的编译与安装.md)
-   [24.4 额外（单一）核心模块编译](chapter_24/24.4额外-单一核心模块编译.md)
    -   [24.4.1 编译前注意事项](chapter_24/24.4额外-单一核心模块编译.md)
    -   [24.4.2 单一模块编译](chapter_24/24.4额外-单一核心模块编译.md)
    -   [24.4.3 核心模块管理](chapter_24/24.4额外-单一核心模块编译.md)
-   [24.5 以最新核心版本编译 CentOS 7.x 的核心](chapter_24/24.5以最新核心版本编译CentOS7.x的核心.md)
-   [24.6 重点回顾](chapter_24/24.6重点回顾.md)
-   [24.7 本章习题](chapter_24/24.7本章习题.md)
-   [24.8 参考资料与延伸阅读](chapter_24/24.8参考资料与延伸阅读.md)