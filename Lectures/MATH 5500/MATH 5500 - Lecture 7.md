#lecture 
- [ ] Sorted

## Examples:
- Prove $f(x) = 3x^2$ is integrable on $[1,2]$. 
	- $M_i(f)=3x_i^2$,  $m_i(f)=3x_{(i-1)}^2$
	- Let $x_i-x_{i-1} < \delta$. 
	- $U(P,f)-L(P,f)=\sum{_{i=1}^n}(3x_i^2-3_{i-1}^2)(x_i-x_{i-1}) = 3\delta \sum_{i=1}^n(x_i^2-x_{i-1}^2)=3\delta(3)=9 \delta < \epsilon \iff \delta < \frac{\epsilon}{9}$  
	- Proof: $\forall \epsilon > 0$, ==CHECK NOTES==
- Let $f: [0,1] \mapsto \mathbb{R}$ be defined by $f(x) = 0 \text{ if } x \in \mathbb{Q} \text{ ;} 1 \text{ if } x \in \frac{\mathbb{R}}{\mathbb{Q}}$. ==CHECK NOTES==
- Let $f: [0,2] \mapsto \mathbb{R}$ be defined by $f(x) = 1, x \in [0,1] \text{ ;} 2, x \in (1,2]$. Show that $f \in R(x)$ on $[0,2]$ and compute $\int_a^bfdx$.
	- Proof: $\forall \epsilon > 0$, let $P=\{0,1, 1+\epsilon, 2\}$. 
		- $L(P,f)=1+\epsilon + 2(2-(1+\epsilon))=3 - \epsilon$.
		- $U(P,f)=1 + 2\epsilon + 2(2-(1+\epsilon))=3$ 
		- So $U(P,f)-L(P,f)=\epsilon$. Then $f \in R(x)$ on $[0,2]$. Now to compute this integral. $$ 3 - \epsilon \leq \int_a^bfdx \leq 3$$ so $\int^b_a f dx = 3$.
  
## Test Review
- Test covers up to today's section (5.2)
- Test will be definitions, true or false questions (review handout from first day), homework problems (2 from ch5, 4 from ch4)
	- T or F example: Does differentiable imply uniformly continuous? False. Other direction is false as well.
	- 1 q from 4.1 similar to in class example
	- 1 q from 4.4 
	- 2 q from 4.3 

**Date:** February 1, 2024
**Class Page:** [[MATH 5500 - Introduction to Analysis II]]
**Previous Lecture:** [[MATH 5500 - Lecture 6]]
**Next Lecture:** [[MATH 5500 - Lecture 8]]