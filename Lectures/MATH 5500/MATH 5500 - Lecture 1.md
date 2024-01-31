#lecture 
>Definition: Let $f: D \mapsto R$ with $x_0$ an accumulation point of $D$ and $x_0 \in D$. For each $x \in D$ with $x \neq x_0$, define $T(x)  = \frac{f(x)-f(x_0)}{x-x_0}$. The function^[[[11 - Functions (or Maps)]]] $f$ is said to be **differentiable**^[[[1 - Differentiation of Functions]]] at $x_0$ if and only if $T$ has a limit at $x_0$.
>Alternate Definition: Let $f: D \mapsto R$ with $x_0$ an accumulation point of $D$ and $x_0 \in D$. For each $t \in R$ such that $x_0 + t \in D$ and $t \neq 0$, define $Q(t)=\frac{f(x_0+t)-f(x_0)}{t}$. The function is said to be **differentiable** at $x_0$ if and only if and only if $Q$ has a limit at zero. 
>>Related Definition: If $f$ is differentiable for each $x \in E \subset D$, we say $f$ is **differentiable** on $E$.

>Theorem: Suppose $f: D \mapsto R, x_0 \in D$, and $x_0$ is an accumulation point of $D$. Then $f$ is differentiable at $x_0$ if and only if for every sequence $\{x_n\}^{\infty}_{n=1}$ of points of $D \setminus \{x_0\}$ converging to $x_0$, the sequence $\{\frac{f(x_n)-f(x_0)}{x_n-x_0}\}^{\infty}_{n=1}$ converges to the derivative of $f$ at $x_0$.
>>Proof is not given
>
>>Example: Consider the function $f(x)=|x|$ for all $x \in \mathbb{R}$. Set $x_0=0$, and consider the sequence $\{ \frac{(-1)^n}{n}\}^{\infty}_{n=1}$. This sequence converges to zero, but zero is not term of this sequence. 
>>For *n* even: $\frac{(-1)^n}{n}=\frac{1}{n}$ and $\frac{f(\frac{1}{n})-f(0)}{\frac{1}{n}}=1$, and for *n* odd, $\frac{(-1)^n}{n}=\frac{-1}{n}$ and $\frac{f(-\frac{1}{n})-f(0)}{-\frac{1}{n}}=-1$.
>>Therefore the sequence $\{\frac{f(\frac{(-1)^n}{n})-f(0)}{\frac{(-1)^n}{n}}\}^{\infty}_{n=1}$ does not converge, as it goes to different values as *n* goes to infinity
>
>>More examples can be found in [[Introduction to Analysis by Gaughan]]

>Theorem: Let $f: D \mapsto R$ be differentiable at $x_0$. From this we can conclude that $x_0 \in D$ and that $x_0$ in an accumulation point of $D$. Then $f$ is continuous^[[[2 - Continuity of Functions]]] at $x_0$.
>>Proof: Let $T: D \setminus \{x_0\} \mapsto R$ be defined by $T(x) = \frac{f(x)-f(x_0)}{x-x_0}$.
>>$T$ has a limit at $x_0$ and $\lim_{x \rightarrow x_0} T(x)=f'(x_0)$. For $x \neq x_0$, $f(x)=\frac{f(x)-f(x_0)}{x-x_0}(x-x_0)+f(x_0)=T(x)(x-x_0)+f(x_0)$.]
>>Now $f$ is a sum of two functions, one of which is constant and the other the product of two functions, each of which has a limit at $x_0$. So $f$ has a limit at $x_0$ and $$\lim_{x \rightarrow x_0} f(x)= \lim_{x \rightarrow x_0}[T(x)(x-x_0)+f(x_{0})] = [\lim_{x \rightarrow x_0}T(x)][\lim_{x \rightarrow x_0}(x-x_{0})]+\lim_{x \rightarrow x_0}f(x_0) = f'(x_{0})*0 + f(x_{0})=f(x_{0}).$$
>>Therefore, $f$ has a limit at $x_0$, and it equals $f(x_0)$. 

>Remarks concerning Continuity and Differentiability:
>>$f$ is not continuous^[[[2 - Continuity of Functions]]] at $x_{0}$ $\implies$ $f$ is not differentiable at $x_0$
>
>>$f$ is continuous at $x_0$ $\centernot \implies$ $f$ is differentiable at $x_0$
>
>>$f$ is differentiable at $\forall x \in D$ $\centernot \implies$ $f$ is uniformly continuous on $D$.

## Post Lecture Studies:
>Definition: Let $S$ be a set of real numbers. A real number $A$ is an **accumulation point** of $S$ if and only if every neighborhood of $A$ contains infinitely many points of $S$.  

>Definition: A function $f: D \mapsto \mathbb{R}$ is **uniformly continuous** on $E \subset D$ if and only if for every $\mathcal{E} > 0$, there is $\delta > 0$ such that if $x, y \in E$ with $|x - y| < \delta$, then $|f(x) - f(y)| < \mathcal{E}$.
>>Related definition: If $f$ is uniformly continuous on $D$, we say $f$ is uniformly continuous.

**Date:** January 10, 2024
**Class Page:** [[MATH 5500 - Introduction to Analysis II]]
**Next Lecture:** [[MATH 5500 - Lecture 2]]