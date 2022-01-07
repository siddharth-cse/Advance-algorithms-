# Advance-algorithms-
Lecture notes and problems 

# P vs NP hard vs NP complete ?

**P** - Problems that can be solved in polynomial time (Binary Search)  

**NP** - These are the decision problems which can be verified in polynomial time. That means, if I claim that there is a polynomial time solution for a particular problem, you ask me to prove it. Then, I will give you a proof which you can easily verify in polynomial time. These kind of problems are called NP problems. Note that, here we are not talking about whether there is a polynomial time solution for this problem or not. But we are talking about verifying the solution to a given problem in polynomial time.

**NP-Hard** - These are at least as hard as the hardest problems in NP. If we can solve these problems in polynomial time, we can solve any NP problem that can possibly exist. Note that these problems are not necessarily NP problems. That means, we may/may-not verify the solution to these problems in polynomial time.

**NP-Complete** These are the problems which are both NP and NP-Hard. That means, if we can solve these problems, we can solve any other NP problem and the solutions to these problems can be verified in polynomial time.

Reduction - Hard problems that can be reduced to NP-hard problems in polynomial time 

# Lecture 1

## Approximation Algorithms

They are algorithms for NP-hard optimization problems. Since we need to find a polynomial time non-deterministic algorithm before the problem is NP complete. We can find out a non optimal solution for the problems and see how far we are from the optimized solution. (Approximation ratio). With this approximation ration we can make a lower bound (max problems) or an upper bound (for min problems) for how bad the polynomial time algorithm can perform w.r.t to the optimal soltion.

### For maximization problems: 

<img src="https://latex.codecogs.com/svg.latex?\rho=\frac{C*}{C}" title="asdas" /> 

Where C* is the optimal solution for the max problem and C is the solution from the polynomial time Non deterministic algorithm also known as approximation algorithm. 

### For minimzation problems: 

<img src="https://latex.codecogs.com/svg.latex?\rho=\frac{C}{C*}" title="a" />


Where C* is the optimal solution for the max problem and C is the solution from the polynomial time Non deterministic algorithm also known as approximation algorithm. 


### Load Balancing Problem

Load balancing a popular NP hard problem where we have 


<img src="https://latex.codecogs.com/svg.latex?\newline&space;1.We~have~M~identical~machines&space;\newline&space;2.We~have~N~jobs~with~j_1,j_2,j_3...j_n~processing~times" title="\newline 1.~~M~identical~machines \newline 2.~~N~jobs~with~j_1,j_2,j_3...j_n~processing~times" />

We need to find the best way to delegate these jobs to each machine such that the total time to complete all the jobs simultaneously (`makespan`) is minimum. 


# Lecture 4

## Max-flow and Min-cut 

Given a graph G(V,E) where edges have weights representing the capacity of the channel between the two vertices. There is a start vertex S (`source`) and an end vertex T (`sink`). **Max flow** problem tries to preserve the flow value and source and sink vertices i.e incoming flow == outgoing flow. The aim is to maximise the outgoing flow and if 100% flow is preserved then the solution is optimal. 

Intuitively we can form a dual of this problem - **Min-Cut** (In a channel of pipes the avg max flow will be decided by the smallest pipe as it has to pass through this smallest pipe in order to reach the sink) where we seperate the graph into two subset of vertices, where each set must contain either `sink` node or `source` node and not both in the same set. The weights of the edges we cut through that has the least sum, will be the **Max Flow** of the given graph. 
