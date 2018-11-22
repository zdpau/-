# - 网上学到的一些知识
## 一，gossip 算法
### http://www.docin.com/p-1425281621.html （论文，有讲解历史）
### https://www.cnblogs.com/dyf6372/p/3528193.html  https://www.cnblogs.com/xingzc/p/6165084.html （两个基本相同，讲得比较细）
### https://blog.csdn.net/frankchina/article/details/51385367 https://my.oschina.net/u/3705388/blog/1631251 （两篇比较短，但有用）
### http://www.cnblogs.com/HouZhiHouJueBlogs/articles/4741203.html （讲了一些函数定义）

## 二，什么是wall-clock time
#### wall clock time or wall time is a measure of how much real time that elapses from start to end, including time that passes due to programmed (artificial) delays or waiting for resources to become available.
#### In computing, wall clock time[1] is the actual time taken by a computer to complete a task. It is the sum of three terms: CPU time, I/O time, and the communication channel delay (e.g. if data are scattered on multiple machines). In contrast to CPU time, which measures only the time during which the processor is actively working on a certain task, wall time measures the total time for the process to complete. The difference between the two consists of time that passes due to programmed delays or waiting for resources to become available

## 三、infiniband
InfiniBand架构是一种支持多并发链接的“转换线缆”技术，它是新一代服务器硬件平台的I/O标准。由于它具有高带宽、低延时、 高可扩展性的特点，它非常适用于服务器与服务器（比如复制，分布式工作等），服务器和存储设备（比如SAN和直接存储附件）以及服务器和网络之间（比如LAN， WANs和the Internet）的通信 。

目的是为了取代PCI成为系统互连的新技术标准，其核心就是将I/O系统从服务器主机中分离出来。

## 四，Discrete event simulation（DES）离散时间仿真 https://zhuanlan.zhihu.com/p/22689081
先说仿真，仿真就是模拟，是应用模型对现实事物的再认识。仿真的目的是为了认清事物。仿真分两种：

* 一种是认识事物的外在表现，比如售楼处的微缩沙盘，汽车设计时电脑中的3D模型，展示微观世界的短片等等。这些仿真手法解决了观察事物外观的种种困难，带我们看清了“庐山真面目”。

* 另外一种仿真是为了认识事物的内在规律，这一类仿真的范围其实更加宽泛。比如细胞实验模拟了细胞中的环境，能够帮助认识药物代谢的规律。飞机模拟驾驶，让操作人员在安全的虚拟环境中认识系统操作的方法。宏观经济学模型，研究国民生产总值、利率、失业率等市场指标的相互作用。这些仿真手法，让我们能够预见事物的发展方向，得以“一叶而知秋”。

那离散事件仿真（Discrete Event Simulation，缩写为DES）是什么呢？它首先关注的是事物的内在规律。我们把这些字拆开来看下：

* “Discrete”是离散，在一个离散的系统中，我们总是能够找到一个时间点来标注系统的变化，比如研究对象进入系统和离开系统的时间点，进入队列和离开队列的时间点，开始加工和完成加工的时间点等等。这些时间点在时间轴上是离散而非连续的，而系统状态仅在离散的时间点上发生变化。

* “Event”是抽象的事件，就是我们在时间轴上标记的一系列事件。这些事件所发生的时间或是我们提前制定好的，或是受到其他事件的影响而发生，或是在某些条件到达的时刻发生。总之，一定能根据规律找到事件发生的那个时时间点，而这些时间点，就是我们预测系统变化的依据。

* “Simulation”就是属于前文提到的第二种仿真，就是实现预测的方法。

** 离散事件仿真就是根据事件在离散的时间点上变化的规律，来预测系统变化的方法。**  



