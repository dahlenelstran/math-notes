#lecture 
- [ ] Sorted
>Definition: Let $f: D \mapsto R$. A point $x_0 \in D$ is a **relative maximum (minimum)** of function^[[[11 - Functions (or Maps)]]] $f$ if and only if there is a neighborhood $Q$ of $x_0$ such that if $x \in Q \cap D$, then $f(x) \leq f(x_0)$ (for a minimum, $f(x) \geq f(x_0)$). 

>1.7) Theorem^[Lecture 4, 01-23-2024, [[MATH 5500 - Introduction to Analysis II]]]:  Suppose $f: [a,b] \mapsto R$ and suppose $f$ has either a relative max or a relative min at $x_0 \in (a,b)$. If $f$ is differentiable at $x_0$, then $f'(x_0)=0$.
>>Proof: Assume $f$ has a relative maximum at $x_0$. Then there is $\delta > 0$ such that, if $x_0-\delta<x<x_0+\delta$, then $x \in [a,b]$ (this is because $x_0 \in (a,b)$. I think, essentially, the $\delta$ covers the spot left by the open interval versus the closed) and $f(x) \leq f(x_0)$. Consider any sequence $\{x_n\}^{\infty}_{n=1}$ converging to $x_0$ such that $x_0-\delta< x_n<x_0$. Then, since $f$ is differentiable at $x_0$, $$\left\{\frac{f(x_n)-f(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$ converges to $f'(x_0)$. But $\frac{f(x_n)-f(x_0)}{x_n-x_0}\geq0$ for each $n$ because $f(x_n) \leq f(x_0)$ and $x_n<x_0$, and hence $f'(x_0) \geq 0$. Consider now a sequence ==FINISH THIS==

**Date:** January 23, 2024
**Class Page:** [[MATH 5500 - Introduction to Analysis II]]
**Previous Lecture:** [[MATH 5500 - Lecture 3]]
**Next Lecture** [[MATH 5500 - Lecture 5]]