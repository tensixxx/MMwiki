## Introduction
A **mathematical model** is an idealization of the real-world phenomenon, which will never be completely accurate. However, it is still a good way to help us understand the world through valuable results and conclusions.
### Simplification
Models, approximate real-world behavior, simplify reality. 
Simplifying relationship: **proportionality**
![[Figure 1.png]]
**Definition**: Two variables *y* and *x* are **proportional** (to each other) if the ratio is a nonzero constant. 
$$y = kx$$ We write *y ∝ x*.

**Geometric meaning**: 
The graph of *y* versus *x* is a straight line pass through the origin.

### Modeling Change
Modeling change formula: 
$$ change = future value - present value$$
### Modeling Change with Difference Equations
**Definition**: For a sequence of numbers, the ***n*th first difference** is the difference between the *n*th term and the _(n+1)_ th term. $A = \{a_0, a_1, a_2, a_3, \dots a_n\}$, the ***n*th first difference** is:
$$
\Delta a_n = a_{n+1} - a_n
$$
### Approximating Change with Difference Equations
In many cases, mathematical descriptions of change are not exact. We observe patterns in the data and approximate the change mathematically by using
$$
change = \Delta a_n = some\ function\ f
$$
#### Discrete Versus Continuous Change
Some change takes place in discrete time intervals and the other change happens continuously. Difference equations represents change in discrete time intervals. For some continuous condition, we use difference equation to approximate, which is an example of model simplification. 
### Solutions to Dynamical Systems
**Definition**: A **dynamical system** is a relationship involving time period. 
#### The Method of Conjecture
**Definition**: The method of conjecture is a reasoning guess (conjecture) of relationship or formula to a dynamical system based on observed data. 

The conjectured formula has to be tested and accepted or rejected based on it satisfy the system or not. 

The formula for the linear dynamical system is 
$$ a_n = r ^ n a_0
$$
where $a_0$ is a given initial value. It can also be written as 
$$
a_{n+1}  = ra_n$$
For some special values, if *r* = 0, then the sequence are zero. If r = 1, then $a_{n+1} = a_n$ . If *r* > 1, $a_{n+1}  = ra_n$ . If *r* is negative, the graph oscillates between positive and negative values. If |*r*| < 1, when n approaches to infinity, $a_n$ approaches to zero. 

Adding a constant term *b* to the dynamical system formula shown previously. We get $a_{n+1} = ra_n + b$. In this a dynamical system $a_{n+1} = f(a_n)$, if value x satisfy $x = f(x)$, then *x* is called an **equilibrium value** or **fixed point**. 

The formula of the equilibrium value for the dynamical system is$$ a = \frac b {1 - r}$$where *r* $\neq$ 1. 