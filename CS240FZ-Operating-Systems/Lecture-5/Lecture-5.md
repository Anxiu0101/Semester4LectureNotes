## 本节导读

Scheduling on Multiprocessor Systems 多处理器系统上的调度
- Performance Issues with Multiprocessing 多处理的性能问题
- Queuing Theory 队列理论
- Queue Organization for Multiprocessor Systems 多处理器系统的队列组织

Other Scheduling Environments 
- Distributed Systems 分布式系统
- Real Time Systems 实时系统


## 多处理的性能问题 

使用更多的处理器似乎是提高整个系统吞吐量的明显方法，但是处理器翻倍通常并不能使性能翻倍。
调度问题更加复杂，同样没有一个最佳的解决方案来优化所有情况下的处理器利用率。
对总线、I/O、共享内存、操作系统代码的争夺以及维持高速缓存的一致性都会导致一些 性能滞后。

## Queuing Theory

最大化吞吐量 ==Maximising throughput== 和减少排队时间 ==reducing queuing times== 是许多现实世界服务的共同目标，而不仅仅是计算机系统和解决方案需要应用 Queuing Theory

在对任何系统的性能进行建模和管理时，我们必须解决  
- 任务的到达模式和它们的性质 
- 任务是如何排队和分配的 
- 服务的处理能力

每个现实世界的系统都可能有其独特的到达特征、物理队列配置和服务能力及特征动态。  
排队理论、建模和模拟的目的是协助这些服务的管理者如何最好地组织系统。你可以在构建系统之前看看模型的性能。







