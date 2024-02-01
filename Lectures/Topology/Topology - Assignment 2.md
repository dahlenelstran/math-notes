#lecture 
- [x] Sorted
>Note that a rule of assignment $r$ for a function $f: A \mapsto A$ is also a subset of $A \times A$, is considered a relation^[[[13 - Relations]]], just a strict one.

>Remark: Every element of a set $A$ belongs to an equivalence class, and the union of all equivalence classes is equal to $A$.
>>Example: Consider defining two points equal if they have the same distance from the origin. Thus, each equivalence relation is simply a circle. The union of all circles on the plane, as well as the point itself, makes up the plane. 

>Lemma: Two equivalence classes $E$ and $E'$ are either disjoint or equal.
>>Proof can be found in [[Topology by Munkres]].

>Definition: A **partition** of a set $A$ is a collection of disjoint nonempty subsets of $A$ whose union is all of $A$.
>>Studying equivalence relations and partitions is essentially the same thing. 

>Definition: A relation $C$ on a set $A$ is called an **order relation** (also known as a **simple order** or **linear order**) if it has the following properties:
>1. Comparability: For every $x$ and $y$ in $A$ for which $x \neq y$, either $xCy$ or $yCx$
>2. Nonreflexivity: For no $x$ in $A$ does the relation $xCx$ hold
>3. Transitivity: If $xCy$ and $yCz$, then $xCy$
>>Example: Consider the relation on the real line consisting of all pairs $(x,y)$ of real numbers that $x < y$. It is an order relation, usually called the "usual order relation".
>
>>This is usually denoted by $<$, as to not be confused with equivalence relations

>Definition: An element of a set $X$, call it $a$, is referred to as the **immediate successor** (**immediate predecessor**) of an element in $X$ $b$ if there are no elements in $X$ in $(b,a)$ ($(b,a)$).

>Definition: Suppose that $A$ and $B$ are two sets with order relations $<_A$ and $<_B$. We say that $A$ and $B$ have the same **order type** if there is a bijective correspondence between them that preserves order; that is, if there exists a bijective function $f: A \mapsto B$ such that $a_1 <_A a_2 \implies f(a_1) <_B f(a_2)$. 
>>This is essentially saying that all items $a$ with immediate predecessors and/or successors have it as $f(a)$ as well.
>
>>Example: The interval $(-1,1)$ of real numbers has the same order type as the set $\mathbb{R}$ of real numbers itself, for the function $f: (-1,1) \mapsto \mathbb{R}$ given by $f(x) = \frac{x}{1-x^2}$ is an order-preserving bijective correspondence.
>>>**Ask about this one**

>Definition: Suppose that $A$ and $B$ are two sets with order relations $<_A$ and $<_B$ respectively. Define an order relation $<$ on $A \times B$ by defining $a_1 \times b_1 < a_2 \times b_2$ if $a_1 <_A a_2$ or if $a_1 = a_2$ and $b_1 <_B b_2$. It is called the dictionary order relation on $A \times B$. 
>>I think this is pretty much just giving $a$ all the weight of the relation, and using $b$ as a backup incase they are equal. 
>
>>Example: Consider the dictionary order on the plane $\mathbb{R} \times \mathbb{R}$. In this order, the point $p$ is less than every point lying above it on the vertical line through $p$, and $p$ is less than every point to the right of this vertical line. 

>Definition: We say that a subset $A_0$ of $A$ is **bounded above** if there is an element $b$ of $A$ such that $x \leq b$ for every $x \in A_0$; the element $b$ is called an **upper bound** for $A_0$. If the set of all upper bounds for $A_0$ has a smallest element, that element is called the **least upper bound**, or the **supremum**, of $A_0$.
>>This is written as $sup_{A_0}$ 
>>The same thing can be said for subsets **bounded below**, and the element is referred to as the **infimum**.

>Definition: An ordered set $A$ is said to have the **least upper bound property** if every nonempty subset $A_0$ of $A$ that is bounded above has a least upper bound.
>>The same thing can be said for the **greatest lower bound property**.

**Date:** January 18, 2024
**Class Page:** [[Topology]]
**Previous Assignment:** [[Topology - Assignment 1]]
**Next Assignment:** [[Topology - Assignment 3]]