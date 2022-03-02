# Process Control Block 进程控制块

## Introduction

进程控制块用于跟踪执行上下文(execution context)（有关进程及其活动的所有资源信息），可用于将该进程独立调度(independent scheduling)到任何可用处理器上。

## Construction

A simplified PCD is constructed by this three parts, 

- Process Identification Data 进程识别数据
  - Unique process identifier
  - Owner's user identifier
  - Group identifier
- Processor State 处理器状态
  - CPU Register state
  - Pointers to stack and memory space 堆栈与内存空间的指针
  - Priority 优先级
  - Scheduling parameters 调度参数
  - Events awaited
- Process Control Data 进程控制数据
  - Flags, signals and message
  - Pointers to other processes in the same queue 同一队列中指向其他进程的指针
  - Parent and child linkage pointers
  - Access permissions to I/O object I/O对象的访问权限
  - Accounting information