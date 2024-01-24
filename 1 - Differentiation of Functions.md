#topic 

>1.1) Definition^[Lecture 1, 01-09-2024, [[Introduction to Analysis by Gaughan]]]: Let $f: D \mapsto R$ with $x_0$ an accumulation point of $D$ and $x_0 \in D$. For each $x \in D$ with $x \neq x_0$, define $T(x)  = \frac{f(x)-f(x_0)}{x-x_0}$. The function $f$ is said to be **differentiable** at $x_0$ if and only if $T$ has a limit at $x_0$ ([[11 - Functions (or Maps)]]).
>Alternate Definition: Let $f: D \mapsto R$ with $x_0$ an accumulation point of $D$ and $x_0 \in D$. For each $t \in R$ such that $x_0 + t \in D$ and $t \neq 0$, define $Q(t)=\frac{f(x_0+t)-f(x_0)}{t}$. The function is said to be **differentiable** at $x_0$ if and only if and only if $Q$ has a limit at zero. 
>>Related Definition: If $f$ is differentiable for each $x \in E \subset D$, we say $f$ is **differentiable** on $E$.

>1.2) Theorem^[Lecture 1, 01-09-2024, [[Introduction to Analysis by Gaughan]]]: Suppose $f: D \mapsto R, x_0 \in D$, and $x_0$ is an accumulation point of $D$. Then $f$ is differentiable at $x_0$ if and only if for every sequence $\{x_n\}^{\infty}_{n=1}$ of points of $D \setminus \{x_0\}$ converging to $x_0$, the sequence $\{\frac{f(x_n)-f(x_0)}{x_n-x_0}\}^{\infty}_{n=1}$ converges to the derivative of $f$ at $x_0$.
>>Proof is not given
>
>>Example: Consider the function $f(x)=|x|$ for all $x \in \mathbb{R}$. Set $x_0=0$, and consider the sequence $\{ \frac{(-1)^n}{n}\}^{\infty}_{n=1}$. This sequence converges to zero, but zero is not term of this sequence. 
>>For *n* even: $\frac{(-1)^n}{n}=\frac{1}{n}$ and $\frac{f(\frac{1}{n})-f(0)}{\frac{1}{n}}=1$, and for *n* odd, $\frac{(-1)^n}{n}=\frac{-1}{n}$ and $\frac{f(-\frac{1}{n})-f(0)}{-\frac{1}{n}}=-1$.
>>Therefore the sequence $\{\frac{f(\frac{(-1)^n}{n})-f(0)}{\frac{(-1)^n}{n}}\}^{\infty}_{n=1}$ does not converge, as it goes to different values as *n* goes to infinity
>
>>More examples can be found in [[Introduction to Analysis by Gaughan]]

>1.3) Theorem^[Lecture 1, 01-09-2024, [[Introduction to Analysis by Gaughan]]]: Let $f: D \mapsto R$ be differentiable at $x_0$. From this we can conclude that $x_0 \in D$ and that $x_0$ in an accumulation point of $D$. Then $f$ is **continuous** at $x_0$ ([[2 - Continuity of Functions]]).
>>Proof: Let $T: D \setminus \{x_0\} \mapsto R$ be defined by $T(x) = \frac{f(x)-f(x_0)}{x-x_0}$.
>>$T$ has a limit at $x_0$ and $\lim_{x \rightarrow x_0} T(x)=f'(x_0)$. For $x \neq x_0$, $f(x)=\frac{f(x)-f(x_0)}{x-x_0}(x-x_0)+f(x_0)=T(x)(x-x_0)+f(x_0)$.]
>>Now $f$ is a sum of two functions, one of which is constant and the other the product of two functions, each of which has a limit at $x_0$. So $f$ has a limit at $x_0$ and $$\lim_{x \rightarrow x_0} f(x)= \lim_{x \rightarrow x_0}[T(x)(x-x_0)+f(x_{0})] = [\lim_{x \rightarrow x_0}T(x)][\lim_{x \rightarrow x_0}(x-x_{0})]+\lim_{x \rightarrow x_0}f(x_0) = f'(x_{0})*0 + f(x_{0})=f(x_{0}).$$
>>Therefore, $f$ has a limit at $x_0$, and it equals $f(x_0)$. 

