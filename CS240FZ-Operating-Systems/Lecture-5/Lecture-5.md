```TOC```
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

### Arrival Pattern 到达模式

用户可能在任何时候使用服务，有可能在晚高峰时期集体打车，有可能通过代理进行，或者成组的在餐厅使用点餐系统。所以用户使用服务的时间既具有随机性，也具有一定的特征。

### Queuing and Dispatch Policy 排队和调度政策
例如，可能有多个队列，VIP 或 FASTPASS 优先级队列或公共/私人队列或其他类型分类（异质性）。如果服务决定它太忙或没有空间容纳队列等，可能会有客户被拒绝的策略。

### Modelling the Arrival and Queuing Process 对到队与排队过程进行建模

在计算机系统中，假设任务的到达模式可能是随机的，单个独立任务 single independent tasks 一次到达一个。许多任务有时可能会一起到达，有时很少，有时甚至可能根本没有到达，但假设任务的到达是完全随机的。出于建模目的，我们让 $\lambda$ 表示在观察期间 observation period 到达此类系统的任务的平均速率。在那个时期有更多任务的概率是多少？我们可能想设计一个系统来应对这样的波动。

预计到达分布 arrive distribution 的一种方法可能是监控系统并注意任务到达之间的时间，然后使用统计技术，将概率公式拟合到数据中，以便我们可以估计在任何给定时间段内到达特定数量的可能性。
例如，[[泊松分布 Poisson Distribution]] 可以与我们向计算机系统描述的到达过程一起使用，以便找到特定数量的任务在给定时间段内到达的概率。

### Queuing Process & Service System





如果服务系统繁忙，则将到达的任务置于排队系统中等待服务。
排队系统可以具有特定的配置和/或约束，例如由单个队列或具有有限资源（空间）的多个队列组成，并根据特定学科进行服务，当资源可用时，根据队列服务策略将任务从队列分派到服务系统。

## Multiprocessor System Organisation

多处理器系统可以由处理器的异构或同构集合组成。
使用同构处理器，所有处理器都可以为单个任务队列提供服务。 同构系统可以使用非对称或对称多处理。

假设泊松到达 Poisson Arrivals 和指数服务分布 Exponential Service Distribution，如果系统任务的平均到达率是 $\lambda$，以及 $\mu$ 是服务率，那么可以证明（通过 Litter's Law）平均停留时间或周转时间 $T$，通过以下公式与 $\lambda$ 和 $\mu$ 关联。
$$T=\frac{1}{\mu-\lambda}$$
> 为了系统可以应对负荷，$\mu$ 必须大于 $\lambda$ 









