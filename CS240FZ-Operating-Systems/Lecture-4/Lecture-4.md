## 本节导读

- Non Preemptive Priority Scheduling using HRN 使用 HRN 的非抢占式优先级调度
- Preemptive Scheduling using RR 使用 RR 的抢占式调度
- Analysis of RR with different quantum lengths 不同量子长度的RR分析
- Multilevel Feedback Queues 多级反馈队列
- Case Study – Traditional Unix Scheduler and Fair Share Scheduler Concept 案例研究——传统的 Unix 调度器和公平共享调度器概念

相应时间 $Response Ratio = (W + S)/S$

抢占式调度 ==Preemptive Scheduling==  
在多任务系统中用作调度基础的一种常见算法类型称为==轮询 Round Robin==。 选择轮循是因为它为所有进程提供了**良好的响应时间** ==good response time to all processes==，这对于在多任务系统中实现令人满意的交互性能很重要。

抢占式调度 Round Robin 是FCFS的一个抢占式版本。每个进程轮流执行，直到它的时间量子过期，强制进行任务上下文切换。时间量子(quantum)可以被改变，以便为特定的工作负载提供最佳结果。

就是在每个进程都运行n个单位的CPU时间，轮流执行直至所有任务完成，每个进程被完成时从其中移出


![](Pasted%20image%2020220309142120.png)