>1.4) Remarks concerning Continuity and Differentiability^[Lecture 1, 01-09-2024, [[Introduction to Analysis by Gaughan]]]: ([[2 - Continuity of Functions]])
>>$f$ is not continuous at $x_{0}$ $\implies$ $f$ is not differentiable at $x_0$
>
>>$f$ is continuous at $x_0$ $\centernot \implies$ $f$ is differentiable at $x_0$
>
>>$f$ is differentiable at $\forall x \in D$ $\centernot \implies$ $f$ is uniformly continuous on $D$

## Algebra of Derivatives

>1.5) Theorem^[Lecture 2, 01-11-2024, [[Introduction to Analysis by Gaughan]]]: Suppose $f, g : D \mapsto R$ are differentiable at $x_0$. Then the following are true:
>(1: Addition Rule) $(f' \pm g')(x_0) = f'(x_0) \pm g'(x_0)$
>(2: Product Rule) $(fg)'(x_0) = f'(x_0)g(x_0)+f(x_0)g'(x_0)$
>(3: Quotient Rule) $(\frac{f}{g})'(x_0)=\frac{f'(x_0)g(x_0)+f(x_0)g'(x_0)}{[g(x_0)]^2}$
>>(1) Proof: Let $\{x_n\}^{\infty}_{n=1}$ be any sequence of points in $D \setminus \{x_0\}$ converging to $x_0$. Since $f$ and $g$ are differentiable at $x_0$, $$\left\{\frac{f(x_n)-f(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1} \text{ and } \left\{\frac{g(x_n)-g(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$
>>converse to $f'(x_0) \text{ and } g'(x_0)$ respectively. Thus we have $$\left\{\frac{(f+g)(x_n)-(f+g)(x_0)}{x_n-x_0}\right\}^{\infty}_{n=1} = \left\{\frac{f(x_n)-f(x_0)}{x_{n}-x_{0}} + \frac{g(x_n)-g(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$
>>which converges to $f'(x_0)+g'(x_0)$
>
>>(2) Proof: By 1.3 ([[1 - Differentiation of Functions]]),  $f$ is continuous at $x_0$, and so $\{f(x_n)\}^{\infty}_{n=1}$ converges to $f(x_0)$. Thus, $$\left\{\frac{(fg)(x_n)-(fg)(x_0)}{x_n-x_0}\right\}^{\infty}_{n=1} = \left\{\frac{f(x_{n})g(x_{n})-f(x_{n})g(x_{0})+f(x_{n})g(x_{0})-f(x_{0})g(x_{0})}{x_{n}-x_{0}}\right\}^{\infty}_{n=1} = \left\{f(x_{n})\frac{g(x_{n})-g(x_{0})}{x_{n}-x_{0}}+g(x_{0})\frac{f(x_{n})-f(x_{0})}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$
>>converges to $f(x_0)g'(x_0) +f'(x_0)g(x_0)$.
>>(3) Proof: Let $D' = \{x:x \in D \text{ and }g(x) \neq 0\}$. Then $D'$ is the domain of $f / g$, and $x_0$ is an accumulation point 

## Relative Extrema

>1.6) Definition^[Lecture 4, 01-23-2024, [[00 - Introduction to Analysis]]]: Let $f: D \mapsto R$. A point $x_0 \in D$ is a **relative maximum (minimum)** of $f$ if and only if there is a neighborhood $Q$ of $x_0$ such that if $x \in Q \cap D$, then $f(x) \leq f(x_0)$ (for a minimum, $f(x) \geq f(x_0)$). 

>1.7) Theorem^[Lecture 4, 01-23-2024, [[00 - Introduction to Analysis]]]:  Suppose $f: [a,b] \mapsto R$ and suppose $f$ has either a relative max or a relative min at $x_0 \in (a,b)$. If $f$ is differentiable at $x_0$, then $f'(x_0)=0$.
>>Proof: Assume $f$ has a relative maximum at $x_0$. Then there is $\delta > 0$ such that, if $x_0-\delta<x<x_0+\delta$, then $x \in [a,b]$ (this is because $x_0 \in (a,b)$. I think, essentially, the $\delta$ covers the spot left by the open interval versus the closed) and $f(x) \leq f(x_0)$. Consider any sequence $\{x_n\}^{\infty}_{n=1}$ converging to $x_0$ such that $x_0-\delta< x_n<x_0$. Then, since $f$ is differentiable at $x_0$, $$\left\{\frac{f(x_n)-f(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$ converges to $f'(x_0)$. But $\frac{f(x_n)-f(x_0)}{x_n-x_0}\geq0$ for each $n$ because $f(x_n) \leq f(x_0)$ and $x_n<x_0$, and hence $f'(x_0) \geq 0$. Consider now a sequence 