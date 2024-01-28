#topic
>9.1) Definition^[[[Topology - Assignment 1]]]: A function^[[[11 - Functions (or Maps)]]] $f: A \mapsto B$ is said to be **injective** (or **one-to-one**) if for each pair of distinct points of *A*, their images (essentially, the output) under *f* are distinct.
>>Formally: $[f(a) = f(a')] \implies [a=a']$
>>Solely depends on the rule of *f*.
>>Alternate definition^[[[MATH 5250 - Lecture 2]]]: $f$ takes distinct values on distinct elements of *A*.

>9.2) Definition^[[[Topology - Assignment 1]]]: A function $f: A \mapsto B$ is said to be **surjective** (or **onto**) if every element of *B* is the image of some element of *A* under the function *f*.
>>Formally: $[b \in B] \implies [b = f(a) \text{ for at least one } a \in A]$
>>Depends on the rule of *f*, as well as the range.
>>Alternate definition^[[[MATH 5250 - Lecture 2]]]: for all $y \in Y$, there exists an element $x \in X$ such that $y=f(x)$.

>9.3) Definition^[[[Topology - Assignment 1]]]: If a function is both injective and surjective, it is said to be **bijective** (or is referred to as **one-to-one correspondence**).
>>Fact: The composite of two injective functions is injective.
>>Fact: The composite of two surjective functions is surjective.

>9.4) Fact^[[[Topology - Assignment 1]]]: If a given function *f* is bijective, then *f* has a unique inverse^[[[8 - Inverse Functions]]], denoted by $f^{-1}$ and it is also bijective.