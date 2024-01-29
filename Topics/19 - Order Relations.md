#topic 
>19.1) Definition^[[[Topology - Assignment 2]]]: A relation^[[[13 - Relations]]] $C$ on a set $A$ is called an **order relation** (also known as a **simple order** or **linear order**) if it has the following properties:
>1. Comparability: For every $x$ and $y$ in $A$ for which $x \neq y$, either $xCy$ or $yCx$
>2. Nonreflexivity: For no $x$ in $A$ does the relation $xCx$ hold
>3. Transitivity: If $xCy$ and $yCz$, then $xCy$
>>Example: Consider the relation on the real line consisting of all pairs $(x,y)$ of real numbers that $x < y$. It is an order relation, usually called the "usual order relation".
>
>>This is usually denoted by $<$, as to not be confused with equivalence relations

>19.2) Definition^[[[Topology - Assignment 2]]]: An element of a set $X$, call it $a$, is referred to as the **immediate successor** (**immediate predecessor**) of an element in $X$ $b$ if there are no elements in $X$ in $(b,a)$ ($(b,a)$).

>19.3) Definition^[[[Topology - Assignment 2]]]: Suppose that $A$ and $B$ are two sets with order relations $<_A$ and $<_B$. We say that $A$ and $B$ have the same **order type** if there is a bijective correspondence between them that preserves order; that is, if there exists a bijective function $f: A \mapsto B$ such that $a_1 <_A a_2 \implies f(a_1) <_B f(a_2)$. 
>>This is essentially saying that all items $a$ with immediate predecessors and/or successors have it as $f(a)$ as well.
>
>>Example: The interval $(-1,1)$ of real numbers has the same order type as the set $\mathbb{R}$ of real numbers itself, for the function $f: (-1,1) \mapsto \mathbb{R}$ given by $f(x) = \frac{x}{1-x^2}$ is an order-preserving bijective correspondence.
>>>**Ask about this one**

>19.4) Definition^[[[Topology - Assignment 2]]]: Suppose that $A$ and $B$ are two sets with order relations $<_A$ and $<_B$ respectively. Define an order relation $<$ on $A \times B$ by defining $a_1 \times b_1 < a_2 \times b_2$ if $a_1 <_A a_2$ or if $a_1 = a_2$ and $b_1 <_B b_2$. It is called the dictionary order relation on $A \times B$. 
>>I think this is pretty much just giving $a$ all the weight of the relation, and using $b$ as a backup incase they are equal. 
>
>>Example: Consider the dictionary order on the plane $\mathbb{R} \times \mathbb{R}$. In this order, the point $p$ is less than every point lying above it on the vertical line through $p$, and $p$ is less than every point to the right of this vertical line. 