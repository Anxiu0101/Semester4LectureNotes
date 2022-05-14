# Chapter 5

[TOC]

Content: Probability Densities 概率密度

## 5.1 Continuous random variables~连续随机变量~



Suppose we are interested in **the probability that a given continuous random variable will take on a value on the interval==区间== from a to b**==给定的连续随机变量在 a 到 b 区间中的概率==, where a and b are <u>constants</u>==常量== with a ≤ b. 

Suppose, furthermore, that we divide the interval from a to b into m <u>equal subintervals</u>==等长子区间== of width $\Delta x$ containing, respectively==分别==, the points $x_1, x_2, \dots, x_m$, 
And that the probability that the random variable will take on a value in the subinterval containing $x_i$ is given by $f(x_i)\Delta x_i$. Then the probability that the random variable with which we are concerned will take on a value in the interval from a to b is given by, 
$$
P(a \leq X \leq b) = \sum_{i=1}^{m}f(x_i)\Delta x_i
$$
When f is an <u>integrable function</u>==可积函数== defined for all values of the random variable with which we are concerned, we shall define the probability that the value of the random variable falls between a and b by letting $\Delta x \rightarrow 0$. Namely==即==,
$$
P(a \leq X \leq b) = \int_{a}^{b}f(x)dx
$$
![5-1](Chapter-5.assets/image-20220417053035331.png)

The function f are called <u>probability density function or probability density</u> ==概率密度函数或概率密度== 

It is clear that
$$
P(a \leq X \leq b) = P(a \leq X < b) = P(a < X \leq b) = P(a < X < b)
$$
The probability density satisfies:

1. $$
   f(x) \geq 0\ for\ all\ x;
   $$

2. $$
   \int^{\infty}_{-\infty}f(x)dx = 1
   $$

> #### Definition 5.1 
>
> We define the cumulative distribution function (or distribution function) F(x) be the probability that a random variable with the probability density f(x) takes on a value less than or equal to x, that is we let F(x) = P(X≤ x) which is the area under the probability density function over the interval −∞ to x.
> In the usual calculus notation for the integral.

So it's clear that,

1. $$
   F(x) = P(X \leq x) = \int^{x}_{-\infty}f(t)dt
   $$

2. $$
   P(a \leq x \leq b) = \int^{b}_{a}f(x)dx=F(b)-F(a)
   $$

3. $$
   \frac{dF(x)}{dx}=f(x)
   $$

> #### Example 5.1
>
> If a random variable has the probability density
> $$
> f(x) = \left\{
> \begin{aligned}
> &2e^{-2x} &\ x > 0\\
> &0 &\ x\leq 0\\
> \end{aligned}
> \right.
> $$
> find the probabilities that it will take on a value
>
> 1. Between 1 and 3
> 2. Greater that 0.5
> 3. Find the distribution function
> 4. Determine the probability that the random variable will take on a value less than or equal to 1.
>
> 
>
> Solution: 
>
> 1. $$
>    P_1 = F(3) - F(1) = \int_{1}^{3}2e^{-2x}dx=
>    $$
>
> 2. 

> #### Example 5.2
>
> 略

> #### Definition 5.2
>
> The mean of a probability density is defined by
> $$
> \mu = E(x) = \int_{-\infty}^{\infty}xf(x)dx
> $$
> And the variance of a probability density is defined by
> $$
> \sigma^2 = \int_{-\infty}^{\infty}(x-\mu)^2f(x)dx = \int_{-\infty}^{\infty}x^2f(x)dx-\mu^2
> $$


d

a

