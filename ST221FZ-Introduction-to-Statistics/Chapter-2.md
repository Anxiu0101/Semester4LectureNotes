Absolute variation 38 
Arithmetic mean 34 
Bar chart 22
Boxplot 41 
Categorical distribution 24 
Class boundary 26 
Class frequency 25 
Class interval 26 
Class limit 24 
Class mark 26
Coefficient of variation 39 
Cumulative distribution 26 
Density histogram 29 
Deviation from the mean 37 
Dot diagram 23 
Double-stem display 34 
Empirical cumulative distribution 33 
Endpoint convention 25 
Exploratory data analysis 32 
Five-stem display 34
Frequency distribution 24 
Histogram 27 
Interquartile range 41 
Leaf 31 
Maximum 41 
Mean 35 
Median 34 
Minimum 41 
Modified boxplot 41
Numerical distribution 24

## 2.1 Pareto Diagrams and Dot Diagrams

### Pareto Diagrams 帕累托图

帕累托图将根据频率对**每种类型的故障或缺陷进行排序**，可以帮助工程师识别重要缺陷及其原因。 当公司将流程确定为改进的候选时，第一步是收集有关每种故障频率的数据。 例如，计算机控制的车床的性能低于标准，因此工人们会记录以下故障原因及其频率：
 
 | error                  | number |
 |:---------------------- | ------:|
 | power fluctuations     |      6 |
 | controller not stable  |     22 |
 | operator error         |     13 |
 | worn tool not replaced |      2 |
 | other                  |      5 |

由此可以生成帕累托图如下：  
![](Pasted%20image%2020220311083913.png)

图中折现图表示了 defect 的累计百分比，以图形方式描述了帕累托的经验法则，即**任何种类的事件都由几个主要元素和许多次要元素组成。**通常，两个或三个元素将占总频率的一半以上。  

 ### dot diagram 点图
 
作为改进工艺的第二步，收集有关切割速度与控制器设定的目标值的偏差的数据。 (切削速度) - (目标) 的七个观测值，  
![](Pasted%20image%2020220311090255.png)
获得如下点图，  
![](Pasted%20image%2020220311090408.png)

点图直观地总结了车床通常运行速度快的信息。

## 2.2 Frequency Distributions

**频率分布** (Frequency Distributions) 是将一组数据划分为适当数量的类（类别）的表格，还显示了属于每个类的项目数。 该表牺牲了数据中包含的一些信息。 我们不知道每个项目的确切值，而是只知道它属于某个类别。 另一方面，分组通常会带出数据的重要特征，而“易读性”的收益通常会弥补信息的损失。 我们将主要考虑数值分布； 也就是说，数据根据大小分组的频率分布。 如果数据根据某种质量或属性进行分组，我们将这种分布称为分类分布。

构建频率分布的第一步包括决定使用多少类，并为每个类选择**类限制** (class limits) 。 也就是说，决定每个类的范围。 一般来说，我们使用的类的数量取决于观察的数量，但使用少于 5 个或超过 15 个很少是有益的。上限的例外是当数据集的大小为数百甚至是 几千。 它还取决于数据的范围，即最大观测值与最小观测值之间的差异。 设置好类后，我们计算每个类中的观察次数，称为**类频率** class frequencies 。 如果首先将数据从小到大排序，则此任务会得到简化。

这些类不重叠，它们容纳所有数据，并且它们都具有相同的宽度。




