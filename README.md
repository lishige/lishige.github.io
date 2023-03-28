# 个人简介

- 姓： 李
- 名： 世阁
- 昵称： 读书百遍者
- 邮箱：
    - 国内：[lishige@petalmail.com]
    - 国外：[lishige@outlook.com]
# Hadoop
# No-SQL
# Spark
## Spark运行架构特点
1. 每个应用都有自己专属的Executor进程，并且该进程在应用运行期间一直驻留。
   1. Executor进程以多线程的方式运行任务
   2. 减少了多进程任务频繁的启动开销
   3. 使得任务执行变得非常高效和可靠
2. Spark运行过程与资源管理器无关,只要能够获取Executor进程并保持通信就可以
3. Executor上有一个BlockManager存储模块,类似于键盘存储系统
4. 任务采取了数据本地性和推测执行等优化机制
