## Program 程序

A program is a collection of instructions specifying a defined sequence of execution. It is the translation of an algorithm into a programming language.

程序是指定定义的执行顺序的指令集合。 它是将算法转换为编程语言。编译器将程序代码映射(maps)为特定处理器的一系列机器指令，这些是存储在目标文件中。

## Process 进程

A process is an instance of a program in action. It is an operating system abstraction. When the instructions are being carried out, a process exists.

进程是正在运行的程序的一个实例。 它是一种操作系统抽象。在执行指令时，存在一个过程。
程序的可执行模块作为程序映像加载到主存储器(main memory)中，处理器从中获取指令。程序映像(program image)具有特定于特定操作系统和处理器的格式，并且包括任何程序参数、堆栈空间、数据空间和程序代码。

进程是一个执行上下文(execution context)，是它运行时所需的内核管理信息(kernel managed information)的集合。
进程是动态实体(dynamic entities)，其生命周期(lifetimes)从几毫秒到几个月不等。
进程可能是持久的(persistent)，实现系统服务。
操作系统本身可能由多个进程组成，例如进程管理器(process manager)、内存管理器(the memory manager)、文件管理器(the file manager)等。

## Processor 处理器

处理器是通过执行存储在内存映像(memory image)中的指令(instructions)来运行进程的代理(agent)。在大多数台式机中，只有一个处理器（有时称为 CPU——中央处理器）。
现代处理器具有多个执行“核心”(cores)，并且能够同时执行多个进程的指令。
