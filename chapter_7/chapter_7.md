# 第七章、Linux 磁盘与文件系统管理

系统管理员很重要的任务之一就是管理好自己的磁盘文件系统，每个分区不可太大也不能太小， 太大会造成磁盘容量的浪费，太小则会产生文件无法储存的困扰。此外，我们在前面几章谈到的文件权限与属性中， 这些权限与属性分别记录在文件系统的哪个区块内？这就得要谈到 filesystem 中的 inode 与 block 了。同时，为了虚拟化与大容量磁盘， 现在的 CentOS 7 默认使用大容量性能较佳的 xfs 当默认文件系统了！这也得了解一下。 在本章我们的重点在于如何制作文件系统，包括分区、格式化与挂载等，是很重要的一个章节喔！