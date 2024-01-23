#textbook 
## Chapter 4: Differentiation
### Section 4.1: Derivatives
[[1 - Differentiation of Functions]]
[[2 - Continuity of Functions]]
### Section 4.2: The Algebra of Derivatives
[[1 - Differentiation of Functions]]
### @@@go back and finish!!!!! and look at class notes for sure@@@
## Section 4.3: Rolle's Theorem and the Mean Value Theorem
[[1 - Differentiation of Functions]]
[[14 - IVT, MVT, and Rolle's Theorem]]
### Example from today because I need to pay attention lmao
>Example^[Lecture 4, 01-23-24, [[00 - Introduction to Analysis]]]: Show $1-\frac{y}{x} \leq ln(x)-ln(y) \leq \frac{x}{y}-1$.
>>Proof: When $y=x$: you are done. 
>>	   When $y < x$: Let $f(t)=ln(t), t \in [y,x]$ so $f$ is continuous on $[y,x]$, and differentiable on $(y,x)$. By the Mean Value Theorem, $\exists \text{ c} \in (y,x)$ such that $f(x)-f(y)=f'(c)(x-y) \implies ln(x) - ln(y) = \frac{1}{c}(x-y)$ .
>>	   $y<c<x$ **CATCH THE REST OF THE EXAMPLE IN THE ONLINE NOTES**

>Example^[Lecture 4, 01-23-24, [[00 - Introduction to Analysis]]]: Let $f:[0,Z] \mapsto \mathbb{R}$ be differentiable, $f(0)=0, f(1)=2, f(2)=2$. Show:
>1. $\exists c_1$ such that $f'(c_1)=0$
>2. $\exists c_2$ such that $f'(c_2)=0$
>3. $\exists c_3$ such that $f'(c_3)=\frac{3}{2}$
>>Proof:  1. By Rolle's Theorem, $\exists f'(c_1)=0$.
>>        2. Also by Rolle's Theorem, $\exists c_2 \in (0,1)$ such that $f(1)-f(0)=f'(c_2)(1-0)$ so we have $2-0=f'(c_2)$, and finally $2=f'(c_2)$.
>>        3. $\exists c_3 \in (c_2, c_1)$ such that $f'(c_3)=\frac{3}{2}$.

## Section 4.4: L'Hospital's Rule and the Inverse-Function Theorem
>Theorem^[Lecture 4, 01-23-24, [[00 - Introduction to Analysis]]]: Let
>1. $f,g$ be continuous on $[a,b]$, and differentiable on $(a,b)$; $g'(x)\neq 0$ on $(a,b)$; $x_0 \in [a,b]$
>2. $f(x_0)=g(x_0)=0$
>3. $\lim_{  x \to x_{0} } \frac{f'(x)}{g'(x)}$ exists
>Then $\lim_{  x \to x_{0} } \frac{f(x)}{g(x)}=\lim_{  x \to x_{0} }\frac{f'(x)}{g'(x)}= \lim_{  x \to x_{0} } \frac{f'(c)}{g'(c)}$ where $c$ is between $x$ and $x_0$. Thus we can write it as follows $\lim_{  x \to x_{0} } \frac{f'(x)}{g'(x)}$.