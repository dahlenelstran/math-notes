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
>Example^[Lecture 4, 01-23-24, [[Introduction to Analysis by Gaughan]]]: Show $1-\frac{y}{x} \leq ln(x)-ln(y) \leq \frac{x}{y}-1$.
>>Proof: When $y=x$: you are done. 
>>	   When $y < x$: Let $f(t)=ln(t), t \in [y,x]$ so $f$ is continuous on $[y,x]$, and differentiable on $(y,x)$. By the Mean Value Theorem, $\exists \text{ c} \in (y,x)$ such that $f(x)-f(y)=f'(c)(x-y) \implies ln(x) - ln(y) = \frac{1}{c}(x-y)$ .
>>	   $y<c<x$ **CATCH THE REST OF THE EXAMPLE IN THE ONLINE NOTES**

>Example^[Lecture 4, 01-23-24, [[Introduction to Analysis by Gaughan]]]: Let $f:[0,Z] \mapsto \mathbb{R}$ be differentiable, $f(0)=0, f(1)=2, f(2)=2$. Show:
>1. $\exists c_1$ such that $f'(c_1)=0$
>2. $\exists c_2$ such that $f'(c_2)=0$
>3. $\exists c_3$ such that $f'(c_3)=\frac{3}{2}$
>>Proof:  1. By Rolle's Theorem, $\exists f'(c_1)=0$.
>>        2. Also by Rolle's Theorem, $\exists c_2 \in (0,1)$ such that $f(1)-f(0)=f'(c_2)(1-0)$ so we have $2-0=f'(c_2)$, and finally $2=f'(c_2)$.
>>        3. $\exists c_3 \in (c_2, c_1)$ such that $f'(c_3)=\frac{3}{2}$.

## Section 4.4: L'Hospital's Rule and the Inverse-Function Theorem
>Theorem^[Lecture 4, 01-23-24, [[Introduction to Analysis by Gaughan]]]: Let
>1. $f,g$ be continuous on $[a,b]$, and differentiable on $(a,b)$; $g'(x)\neq 0$ on $(a,b)$; $x_0 \in [a,b]$
>2. $f(x_0)=g(x_0)=0$
>3. $\lim_{  x \to x_{0} } \frac{f'(x)}{g'(x)}$ exists
>Then $\lim_{  x \to x_{0} } \frac{f(x)}{g(x)}=\lim_{  x \to x_{0} }\frac{f'(x)}{g'(x)}= \lim_{  x \to x_{0} } \frac{f'(c)}{g'(c)}$ where $c$ is between $x$ and $x_0$. Thus we can write it as follows $\lim_{  x \to x_{0} } \frac{f'(x)}{g'(x)}$.

## Thursday Notes I need to format:
>Theorem^[Lecture 5, 01-25-2024, [[Introduction to Analysis by Gaughan]]]: Suppose $f: [a,b] \mapsto \mathbb{R}$ is continuous and differentiable with $f'(x) \neq 0 \forall x \in [a,b]$. Then $f$ is injective^[[[9 - Injective and Surjective Functions]]], $f^{-1}$ is continuous and differentiable on $f([a,b])$, and $(f^{-1})'(f(x))=\frac{1}{f'(x)}$ for all $x \in [a,b]$.
>
>>Example: Find an equation of the tangent line to the graph of $f^{-1}$ at the point $(1,0)$ if $f(x)=x^3+2x^2-x+1$. 
>>>Note: $(0,1)\inf^{-1} \iff (0,1) \in f$ 
>>>Solution: $f'(x) = 3x^2+4x-1 \rightarrow (f^{-1})'(1)=\frac{1}{f'(0)}=\frac{1}{-1}=-1$. Therefore the tangent line is $$y=(-1)(x-1)$$

## Chapter 5: The Riemann Integral
### The Riemann Integral
>Definition^[Lecture 5, 01-25-2024, [[Introduction to Analysis by Gaughan]]]: Let $a < b$.
>1. $p = \{x_0, x_1, \dots, x_n\}$ is a partition^[[[13 - Relations]]] of $[a,b]$ if $a=x_0<x_1< \dots < x_{n-1} <x_n = b$.
>2. If $P$ and $Q$ are partitions of $[a,b]$ with $P \subset Q$ , then $D$ is called a refinement of $P$. Let $f: [a,b] \mapsto \mathbb{R}$ be bounded, $m \leq f(x) \leq M$, and $p=\{x_0,\dots,x_n\}$ be a partition of [a,b]. For $i=1, 2, \dots, n$ define $M_i(f)=sup\{f(x): x \in [x_{i-1},x_1]\}$ and $m_i(f)=inf\{f(x): x \in [x_{i-1},x_i]\}$. Then $m \leq m_i \leq M_i \leq M$.
>3. Let $U(P,f)=\sum^n_{{i=1}} M_i(f)(x_1-x_{i-1})$, and $L(P,f)=\sum^n_{{i=1}} m_i(f)(x_1-x_{i-1})$, called the upper and lower sum, respectively. So we have $m(b-a) \leq L(P,f) \leq U(P,f) \leq M(b-a)$.

>Definition^[Lecture 5, 01-25-2024, [[Introduction to Analysis by Gaughan]]]: The **upper integral** of $f$ is defined as $\overline{\int}^b_afdx = inf\{U(P,f): \forall \text{ partition } p \text{ of } [a,b]\}$. Similarly, the **lower integral** is defined as $\underline{\int}^b_afdx = sup\{L(P,f): \forall \text{ partition } p \text{ of } [a,b]\}$. 
>==CHECK NOTES==

>Definition^[Lecture 5, 01-25-2024, [[Introduction to Analysis by Gaughan]]]: Let $f: [a,b] \mapsto \mathbb{R}$ be bounded, and $P,Q$ be any partitions of $[a,b]$. Then:
>1. $P \subset Q \implies L(P,f) \leq L(Q,f)$ and $U(P,f) \geq U(Q,f)$
>2. $L(P,f) \leq U(Q,f)$
>3. $\underline{\int}_a^bfdx \leq \overline{\int}^b_afdx$ 
>>Proof: 
>>1. Let $P=\{x_0, x_1, \dots, x_n\}$. 
>>	1. Case 1: $Q$ contains $1$ point not in $P$, say $Q=\{x_0,x_1,\dots,x_{j-1},z,x_j,\dots,x_n\}$. Let $M_i(f)=sup \{f(x): x \in [x_{i-1}, x_i] \}$ and $m_i(f)=inf \{f(x): x \in [x_{i-1}, x_1]\}$. Then let $r_1=sup\{f(x):x \in [x_{j-1},z]\}$ and $r_2=sup\{f(x):x \in [z, x_j] \}$, and $s_1=inf\{f(x):x \in [x_{j-1},x]\}$ and $s_2=inf \{f(x): x \in [z, x_j]\}$. This implies $M_j(f) \geq max\{r_1,r_2\}$, and $m_j(f) \leq min\{s_1,s_2\}$. 