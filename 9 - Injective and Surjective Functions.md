#topic

>9.1) Definition^[Lecture 1, 01-14-2024, [[Topology by Munkres]]]: A function $f: A \mapsto B$ is said to be **injective** (or **one-to-one**) if for each pair of distinct points of *A*, their images (essentially, the output) under *f* are distinct  ([[11 - Functions (or Maps)]]).
>>Formally: $[f(a) = f(a')] \implies [a=a']$
>>Solely depends on the rule of *f*.
>>Alternate definition^[Lecture 2, 01-11-2024, [[A Course in Group Theory by Humphreys]]]: $f$ takes distinct values on distinct elements of *A*.

>9.2) Definition^[Lecture 1, 01-14-2024, [[Topology by Munkres]]]: A function $f: A \mapsto B$ is said to be **surjective** (or **onto**) if every element of *B* is the image of some element of *A* under the function *f*.
>>Formally: $[b \in B] \implies [b = f(a) \text{ for at least one } a \in A]$
>>Depends on the rule of *f*, as well as the range.
>>Alternate definition^[Lecture 2, 01-11-2024, [[A Course in Group Theory by Humphreys]]]: for all $y \in Y$, there exists an element $x \in X$ such that $y=f(x)$.

>9.3) Definition^[Lecture 1, 01-14-2024, [[Topology by Munkres]]]: If a function is both injective and surjective, it is said to be **bijective** (or is referred to as **one-to-one correspondence**).
>>Fact: The composite of two injective functions is injective.
>>Fact: The composite of two surjective functions is surjective.

>9.4) Fact^[Lecture 1, 01-14-2024, [[Topology by Munkres]]]: If a given function *f* is bijective, then *f* has a unique inverse, denoted by $f^{-1}$ and it is also bijective ([[8 - Inverse Functions]]).