#topic
>4.1) Definition^[[[MATH 5450 - Week 1]]]: An $n$th order differential equation is an equation of the form $$P_{0}(t) \frac{d^ny}{dt^n}+P_{1}(t) \frac{d^{n-1}y}{dt^{n-1}} + \dots + P_{n-1}(t)\frac{dy}{dt}+P_{n}(t)y = G(t)$$We assume that the functions $P_0, \dots, P_n,$ and $G$ are continuous, real-valued functions on some interval $I: \alpha < t < \beta$, and that $P_0$ is nowhere zero in this interval. We can then divide that equation by $P_0(t)$, we obtain $$L[y]=\frac{d^ny}{dt^n} + p_{1}(t)\frac{d^{n-1}y}{dt^{n-1}} + \dots + p_{n-1}\frac{dy}{dt} + p_n(t)y=g(t)$$L is referred to as a **linear differential operator**. 

>4.2) Theorem^[[[MATH 5450 - Week 1]]]: If the functions making up an $n$th order differential equation are continuous, then there exists exactly one unique solutions that satisfies the initial conditions. 
>>Proof not provided, but I also think it's not really needed for comprehension. 

>4.3) Definition^[[[MATH 5450 - Week 1]]]: An $n$th order differential equation $L[y]=y^{(n)} + p_1(t)y^{(n-1)}+ \dots + p_{n-1}(t)y' + p_n(t)y =0$ .