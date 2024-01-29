#topic 
>13.1) Definition^[[[MATH 5250 - Lecture 2]]]: A **relation** on a set $X$ is a subset $R$ of the Cartesian product $X \times X = \{ (x_1, x_2): x_1, x_2 \in X\}$.
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