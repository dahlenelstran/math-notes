#topic

> 10.1) Definition^[Lecture 1, 01-09-24, [[A Course in Group Theory by Humphreys]]]: A **group** is a set *G* together with an operation $\circ$ satisfying the following requirements:
>>1. **Closure Axiom**: for each pair $x,y$ of elements of *G*, $x \circ y$ is an element of *G*
>>2. **Associativity Axiom**: for all elements $x, y, z$ of *G*, $(x \circ y) \circ z = x \circ (y \circ z)$
>>3. **Identity Axiom**: there is an element *e* in *G* such that for all *g* in *G* $e \circ g = g = g \circ e$
>>4. **Inverse Axiom**: given an element *g* in *G* such that $g \circ g' = e = g' \circ g$

>10.2) Definition^[Lecture 1, 01-09-24, [[A Course in Group Theory by Humphreys]]]: A group *G* is said to be abelian if for all $x,y$ in *G*, $x \circ y = y \circ x$ . 

>10.3) Definition^[Post-Lecture 1, 01-10-24, [[A Course in Group Theory by Humphreys]]]: The **direct product** of *G* and *H* is the set of ordered pairs $G \times H = \{ (g, h): g \in G, h \in H\}$, under the operation $(g_1, h_1) \circ (g_2, h_2) = (g_1  {\circ}_G  g_2, h_1  {\circ}_H  h_2)$ where ${\circ}_G$ and ${\circ}_H$ denote the operations in *G* and *H*.

>10.4) Fact^[Lecture 2, 01-11-2024, [[A Course in Group Theory by Humphreys]]]: We typically use multiplicative notation with groups, so we omit the composition sign $\circ$ ([[6 - Notation]]).
>>Example: $g \circ h = gh$, or $g \circ g = gg = g^2$
>>Additive Notation would look like this: $g \circ h = g + h$, or $g \circ g = g+g = 2g$

