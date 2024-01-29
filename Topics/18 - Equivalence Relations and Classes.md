#topic 
>18.1) Definition^[[[MATH 5250 - Lecture 3]]]: A relation^[[[13 - Relations]]] $R$ on $X$ is an **equivalence relation** on $X$ is $R$ satisfies the following three requirements for all $x,y,z$ in $X$:
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

>13.3) Definition^[[[MATH 5250 - Lecture 3]]]: Given an equivalence relation $R$ on a set $X$, the **equivalence class** $[x]_R$ of an element $x$ in $X$ is the set of elements of $X$ related to $x$: $$[x]_r = \{y \in X: (x,y) \in R\}$$
>>>This is also written as $E = \{y|y$ ~$x\}$. 
>>Remark: Because an equivalence relation is symmetric, it does not matter whether we write $(x,y) \in R$ or $(y,x) \in R$. 
>
>>Remark^[[[Topology - Assignment 2]]]: Every element of a set $A$ belongs to an equivalence class, and the union of all equivalence classes is equal to $A$.
>>>Example: Consider defining two points equal if they have the same distance from the origin. Thus, each equivalence relation is simply a circle. The union of all circles on the plane, as well as the point itself, makes up the plane. 

>13.4) Lemma^[[[Topology - Assignment 2]]]: Two equivalence classes $E$ and $E'$ are either disjoint or equal.
>>Proof can be found in [[Topology by Munkres]].

>Definition^[[[Topology - Assignment 2]]]: A **partition** of a set $A$ is a collection of disjoint nonempty subsets of $A$ whose union is all of $A$.
>>Studying equivalence relations and partitions is essentially the same thing. 

>13.5) Definition^[[[MATH 5250 - Lecture 3]]]: For any set $X$, a set of non-empty subsets of $X$ is a partition of $X$ if each element of $X$ is in precisely one of the subsets. It follows that the union of the set of subsets is $X$, but the intersection of any two different subsets is the empty set.

>13.6) Proposition^[[[MATH 5250 - Lecture 3]]]: The equivalence classes of any equivalence relation on  set $X$ form a partition of the set.
>>Proof: Because $R$ is reflexive, any element $x$ in $X$ is in the equivalence class $[x]_R$ and so the union of all equivalence classes is $X$. If $z$ is in both $[x]_R$ and $[y]_R$, then $xRz$ and $yRz$ by the definition of equivalence classes. Since $R$ is symmetric, we see that $zRy$ and so the fact that $R$ is transitive means that $xRy$. Thus, $y$ is in $[x]_R$ and $yRx$, so that $[x]_R = [y]_R$. 