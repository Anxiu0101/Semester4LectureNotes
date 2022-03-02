## 操作系统的作用

操作系统的一项基本任务是进程管理——创建、控制、终止——管理执行环境(Execution Environment)
操作系统必须为进程分配(allocate)内存空间和CPU时间等资源，它必须保护资源免受其他进程活动的影响，并在共享相同资源的进程之间提供同步机制(synchronisation mechanisms)。

为了完成这个基本任务，操作系统使用数据结构(data structures)来表示它正在处理的进程对象的状态。
对于每个进程，操作系统都维护一个进程控制块 ([[process control block]], PCB) 或进程描述符(process descriptor)，以清楚地了解每个进程正在做什么、它在执行过程中达到了什么点以及分配(assigned)了哪些资源。