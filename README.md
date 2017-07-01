# 前言

Java语言已经发展了10多年，根据市场反馈，各行各业对Java语言的热度仍然不减，排行上仍然稳居第二，市场上对Java语言学习的热潮仍然没有退去，本项目聚集多个Java开发和架构高手，一起研究和总结JVM的核心技术和关键特性，每个知识点都配以案例和代码，并以文章的形式呈现给大家，最后整理成书，帮助更多的学习Java语言的小伙伴快速掌握Java的要领。

加进来的作者可以自行选择主题，围绕《Java核心要点和最佳实践》，可以独立成章，也可以写一个小节，暂时不用编号，直接按照题目新建文件夹即可。

# 作者

> 33493248@qq.com 李艳鹏 第1章

> jiaboyan@live.com 贾博岩 第2章

> 1428665561@qq.com 梁朋举 第3.1节

> chinazhaoht@gmail.com 赵宏涛 第3.2节

> ycuzjj@163.com 张军军 第3.3节

> jiaboyan@live.com 贾博岩 第3.4节

> 156418415@qq.com 杨彪 第4章

# 阅稿人

N/A

# 目录

## 3 Java并发机制

### 3.1 基础的同步工具

#### 3.1.1 Object类的wait、notify、notifyAll
#### 3.1.2 线程的suspend、resume、fork和join
#### 3.1.3 Synchronized和ReentrantLock
#### 3.1.4 Volatile和Synchronized

### 3.2 高级的同步工具

#### 3.2.1 AQS和Unsafe的park和unpark
#### 3.2.2 CAS
#### 3.2.3 原子变量
#### 3.2.4 Sephemore
- 可用于限流

#### 3.2.5 Barrier
#### 3.2.6 Latch
#### 3.2.7 读写锁

### 3.3 各种各样的锁

#### 3.3.1 锁的本质是排队
- 用排队比喻锁，画一张排队的图比喻锁，锁的排队的空间和时间不一样 

#### 3.3.2 应用层的锁
#### 3.3.3 悲观锁
#### 3.3.4 乐观锁
#### 3.3.5 分布式锁
#### 3.3.6 行级锁

### 3.4 最高境界是无锁

#### 3.4.1 不可变变量
#### 3.4.2 拆分后无竞争
#### 3.4.3 SpinLock
#### 3.4.4 Disruptor RingBuffer

### 3.5 解决棘手的并发问题

#### 3.5.1 热点账户
- 账户热点，分而治之，大而化小，小而化了

#### 3.5.1 使用悲观锁
#### 3.5.1 使用悲观锁和分布式锁
#### 3.5.1 使用悲观锁和信号量
- 外面套分布式锁，降级为本地应用的sephamore

#### 3.5.1 使用行级锁
- 获得余额变动记录需要在同一个事务中再查询一次，比悲观所快一点

#### 3.5.1 使用行级锁和分布式锁
#### 3.5.1 使用行级锁和信号量
#### 3.5.1 账户拆分
- 需要业务逻辑允许

