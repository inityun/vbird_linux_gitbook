# 第十六章、程序管理与 SELinux 初探


一个程序被载入到内存当中运行，那么在内存内的那个数据就被称为程序（process）。程序是操作系统上非常重要的概念， 所有系统上面跑的数据都会以程序的型态存在。那么系统的程序有哪些状态？不同的状态会如何影响系统的运行？ 程序之间是否可以互相控管等等的，这些都是我们所必须要知道的项目。 另外与程序有关的还有 SELinux 这个加强文件存取安全性的咚咚，也必须要做个了解呢！