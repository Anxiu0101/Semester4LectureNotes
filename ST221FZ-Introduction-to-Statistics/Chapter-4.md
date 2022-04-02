
## Random variables==随机变量==

A **random variable**==随机变量== is any function that assigns a numerical value to each possible outcome. 随机变量是为每个可能的结果分配数值的任何函数。

The **probability distribution**==概率分布== of a discrete random variable X is a list of the possible values of X together with their probabilities. 离散随机变量 X 的概率分布是 X 的可能值及其概率的列表
$$
f(x) = P[X=x]
$$
The **probability distribution**==概率分布== always satisfies the conditions.

$$
f(x) \geq 0\ and\ \sum_{all\ x}f(x)=1
$$

> Example 4.1 Check whether the following can serve as probability distributions:
>
> 1. $$
>    f(x)=\frac{x-2}{2}\ for\ x=1,2,3,4;
>    $$
>
> 2. $$
>    h(x)=\frac{x^2}{25}\ for\ x=0,1,2,3,4.
>    $$

We define $F(x)=P[X\leq x]\ for\ x\in(-\infty,+\infty)$ to be the **cumulative distribution function**==累积分布函数== or just the **distribution function**==分布函数== of the random variable.



## The Binomial Distribution==二项分布==

Bernoulli trials==伯努利试验== are trials==试验== that satisfies, 

1. There are only two possible outcomes for each trial.
2. The probability of success is the same for each trial.
2. The outcomes from different trials are independent.
2. There are a fixed number==固定数量== $n$ of Bernoulli trials conducted.

> Example 4.2 Can the following be treated as Bernoulli trials? 
> Drivers stopped at a roadblock will be checked for failure to wear a seatbelt. 停在路障前的司机将被检查是否未系安全带。
