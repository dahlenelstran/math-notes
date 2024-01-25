#topic 
>13.1) Definition^[Lecture 2, 01-11-2024, [[A Course in Group Theory by Humphreys]]]: A **relation** on a set $X$ is a subset $R$ of the Cartesian product $X \times X = \{ (x_1, x_2): x_1, x_2 \in X\}$.
>>We will often write^[[[6 - Notation]]] $xRy$ to mean that $(x,y)$ is in $R$. This is read as "x is in the relation $R$ to y"^[Lecture 2, 01-24-2024, [[Topology by Munkres]]]. 
>
>>I think about relations as being ways to compare elements in a set, or to map each element to another element in the same set. I'll admit, I'm a little confused on them, so let me find a lot of examples. 
>
>>Example: If $R$ is the relation $<$, then $(3,5)$ is in $R$ because $3<5$ but $(4,3)$ is not because $4 \not < 3$. 
>
>>Example: Given a map $f: X \mapsto X$, we can define a relation $R$ to be the subset of elements of the form $(x,f(x))$. This is also known as the graph of $f$. 
>
>>Example: Let $n$ be an integer greater than 1. The relation on $X = Z$ of congruence modulo $n$ is defined by $xRy$ if and only if $x \equiv y \mod n$. Thus, two integers $x$ and $y$ are congruent modulo $n$. When $n=2$ there are two congruence classes of integers, those with no remainder when divided by 2, and those with a remainder of 1. 
>>>**Question: Why a relation on $X = Z$? And is this one relation, where we have $(a,b)$ where $a$ is the $x \equiv y$, and $b$ is 0 or 1? Very confused, I need to ask Dr. Barioli.**

## Equivalence Relations

>13.2) Definition^[Lecture 3, 01-18-2024, [[A Course in Group Theory by Humphreys]]]: A relation $R$ on $X$ is an **equivalence relation** on $X$ is $R$ satisfies the following three requirements for all $x,y,z$ in $X$:
>1. $xRx$ (reflexive property)
>2. if $xRy$ then $yRx$ (symmetric property)
>3. if $xRy$ and $yRz$ then $xRz$ (transitive property)
>>Example: None of the typical relations, $<,>$ , etc., on $\mathbb{R}$ is an equivalence relation because none of them are symmetric.
>
>>Example: The relation of congruence module $n$ is an equivalence relation. 
>>>Proof: 
>>>1. (reflexive) Because $n$ divides 0 (because $0= 0 \times n$), we have $x \equiv x \mod n$. 
>>>2. (symmetric) if $x \equiv y \mod n$, then $n$ divides $x-y$ $k$ times, so that $n$ divides $y-x$ $-k$ times and hence $y \equiv x \mod n$.
>>>3. (transitive) given that $x \equiv y \mod n$ and $y \equiv z \mod n$, then $n$ divides $x-y$ $k_1$ times, and $y+z$ $k_2$ times, and so therefore $n$ must divide $k_1 + k_2 = x - y + y - z = x - z$ therefore we have $x \equiv z \mod n$.

>13.3) Definition^[Lecture 3, 01-18-2024, [[A Course in Group Theory by Humphreys]]]: Given an equivalence relation $R$ on a set $X$, the **equivalence class** $[x]_R$ of an element $x$ in $X$ is the set of elements of $X$ related to $x$: $$[x]_r = \{y \in X: (x,y) \in R\}$$
>>>This is also written^[[[6 - Notation]]] as $E = \{y|y$ ~$x\}$. 
>>Remark: Because an equivalence relation is symmetric, it does not matter whether we write $(x,y) \in R$ or $(y,x) \in R$. 
>
>>Remark^[Lecture 2, 01-24-2-2024, [[Topology by Munkres]]]: Every element of a set $A$ belongs to an equivalence class, and the union of all equivalence classes is equal to $A$.
>>>Example: Consider defining two points equal if they have the same distance from the origin. Thus, each equivalence relation is simply a circle. The union of all circles on the plane, as well as the point itself, makes up the plane. 

>13.4) Lemma^[Lecture 2, 01-24-2-2024, [[Topology by Munkres]]]: Two equivalence classes $E$ and $E'$ are either disjoint or equal.
>>Proof can be found in [[Topology by Munkres]].

>Definition^[Lecture 2, 01-24-2-2024, [[Topology by Munkres]]]: A **partition** of a set $A$ is a collection of disjoint nonempty subsets of $A$ whose union is all of $A$.
>>Studying equivalence relations and partitions is essentially the same thing. 

>13.5) Definition^[Lecture 3, 01-18-2024, [[A Course in Group Theory by Humphreys]]]: For any set $X$, a set of non-empty subsets of $X$ is a partition of $X$ if each element of $X$ is in precisely one of the subsets. It follows that the union of the set of subsets is $X$, but the intersection of any two different subsets is the empty set.

>13.6) Proposition^[Lecture 3, 01-18-2024, [[A Course in Group Theory by Humphreys]]]: The equivalence classes of any equivalence relation on  set $X$ form a partition of the set.
>>Proof: Because $R$ is reflexive, any element $x$ in $X$ is in the equivalence class $[x]_R$ and so the union of all equivalence classes is $X$. If $z$ is in both $[x]_R$ and $[y]_R$, then $xRz$ and $yRz$ by the definition of equivalence classes. Since $R$ is symmetric, we see that $zRy$ and so the fact that $R$ is transitive means that $xRy$. Thus, $y$ is in $[x]_R$ and $yRx$, so that $[x]_R = [y]_R$. 

## Order Relations

>Definition^[Lecture 2, 01-24-2-2024, [[Topology by Munkres]]]: A relation $C$ on a set $A$ is called an **order relation** (also known as a **simple order** or **linear order**) if it has the following properties:
>1. Comparability: For every $x$ and $y$ in $A$ for which $x \neq y$, either $xCy$ or $yCx$
>2. Nonreflexivity: For no $x$ in $A$ does the relation $xCx$ hold
>3. Transitivity: If $xCy$ and $yCz$, then $xCy$
>>Example: Consider the relation on the real line consisting of all pairs $(x,y)$ of real numbers that $x < y$. It is an order relation, usually called the "usual order relation".
>
>>This is usually denoted^[[[6 - Notation]]] by 