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
在 Queuing Theory 中，建模 modelling 和模拟 simulation 的目的是协助这些服务的管理者如何最好地组织系统。你可以在构建系统之前看看模型的性能。

在计算机系统中，假设任务的到达模式可能是随机的，单个独立任务一次到达一个。 许多任务有时可能会一起到达，有时很少，有时甚至可能根本没有到达，但假设任务的到达是完全随机的。
出于建模目的，我们让 $\lambda$ 表示在观察期间到达此类系统的任务的平均速率。 在那个时期有更多任务的机会是多少？ 我们可能想设计系统来应对波动。


如果服务系统繁忙，则将到达的任务置于排队系统中等待服务。
排队系统可以具有特定的配置和/或约束，例如由单个队列或具有有限资源（空间）的多个队列组成，并根据特定学科进行服务，当资源可用时，根据队列服务策略将任务从队列分派到服务系统。
