#topic
## Defining Groups

>10.1) Definition^[[[MATH 5250 - Lecture 1]]]: A **group** is a set *G* together with an operation $\circ$ satisfying the following requirements:
>>1. **Closure Axiom**: for each pair $x,y$ of elements of *G*, $x \circ y$ is an element of *G*
>>2. **Associativity Axiom**: for all elements $x, y, z$ of *G*, $(x \circ y) \circ z = x \circ (y \circ z)$
>>3. **Identity Axiom**: there is an element *e* in *G* such that for all *g* in *G* $e \circ g = g = g \circ e$
>>4. **Inverse Axiom**: given an element *g* in *G* such that $g \circ g' = e = g' \circ g$

>10.2) Definition^[[[MATH 5250 - Lecture 1]]]: A group *G* is said to be abelian if for all $x,y$ in *G*, $x \circ y = y \circ x$ . 

>10.3) Definition^[[[MATH 5250 - Lecture 1]]]: The **direct product** of *G* and *H* is the set of ordered pairs $G \times H = \{ (g, h): g \in G, h \in H\}$, under the operation $(g_1, h_1) \circ (g_2, h_2) = (g_1  {\circ}_G  g_2, h_1  {\circ}_H  h_2)$ where ${\circ}_G$ and ${\circ}_H$ denote the operations in *G* and *H*.

>10.4) Fact^[[[MATH 5250 - Lecture 2]]]: We typically use multiplicative notation with groups, so we omit the composition sign $\circ$.
>>Example: $g \circ h = gh$, or $g \circ g = gg = g^2$
>>Additive Notation would look like this: $g \circ h = g + h$, or $g \circ g = g+g = 2g$.
## Consequences of the definitions

>10.5) Proposition^[[[MATH 5250 - Lecture 3]]]: In any group $G$, there is only one identity element.
>>Proof is obvious.

>10.6) Proposition^[[[MATH 5250 - Lecture 3]]]: Every element in a group has a unique inverse.
>>Proof: Supposed that $g$ is an element of a group $G$ with two inverses $g^*$ and $g^{-1}$. This means that $gg^*=1=g^*g$  and $gg^{-1}=1=g^{-1}g$. Then it follows that $g^*(gg^{-1})=g^*1=g^*$. But also, $g^*(gg^{-1})=(g^*g)g^{-1}=g^{-1}1=g^{-1}$. Therefore $g^*=g^{-1}$.

>10.7) Proposition^[[[MATH 5250 - Lecture 3]]]: Let $a$ and $b$ be elements of a group $G$. There is a unique element $x \in G$ such that $ax=b$, and there is also a unique element $y \in G$ such that $ya=b$. 
>>Essentially saying that every element is a multiple or factor of another element.
>
>>Proof: We must prove both that $x$ exists, and that it is unique. 
>>1. Uniqueness: Suppose the equation has two solutions $x$ and $z$, so that $ax=b=az$. By 10.1, $a$ has an inverse, call it $a^{-1}$. Therefore we have $a^{-1}(ax)=a^{-1}(az)$. By associativity, we can get $(a^{-1}a)x)=(a^{-1}a)z)$, so that, because of identity element existence, $x=z$. Therefore $x$ is unique.
>>2. Existence: To prove $x \in G$, we must prove $x=b(a^{-1}) \in G$, and that it satisfies $ax=b$. 
>>	1. By existence of an inverse, we know $a_{-1} \in G$, and $b \in G$ is given. By closure, $b(a^{-1}) \in G$, so $x \in G$. 
>>	2. Let $x=b(a^{-1})$. Then we have $ax=b \rightarrow a(b(a^{-1}))=b$. By associativity, this equals $(aa^{-1})b=b$, and by the identity element existence, $b=b$. 
>>Therefore the proof is complete. 
>
>>Remark: Note that because right and left operations are not necessarily the same, $x=b(a^{-1})$, and $x \neq a^{-1}(b)$.

>10.8) Corollary^[[[MATH 5250 - Lecture 3]]]: Let $a$ and $b$ be elements of a group $G$. Then the inverse of $ab$ is $b^{-1}a^{-1}$.
>>Proof is elementary.

>10.9) Proposition^[[[MATH 5250 - Lecture 3]]]: Let $g_1, g_2, \dots$ be elements of a group $G$, and $n \in \mathbb{Z}^+$. Define the set $P_n(g_1,g_2,\dots)$ inductively by $P_n(g_1)=\{g_1\}$ and $P_n(g_1,g_{2})=\{g_1g_{2}\}$ so that $P_n(g_1,g_2,\dots,g_n)=\{xy: x \in P_r(g_1,\dots,g_r) \text{ and } y \in P_s(g_{r+1}, \dots, g_{r+s}) \text{ with } n=r+s\}$. Then $P_n$ consists of a unique element of $G$ which we denote $g_1g_2\dots g_n$.
>>Proof for this is fairly obvious, just use induction, closure, and associativity.

>10.10) Definition^[[[MATH 5250 - Lecture 3]]]: Let $g$ be an element of group $G$. Define $g^0=1$, $g^1=g$, and $g^n=gg^{n-1}$. We can also define $g^n$ when $n$ is negative to be the inverse of $g^{n}$. 

>10.11) Proposition^[[[MATH 5250 - Lecture 3]]]: Let $g$ be an element of a group $G$ and $r,s \in \mathbb{Z}$. Then
>1. $g^rg^s=g^{r+s}=g^sg^r$
>2. $(g^r)^s=g^{rs}$
>3. $g^{-r}=(g^{(-1)})^r=(g^r)^{-1}$, so that the inverse of $g^r$ is $g^{-r}$.
>>All proofs are relatively simple, but can be found on page 24 for future reference. 
>
>>When applying exponents to groups of elements, like $(xy)^2$, it is important to note that $(xy)^2 \neq x^2y^2$. 

>10.12) Definition^[[[MATH 5250 - Lecture 3]]]: Let $g$ be an element of a group $G$. The **order** of $g$ is the smallest positive integer $n$ such that $g^n=1$. If there is no positive integer such that $g^n=1$, then $g$ is said to have infinite order.
>>So the order pretty much denotes how many times you have to multiply $g$ by itself ($n-1$) to get it's inverse. 
>>>Therefore, it is worth noting that if $g$ has order $n$, then $g^{n-1}=g^{-1}$. More generally, any two powers of an element are equal.
>
>>In a finite group, each element has a finite order. Not sure how to explain this one, but it makes sense. Essentially, $g^n$ will reach every element in $G$, which includes $g^{-1}$. 

>10.13) Proposition^[[[MATH 5250 - Lecture 3]]]: Let $g$ be an element of order $n$ in a group $G$. Then $g^r=g^s$ if and only if $n$ divides $r-s$. 
>>This proof is elementary.
>
>>Let this proposition speak to the, for lack of better term, cyclic nature of groups, especially finite ones. All elements are connected, and are often different forms of one another. 
