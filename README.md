# Advance-algorithms-
Lecture notes and problems 

# NP hard and NP complete ?

# Lecture 1

## Approximation Algorithms

They are algorithms for NP-hard optimization problems. Since we need to find a polynomial time non-deterministic algorithm before the problem is NP complete. We can find out a non optimal solution for the problems and see how far we are from the optimized solution. (Approximation ratio). With this approximation ration we can make a lower bound (max problems) or an upper bound (for min problems) for how bad the polynomial time algorithm can perform w.r.t to the optimal soltion.

### For maximization problems: 

<img src="https://latex.codecogs.com/gif.latex?\rho=\frac{C*}{C}" title="asdas" /> 

Where C* is the optimal solution for the max problem and C is the solution from the polynomial time Non deterministic algorithm also known as approximation algorithm. 

### For minimzation problems: 

<img src="https://latex.codecogs.com/gif.latex?\rho=\frac{C}{C*}" title="a" />


Where C* is the optimal solution for the max problem and C is the solution from the polynomial time Non deterministic algorithm also known as approximation algorithm. 


### Load Balancing Problem

Load balancing a popular NP hard problem where we have 
$`a^2+b^2=c^2`$.

```math
a^2+b^2=c^2
```
