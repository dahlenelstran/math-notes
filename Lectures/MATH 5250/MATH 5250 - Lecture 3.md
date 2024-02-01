#lecture 
- [x] Sorted
>Proposition: In any group $G$, there is only one identity element.
>>Proof is obvious.

>Proposition: Every element in a group has a unique inverse.
>>Proof: Supposed that $g$ is an element of a group $G$ with two inverses $g^*$ and $g^{-1}$. This means that $gg^*=1=g^*g$  and $gg^{-1}=1=g^{-1}g$. Then it follows that $g^*(gg^{-1})=g^*1=g^*$. But also, $g^*(gg^{-1})=(g^*g)g^{-1}=g^{-1}1=g^{-1}$. Therefore $g^*=g^{-1}$.

>Proposition: Let $a$ and $b$ be elements of a group $G$. There is a unique element $x \in G$ such that $ax=b$, and there is also a unique element $y \in G$ such that $ya=b$. 
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

>Corollary: Let $a$ and $b$ be elements of a group $G$. Then the inverse of $ab$ is $b^{-1}a^{-1}$.
>>Proof is elementary.

>Proposition: Let $g_1, g_2, \dots$ be elements of a group $G$, and $n \in \mathbb{Z}^+$. Define the set $P_n(g_1,g_2,\dots)$ inductively by $P_n(g_1)=\{g_1\}$ and $P_n(g_1,g_{2})=\{g_1g_{2}\}$ so that $P_n(g_1,g_2,\dots,g_n)=\{xy: x \in P_r(g_1,\dots,g_r) \text{ and } y \in P_s(g_{r+1}, \dots, g_{r+s}) \text{ with } n=r+s\}$. Then $P_n$ consists of a unique element of $G$ which we denote $g_1g_2\dots g_n$.
>>Proof for this is fairly obvious, just use induction, closure, and associativity.

>Definition: Let $g$ be an element of group $G$. Define $g^0=1$, $g^1=g$, and $g^n=gg^{n-1}$. We can also define $g^n$ when $n$ is negative to be the inverse of $g^{n}$. 

>Proposition: Let $g$ be an element of a group $G$ and $r,s \in \mathbb{Z}$. Then
>1. $g^rg^s=g^{r+s}=g^sg^r$
>2. $(g^r)^s=g^{rs}$
>3. $g^{-r}=(g^{(-1)})^r=(g^r)^{-1}$, so that the inverse of $g^r$ is $g^{-r}$.
>>All proofs are relatively simple, but can be found on page 24 for future reference. 
>
>>When applying exponents to groups of elements, like $(xy)^2$, it is important to note that $(xy)^2 \neq x^2y^2$. 

>Definition: Let $g$ be an element of a group $G$. The **order** of $g$ is the smallest positive integer $n$ such that $g^n=1$. If there is no positive integer such that $g^n=1$, then $g$ is said to have infinite order.
>>So the order pretty much denotes how many times you have to multiply $g$ by itself ($n-1$) to get it's inverse. 
>>>Therefore, it is worth noting that if $g$ has order $n$, then $g^{n-1}=g^{-1}$. More generally, any two powers of an element are equal.
>
>>In a finite group, each element has a finite order. Not sure how to explain this one, but it makes sense. Essentially, $g^n$ will reach every element in $G$, which includes $g^{-1}$. 

>Proposition: Let $g$ be an element of order $n$ in a group $G$. Then $g^r=g^s$ if and only if $n$ divides $r-s$. 
>>This proof is elementary.
>
>>Let this proposition speak to the, for lack of better term, cyclic nature of groups, especially finite ones. All elements are connected, and are often different forms of one another. 

>Definition: A relation $R$ on $X$ is an **equivalence relation** on $X$ is $R$ satisfies the following three requirements for all $x,y,z$ in $X$:
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

>Definition: Given an equivalence relation $R$ on a set $X$, the **equivalence class** $[x]_R$ of an element $x$ in $X$ is the set of elements of $X$ related to $x$: $$[x]_r = \{y \in X: (x,y) \in R\}$$
>>>This is also written as $E = \{y|y$ ~$x\}$. 
>>Remark: Because an equivalence relation is symmetric, it does not matter whether we write $(x,y) \in R$ or $(y,x) \in R$. 

>Definition: For any set $X$, a set of non-empty subsets of $X$ is a partition of $X$ if each element of $X$ is in precisely one of the subsets. It follows that the union of the set of subsets is $X$, but the intersection of any two different subsets is the empty set.

>Proposition: The equivalence classes of any equivalence relation on  set $X$ form a partition of the set.
>>Proof: Because $R$ is reflexive, any element $x$ in $X$ is in the equivalence class $[x]_R$ and so the union of all equivalence classes is $X$. If $z$ is in both $[x]_R$ and $[y]_R$, then $xRz$ and $yRz$ by the definition of equivalence classes. Since $R$ is symmetric, we see that $zRy$ and so the fact that $R$ is transitive means that $xRy$. Thus, $y$ is in $[x]_R$ and $yRx$, so that $[x]_R = [y]_R$. 

>Definition: A **congruence class** is the relation of congruence modulo $n$, and is technically an equivalence class^[[[13 - Relations]]]. 
>
>>This is written as $[1]_3$, where this represents all numbers that give remainder $1$ when divided by $3$. 

>Definition:
>1. Addition of Congruence Classes: $$[x]_{n}  +[y]_{n}=[x+y]_{n}$$
>and $$ \text{if } [x_{1}]_{n} = [x_{2}]_{n} \text{ and } [y_{1}]_{n} = [y_{2}]_{n}, \text{ then } [x_{1}+y_{1}]_{n} = [x_{2}+y_{2}]_{n}$$
>2. Multiplication of Congruence Classes: $$[x]_{n}[y]_{n}=[xy]_{n}$$
>and $$ \text{if } [x_{1}]_{n} = [x_{2}]_{n} \text{ and } [y_{1}]_{n} = [y_{2}]_{n}, \text{ then } [x_{1}y_{1}]_{n} = [x_{2}y_{2}]_{n}$$
>>Proof: Suppose that $[x_1]_n=[x_2]_n$ and $[y_1]_n=[y_2]_n$, so that $n$ divides $x_1-x_2$ and also $n$ divides $y_1-y_2$. Thus we have $x_1 - x_2=nr$ and $y_1-y_2=ns$ for some integers $r$ and $s$. Then we have $(x_1+y_1)-(x_2+y_2)=(x_1-x_2)+(y_1-y_2)=n(r+s)$ so that $n$ divides $(x_1+y_1)-(x_2+y_2)$ and so $[x_1+y_1]_n=[x_2+y_2]_n$.
>>The proof for multiplication follows similarly.

>Fact: The set $Z_n$ is an abelian group^[[[10 - Groups]]] under the operation of addition of congruence classes.

**Date:** January 18, 2024
**Class Page:** [[MATH 5250 - Modern Algebra]]
**Previous Lecture:** [[MATH 5250 - Lecture 2]]
**Next Lecture:** [[MATH 5250 - Lecture 4]]