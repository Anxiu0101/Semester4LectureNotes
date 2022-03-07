# Process Lifecycle 进程生命周期

## Introduction

PCB 可能在进程生命周期内在不同队列之间移动，具体取决于其执行的优先级(priority)或状态(state)。

队列持有等待不同资源的进程，这些资源使用调度算法(scheduling algorithms)提供服务。
进程的进程控制块(PCB [process control block](process%20control%20block.md))代表操作系统队列之一上的进程。

![进程生命周期](Process%20Lifecycle.assets/image-20220223200244243.png)

![A Simplified Process State Transition](Pasted%20image%2020220302142156.png)
The zombie means that if the process is not killed, it may have remain or even running in CPU.

