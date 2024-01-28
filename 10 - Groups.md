#topic

## Defining Groups

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

## Consequences of the definitions

>10.5) Proposition^[01-16-2024, Lecture 3, [[A Course in Group Theory by Humphreys]]]: In any group $G$, there is only one identity element.
>>Proof is obvious.

>10.6) Proposition^[01-16-2024, Lecture 3, [[A Course in Group Theory by Humphreys]]]: Every element in a group has a unique inverse.
>>Proof: Supposed that $g$ is an element of a group $G$ with two inverses $g^*$ and $g^{-1}$. This means that $gg^*=1=g^*g$  and $gg^{-1}=1=g^{-1}g$. Then it follows that $g^*(gg^{-1})=g^*1=g^*$. But also, $g^*(gg^{-1})=(g^*g)g^{-1}=g^{-1}1=g^{-1}$. Therefore $g^*=g^{-1}$.

>10.7) Proposition^[01-16-2024, Lecture 3, [[A Course in Group Theory by Humphreys]]]: Let $a$ and $b$ be elements of a group $G$. There is a unique element $x \in G$ such that $ax=b$, and there is also a unique element $y \in G$ such that $ya=b$. 
>>Essentially saying that every element is a multiple or factor of another element.
>
>>Proof: We must prove both that $x$ exists, and that it is unique. 
>>1. Uniqueness: Suppose the equation has two solutions $x$ and $z$, so that $ax=b=az$. By 10.1, $a$ has an inverse, call it $a^{-1}$. Therefore we have $a^{-1}(ax)=a^{-1}(az)$. By associativity, we can get $(a^{-1}a)x)=(a^{-1}a)z)$, so that,because of identity element existence, $x=z$. Therefore $x$ is unique.
>>2. Existence: To prove $x \in G$, we must prove $x=b(a^{-1}) \in G$, and that it satisfies $ax=b$. 
>>	1. By existence of an inverse, we know $a_{-1} \in G$, and $b \in G$ is given. By closure, $b(a^{-1}) \in G$, so $x \in G$. 
>>	2. Let $x=b(a^{-1})$. Then we have $ax=b \rightarrow a(b(a^{-1}))=b$. By associativity, this equals $(aa^{-1})b=b$, and by the identity element existence, $b=b$. 
>>Therefore the proof is complete. 
>
>>Remark: Note that because right and left operations are not necessarily the same, $x=b(a^{-1})$, and $x \neq a^{-1}(b)$.

>10.8) Corollary^[01-16-2024, Lecture 3, [[A Course in Group Theory by Humphreys]]]: Let $a$ and $b$ be elements of a group $G$. Then the inverse of $ab$ is $b^{-1}a^{-1}$.
>>Proof is elementary.

>10.9 Proposition^[01-16-2024, Lecture 3, [[A Course in Group Theory by Humphreys]]]: Let $g_1, g_2, \dots$ be elements of a group $G$. 