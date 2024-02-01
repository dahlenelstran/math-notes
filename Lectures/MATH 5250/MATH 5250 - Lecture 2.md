#lecture 
- [x] Sorted
>Fact: We typically use multiplicative notation with groups, so we omit the composition sign $\circ$.
>>Example: $g \circ h = gh$, or $g \circ g = gg = g^2$
>>Additive Notation would look like this: $g \circ h = g + h$, or $g \circ g = g+g = 2g$.

>Definition: A bijection^[[[9 - Injective and Surjective Functions]]] $\pi$ from a set $X$ to itself is a **permutation** on $X$.
>>Note: It must be a bijection, otherwise not every element would be mapped to exactly one element.

>Fact: The set of all permutations on $X$ is denoted^[[[6 - Notation]]] by $S(X)$.

>Definition: A **map** (or **function**) $f: X \mapsto Y$ is a rule which assigns to each element $x \in X$ to element $f(x) \in Y$.

>Corollary: Let $X$ be any set. Then the set $S(X)$ of permutations $f:X \mapsto X$ is a group^[[[10 - Groups]]] under composition of functions.

>Fact: Given a function $f: X \mapsto Y$, we say that $f$ has an inverse map, $f^{-1}$, if there is a map $g: Y \mapsto X$ such that $g \circ f= {id}_x$ and $f \circ g= {id}_x$.

>Theorem: If a given map has an inverse, it will be unique. 
>>Proof: Suppose that $g$ and $h$ are both inverses for $f$. This implies $g \circ f = h \circ f = id_x$  and $f \circ g = f \circ h = id_y$. Then $$h = h \circ id_y = h \circ ( f \circ g)
 = (h \circ f) \circ g =id_x \circ g = g$$

>Definition: For any set X, the **identity map** is the map ${id}_x: X \mapsto N$ defined by ${id}_x(x)=x$ for all $x \in X$.
>>It is clear from the definition that if $f: X \mapsto Y$ is any map, then $f \circ {id}_x = f$ and ${id}_x \circ f= f$.

>Alternate Injective definition: $f$ takes distinct values on distinct elements of *A*.

>Alternate Surjective definition: for all $y \in Y$, there exists an element $x \in X$ such that $y=f(x)$.

>Another composite function definition: Given maps $f: X \mapsto Y$ and $g: Y \mapsto Z$, the composite map $g \circ f: X \mapsto Z$ is defined by $g \circ f(x) = g(f(x))$ for all $x \in X$.

>Example: $f_2(a)=a, f_2(b)=a, f_3(a)=b, f_3(b)=b$
>>$f_2 \circ f_3(a) = f_2(b) = a$
>>$f_2 \circ f_3(b) = f_2(b)=a$
>>>Therefore, $f_2 \circ f_3 = f_2$ because they have the same *rule of assignment*^[[[11 - Functions (or Maps)]]].

>Proposition: Given map $f: X \mapsto Y$, $g: Y \mapsto Z$, and $h: Z \mapsto W$ the composite maps $(h \circ g) \circ f: X \mapsto W$ and $h \circ (g \circ f): X \mapsto W$ are equal.
>>Proof: By definition, for all $x \in X$,
>>$$((h \circ g) \circ f)(x) = (h \circ g)(f(x)) = h(g((f(x))) = h(g \circ f(x)) = (h\circ(g\circ f))(x)$$
>>It follows that $(h \circ g) \circ f$ and $h \circ (g \circ f)$ are equal.

>Definition: A **relation** on a set $X$ is a subset $R$ of the Cartesian product $X \times X = \{ (x_1, x_2): x_1, x_2 \in X\}$.
>>We will often write $xRy$ to mean that $(x,y)$ is in $R$. This is read as "x is in the relation $R$ to y"^[Lecture 2, 01-24-2024, [[Topology by Munkres]]]. 
>
>>I think about relations as being ways to compare elements in a set, or to map each element to another element in the same set. I'll admit, I'm a little confused on them, so let me find a lot of examples. 
>
>>Example: If $R$ is the relation $<$, then $(3,5)$ is in $R$ because $3<5$ but $(4,3)$ is not because $4 \not < 3$. 
>
>>Example: Given a map $f: X \mapsto X$, we can define a relation $R$ to be the subset of elements of the form $(x,f(x))$. This is also known as the graph of $f$. 
>
>>Example: Let $n$ be an integer greater than 1. The relation on $X = Z$ of congruence modulo^[[[16 - Congruence Modulo N]]] $n$ is defined by $xRy$ if and only if $x \equiv y \mod n$. Thus, two integers $x$ and $y$ are congruent modulo $n$. When $n=2$ there are two congruence classes of integers, those with no remainder when divided by 2, and those with a remainder of 1. 
>>>**Question: Why a relation on $X = Z$? And is this one relation, where we have $(a,b)$ where $a$ is the $x \equiv y$, and $b$ is 0 or 1? Very confused, I need to ask Dr. Barioli.**

**Date:** January 11, 2024
**Class Page:** [[MATH 5250 - Modern Algebra]]
**Previous Lecture:** [[MATH 5250 - Lecture 1]]
**Next Lecture:** [[MATH 5250 - Lecture 3]]