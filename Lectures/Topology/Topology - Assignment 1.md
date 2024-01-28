#lecture 
>Definition: If both *A* and *B* are sets, *A* is a **proper subset** of *B* if *A* is within *B*, but not equal to it. This is denoted by the subset notation^[[[6 - Notation]]] without the line below it: $A \subset B$. If $A$ is in $B$, but not necessarily not equal to it, then we say it is a **subset** of $B$, denoted by: $A \subseteq B$.  

>Fact: Any set intersected with the empty set is the empty set, and any set unioned with the empty set is itself.

>Definition: The **difference** of two sets, denoted $A - B$ is defined as the set consisting of those elements of A that are not in B, which can be formally represented as $\{A - B = x | x \in A \text{ and } x \not \in B\}$.
>>It can also be referred to as the **complement** of B relative to A

>**Distributive Law**: $A \cup (B \cap C) = (A \cup B) \cap ( A \cup C)$.

>**DeMorgan's Law**: $A - (B \cup C) = (A-B) \cap (A-C)$.

>Definition: A **Powerset** of a set A is the set of A and all subsets of A.

>Definition: given "If P, then Q", then the **contrapositive** is "If not Q, then not P."
>>A logic representation: $P \implies Q$ becomes $\tilde{~} Q \implies \tilde{~} P$

>Definition: given "If P, then Q", then the **converse** is "If Q, then P".
>>A logic representation: $P \implies Q$ becomes $Q \implies P$

>Definition: A **rule of assignment** is a subset *R* of the cartesian product *C* x *D* or two sets, having the property that each element of *C* appears as the first coordinate of at most one ordered pair belonging to *R*.

>Definition: A function^[[[11 - Functions (or Maps)]]] $f: A \mapsto B$ is said to be **injective** (or **one-to-one**) if for each pair of distinct points of *A*, their images (essentially, the output) under *f* are distinct.
>>Formally: $[f(a) = f(a')] \implies [a=a']$
>>Solely depends on the rule of *f*.

>Definition: A function $f: A \mapsto B$ is said to be **surjective** (or **onto**) if every element of *B* is the image of some element of *A* under the function *f*.
>>Formally: $[b \in B] \implies [b = f(a) \text{ for at least one } a \in A]$
>>Depends on the rule of *f*, as well as the range.

>Definition: If a function is both injective and surjective, it is said to be **bijective** (or is referred to as **one-to-one correspondence**).
>>Fact: The composite of two injective functions is injective.
>>Fact: The composite of two surjective functions is surjective.

>Fact: If a given function^[[[11 - Functions (or Maps)]]] *f* is bijective^[[[9 - Injective and Surjective Functions]], then *f* has a unique inverse, denoted by $f^{-1}$ and it is also bijective.

>Definition: the **image set** of *R* is defined as the subset of the domain consisting of all second coordinates of elements of *R*.

>Definition: If *f* is a function mapping *A* to *B*, and if $A_{0}$  is a subset of *A*, we define the **restriction** on *f* to $A_{0}$  to be the function mapping $A_{0}$  into *B* whose rule is $\{(a, f(a) | a \in A_0)\}$
>> It is denoted by *f*|$A_0$, which is read "*f*" restricted to $A_0$.

>Definition: Let $f: A \mapsto B$. If $A_0$ is a subset of *A*, we denote by $f(A_0)$ the set of all images of points of $A_0$ under the function *f*; this set is called the **image** of $A_0$ under *f*.
>>Formally: $f(A_0) = \{b | b = f(a) \text{ for at least one } a \in A_0\}$

>Definition: if $B_0$ is a subset of *B*, we denote by $f^{-1}(B_{0})$ the set of all elements of *A* whose images under *f* lie is $B_0$; it is called the **preimage** of $B_0$ under *f* (or the **counterimage** or the **inverse^[[[8 - Inverse Functions]]] image** of $B_0$).
>>Formally: $f^{-1}(B_0)=\{a | f(a) \in B_0\}$

>Definition: Given functions $f:A \mapsto B$ and $g:A \mapsto B$, we define the **composite** $g \circ f$ of *f* and *g* as the function $g \circ f: A \mapsto C$ defined by the equation $(g \circ f)(a) = g(f(a))$.
>>A formal definition: $g \circ f: A \mapsto C$ is the function whose rule is $\{(a,c) | \text{ For some } b \in B, f(a) = b \text{ and } g(b) = c\}$ 
>>A useful image from [[Topology by Munkres]]: ![[Composite Functions Diagram.png]]

**Date:** January 14, 2024
**Class Page:** [[Topology]]
**Next Assignment:** [[Topology - Assignment 2]]