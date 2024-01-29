#topic
>11.1) Definition^[[[MATH 5250 - Lecture 2]]]: A **map** (or **function**) $f: X \mapsto Y$ is a rule which assigns to each element $x \in X$ to element $f(x) \in Y$.

>11.2) Definition^[[[Topology - Assignment 1]]]: A **rule of assignment** is a subset *R* of the cartesian product *C* x *D* or two sets, having the property that each element of *C* appears as the first coordinate of at most one ordered pair belonging to *R*.
>>Note that a rule of assignment $r$ for a function $f: A \mapsto A$ is also a subset of $A \times A$, is considered a relation^[[[13 - Relations]]], just a strict one^[[[Topology - Assignment 2]]].

>11.3) Definition^[[[Topology - Assignment 1]]]: the **image set** of *R* is defined as the subset of the domain consisting of all second coordinates of elements of *R*.

>11.4) Definition^[[[Topology - Assignment 1]]]: If *f* is a function mapping *A* to *B*, and if $A_{0}$  is a subset of *A*, we define the **restriction** on *f* to $A_{0}$  to be the function mapping $A_{0}$  into *B* whose rule is $\{(a, f(a) | a \in A_0)\}$
>> It is denoted by *f*|$A_0$, which is read "*f*" restricted to $A_0$.

>11.5) Definition^[[[Topology - Assignment 1]]]: Let $f: A \mapsto B$. If $A_0$ is a subset of *A*, we denote by $f(A_0)$ the set of all images of points of $A_0$ under the function *f*; this set is called the **image** of $A_0$ under *f*.
>>Formally: $f(A_0) = \{b | b = f(a) \text{ for at least one } a \in A_0\}$ 

>11.6) Definition^[[[Topology - Assignment 1]]]: if $B_0$ is a subset of *B*, we denote by $f^{-1}(B_{0})$ the set of all elements of *A* whose images under *f* lie is $B_0$; it is called the **preimage** of $B_0$ under *f* (or the **counterimage** or the **inverse^[[[8 - Inverse Functions]]] image** of $B_0$).
>>Formally: $f^{-1}(B_0)=\{a | f(a) \in B_0\}$

>11.7) Definition^[[[MATH 5250 - Lecture 2]]]: For any set X, the **identity map** is the map ${id}_x: X \mapsto N$ defined by ${id}_x(x)=x$ for all $x \in X$.
>>It is clear from the definition that if $f: X \mapsto Y$ is any map, then $f \circ {id}_x = f$ and ${id}_x \circ f= f$.