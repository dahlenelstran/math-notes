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
>>So then define $T(x)=\frac{f(x)-f(x_0)}{x-x_0}, x \in D, x \neq x_0$. Then $\forall x \neq x_0$, we have $$\frac{(g \circ f)(x)-(g \circ f)(x_0)}{x-x_{0}}=(h \circ f)(x) \times T(x)$$ >Note that, if $f(x) \neq f(x_0)$, 

**Date:** January 11, 2024
**Class Page:** [[MATH 5500 - Introduction to Analysis II]]
**Previous Lecture:** [[MATH 5500 - Lecture 1]]
**Next Lecture:** [[MATH 5500 - Lecture 3]]