#lecture 
- [ ] Sorted
>Definition: An $n$th order differential equation is an equation of the form $$P_{0}(t) \frac{d^ny}{dt^n}+P_{1}(t) \frac{d^{n-1}y}{dt^{n-1}} + \dots + P_{n-1}(t)\frac{dy}{dt}+P_{n}(t)y = G(t)$$We assume that the functions $P_0, \dots, P_n,$ and $G$ are continuous, real-valued functions on some interval $I: \alpha < t < \beta$, and that $P_0$ is nowhere zero in this interval. We can then divide that equation by $P_0(t)$, we obtain $$L[y]=\frac{d^ny}{dt^n} + p_{1}(t)\frac{d^{n-1}y}{dt^{n-1}} + \dots + p_{n-1}\frac{dy}{dt} + p_n(t)y=g(t)$$L is referred to as a **linear differential operator**. 

>Theorem: If the functions making up an $n$th order differential equation are continuous, then there exists exactly one unique solutions that satisfies the initial conditions. 
>>Proof not provided, but I also think it's not really needed for comprehension. 

>Definition: An $n$th order differential equation $L[y]=y^{(n)} + p_1(t)y^{(n-1)}+ \dots + p_{n-1}(t)y' + p_n(t)y =0$ is called **homogeneous** because it equals $0$, and not some function of $t$. 

>Theorem: If the functions $p_1,p_2, \dots, p_n$ are continuous on the open interval $I$, if the functions $y_1,y_2, \dots, y_n$ are solutions of the homogeneous differential equation, and if $W(y_1,y_2,\dots,y_n)(t) \neq 0$ for at least one point in $I$, then every solution of the equation can be expressed as a linear combination of the solutions $y_1, y_2, \dots, y_n$.
>>A set of solutions whose Wronskian is nonzero is referred to as a fundamental set of solutions. 

>Theorem: If $y_1(t), \dots, y_n(t)$ is a fundamental set of solutions of a homogeneous differential equation on an interval $I$, then $y_1(t), \dots, y_n(t)$ are linearly independent on $I$. Conversely, if $y_1(t), \dots, y_n(t)$ are linearly independent solutions, then they form a fundamental set of solutions on $I$.

**Date:** January 8, 2024
**Class Page:** [[MATH 5450 - Ordinary Differential Equations]]
**Next Lecture:** [[MATH 5450 - Week 2]]