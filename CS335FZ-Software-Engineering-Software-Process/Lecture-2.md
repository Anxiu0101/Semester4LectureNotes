![](Pasted%20image%2020220314141729.png)
## 一般过程模型中的基本活动

瀑布模型 The Waterfall Model
将基本活动表示为单独的过程阶段，包括需求规范、设计、实施、测试和维护。

渐进式发展 Incremental Development
交错基本活动； 该系统是作为一系列“增量”开发的，每个增量都会为之前的版本添加功能。

集成与配置 Integration & Configuration
依赖于可重用组件的可用性； 系统开发侧重于配置、组合和集成，以便在新环境中使用。

### 瀑布流模型

分为五步：
- Requirements Definition 定义项目需求
	- 收集有关所需功能（例如，软件系统应提供登录功能）和约束（例如，软件系统应使用 PostgreSQL 作为后端数据库，因为它与组织的现有 IT 基础设施兼容）的信息 
	- 在给定一组预算、时间框架、资源、技能和可用技术的情况下，分析软件系统是否可以实现 
	- 创建详细的系统规范
- System & Software Design 系统和软件设计
	- 将需求分配给硬件或软件系统 
	- 建立整体系统架构（例如，识别和描述组件的接口及其关系等）
- Implementation & Unit Testing 实现与单元测试
	- 软件设计被实现为一组程序或程序单元
	- 程序单元经过测试以满足其规范
- Integration & System Testing 集成与系统测试
	- 各个程序单元或程序作为一个完整的系统进行集成和测试
	- 经过验证和验证的软件系统在测试后交付给用户
- Operation & Maintenance 运维
	- 系统部署并投入实际使用
	- 软件系统可能会持续更新以修补错误或安全威胁； 提高系统的稳定性； 或增强系统的功能

- 第一个发布的软件开发过程 
- 源自大型军事系统工程中使用的工程流程 
- 在开始软件开发之前计划和安排所有的过程活动，因此它是一个计划驱动的过程 
- 原则上，在之前的阶段完成之前，不应开始以下阶段。

瀑布流模型是适合使用在嵌入式系统、核心系统、大型软件系统，这些系统中常常需要后期尽可能少的更改，所以适合使用瀑布流模型一次性完成。然而在应对时刻需要变化的系统来说，瀑布流的单向过程的性质使之略显笨拙


### The V-Model

- 由于模型的刚性，简单易管理。Easy to manage.
- 它鼓励在所有阶段进行验证和确认。Encourage validation and check
- 它对开发和测试给予同等重视。Give same weight of development and test
- 但不合适使用在一个中高危险改变的需求场景中
- 不建议在长期的复杂面向对象项目中 Not suggest in complex OO Program

![](Pasted%20image%2020220314144224.png)

V 模式是瀑布流模式的一个改进，它保证测试能及时反馈设计，使得快速应对变化

## Incremental Development 渐进式开发