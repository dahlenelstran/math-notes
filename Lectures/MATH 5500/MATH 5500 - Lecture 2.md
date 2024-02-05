#lecture 
- [ ] Sorted
>Theorem: Suppose $f, g : D \mapsto R$ are differentiable at $x_0$. Then the following are true:
>1. (Addition Rule) $(f' \pm g')(x_0) = f'(x_0) \pm g'(x_0)$
>2. (Product Rule) $(fg)'(x_0) = f'(x_0)g(x_0)+f(x_0)g'(x_0)$
>3. (Quotient Rule) $(\frac{f}{g})'(x_0)=\frac{f'(x_0)g(x_0)+f(x_0)g'(x_0)}{[g(x_0)]^2}$
>>1. Proof: Let $\{x_n\}^{\infty}_{n=1}$ be any sequence of points in $D \setminus \{x_0\}$ converging to $x_0$. Since $f$ and $g$ are differentiable at $x_0$, $$\left\{\frac{f(x_n)-f(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1} \text{ and } \left\{\frac{g(x_n)-g(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$
>>converse to $f'(x_0) \text{ and } g'(x_0)$ respectively. Thus we have $$\left\{\frac{(f+g)(x_n)-(f+g)(x_0)}{x_n-x_0}\right\}^{\infty}_{n=1} = \left\{\frac{f(x_n)-f(x_0)}{x_{n}-x_{0}} + \frac{g(x_n)-g(x_0)}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$
>>which converges to $f'(x_0)+g'(x_0)$
>
>>2. Proof: By 1.3^[[[1 - Differentiation of Functions]]],  $f$ is continuous at $x_0$, and so $\{f(x_n)\}^{\infty}_{n=1}$ converges to $f(x_0)$. Thus, $$\left\{\frac{(fg)(x_n)-(fg)(x_0)}{x_n-x_0}\right\}^{\infty}_{n=1} = \left\{\frac{f(x_{n})g(x_{n})-f(x_{n})g(x_{0})+f(x_{n})g(x_{0})-f(x_{0})g(x_{0})}{x_{n}-x_{0}}\right\}^{\infty}_{n=1} = \left\{f(x_{n})\frac{g(x_{n})-g(x_{0})}{x_{n}-x_{0}}+g(x_{0})\frac{f(x_{n})-f(x_{0})}{x_{n}-x_{0}}\right\}^{\infty}_{n=1}$$
>>converges to $f(x_0)g'(x_0) +f'(x_0)g(x_0)$.
>>3. Proof: Not given in class

>Theorem (Chain Rule): Let $f: D \mapsto \mathbb{R}$ and $g: D' \mapsto \mathbb{R}$ with $f(D) \subset D'$. Assume $f$ is differentiable at $x_0$ and $g$ is differentiable at $f(x_0)$. Then $g \circ f$^[[12 - Composite Functions]] is differentiable at  $x_0$, and $$(g \circ f)'(x_{0})=g'(f(x_{0}))f'(x_{0})$$
>>Proof: Let $y_0 = f(x_0)$. Define $h(x) \frac{g(y) - g(y_0)}{y-y_0} \text{ if } y \neq y_0 \text{; } g'(y_0) \text{ if }y=y_0$. Then $$\lim_{ y \to y_{0} }h(y) = \lim_{ y \to y_{0} }\frac{g(y) - g(y_0)}{y-y_0} = g'(y_{0})=h(y_{0}) $$
>>So we know $h$ is continuous at $y_0$. So $h \circ f$ is continuous at $x_0$.
>>So then define $T(x)=\frac{f(x)-f(x_0)}{x-x_0}, x \in D, x \neq x_0$. Then $\forall x \neq x_0$, we have $$\frac{(g \circ f)(x)-(g \circ f)(x_0)}{x-x_{0}}=(h \circ f)(x) \cdot T(x)$$
>>>Note that, if $f(x) \neq f(x_0)$, then $\frac{(g \circ f)(x)-(g \circ f)(x_0)}{x-x_{0}}= \frac{(g \circ f)(x)-(g \circ f)(x_0)}{f(x)-f(x_0)} \cdot \frac{f(x)-f(x_0)}{x-x_0}=(h \circ f)(x) \cdot T(x)$ . If $f(x)=f(x_0)$, we have $\frac{(g \circ f)(x)-(g \circ f)(x_0)}{x-x_{0}}=0$, and $(h \circ f)(x) \cdot T(x)=0$. Therefore, the formula is always true. 
>>From the equation, $(g \circ f)'(x_0)=\lim_{x \rightarrow x_0} \frac{(g \circ f)(x)-(g \circ f)(x_0)}{x-x_0} = \lim_{x \rightarrow x_0} [(h \circ f)(x) \cdot T(x)]$ Given our knowledge on composite functions^[[[12 - Composite Functions]]], we know that $\lim_{x \rightarrow x_0} [(h \circ f)(x) \cdot T(x)] = (h \circ f)(x_0) \cdot f'(x_0) = h(f(x_0)) \cdot f'(x_0)=g'(f(x_0)) \cdot f'(x_0)$. 

>Example: Suppose $f: \mathbb{R} \mapsto \mathbb{R}$ is differentiable and defined $g(x)=x^2f(x^3)$. Show that $g$ is differentiable and compute $g'$. 
>>Solution: $x^3$ and $f$ are both differentiable, therefore $f(x^3)$ is differentiable. Because $x^2$ is differentiable, then $x^2f(x^3)$ is also differentiable. Moreover, $g'(x)=2xf(x^3)+x^2f'(x^3)3x^2=2xf(x^3)+3x^4f'(x^3)$. 

>Definition: Let $f: D \mapsto \mathbb{R}$. $x_0 \in D$ is a relative maximum of $f$ if $\exists$ a neighborhood $Q$ of $x_0$ such that $f(x) \leq f(x_0)$ for all $x \in Q \cap D$. 
>>A similar definition can be made for a relative minimum.

>Theorem: Let $f: [a,b] \mapsto \mathbb{R}$, and $f$ has a relative maximum or minimum at $x_0 \in (a,b)$. 
>>Proof: Without loss of generality, assume $x_0$ is a relative minimum of $f$. Then there exists a neighborhood $Q$ of $x_0$ such that $f(x) \geq f(x_0) \forall x \in Q \cap [a,b]$. Because $f'(x_0)$ exists, this implies that $\forall \{x_n\} \subset [a,b], x_n \neq x_0$, as $x_n \rightarrow x_0$, we have $f'(x_0) = \lim_{n \rightarrow \infty} \frac{f(x_n)-f(x_0)}{x_n - x_0}$.
>>Then choose $\{x_n\} \subset Q \cap [a,b], x_n > x_0$, as $x_n \rightarrow x_0$. Then $f(x_n) \geq f(x_0)$, and $f'(x_0) = \lim_{n \rightarrow \infty} \frac{f(x_n) - f(x_0)}{x_n - x_0} \geq 0$. 
>>Choose $\{y_n\} \subset Q \cap [a,b], y_n < x_0, y_n \rightarrow x_0$. Then $f(y_n) \geq f(x_0)$, and $f'(x_0)=\lim_{n \rightarrow \infty} \frac{f(y_n)-f(x_0)}{y_n-x_0} \leq 0$. So $f'(x_0) = 0$. 
>
>>Note: The converse is not true, and if $x_0=a$ or $b$, the conclusion may not be true.

**Date:** January 11, 2024
**Class Page:** [[MATH 5500 - Introduction to Analysis II]]
**Previous Lecture:** [[MATH 5500 - Lecture 1]]
**Next Lecture:** [[MATH 5500 - Lecture 3]]