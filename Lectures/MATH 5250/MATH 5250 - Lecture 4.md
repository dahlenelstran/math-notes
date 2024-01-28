#lecture
>Definition: A subgroup of a group^[[[10 - Groups]]] $G$ is a nonempty subset $H \subset G$ which itself is a group under the same operation as that of $G$. Note that $H \leq G$. 
>>Two easy examples of subgroups existing in all groups: the group itself, and $\{1\}$. 

>Proposition: The following conditions on a subset $H$ of group $G$ are equivalent:
>1. $H$ is a subgroup of $G$.
>2. $H$ satisfies these three requirements:
>	1. the identity element of $G$ is in $H$.
>	2. if $x$ and $y$ are in $H$, so is $xy$.
>	3. if $h$ is in $H$, so is $h^{-1}$. 
>3. $H$ satisfies the conditions:
>	1. the identity element of $G$ is in $H$.
>	2. if $a$ and $b$ are in $H$, so is $ab^{-1}$. 
>>Proof: We must prove that these three statements are equal, and so each statement must imply the other two. Therefore, the proof is split into the following parts:
>>1. ($1 \implies 2$) If  $H$ is a subgroup, it is nonempty and satisfies requirements 2.2 and 2.3. $H$ will also have an identity element $1_H$ such that $1_Hh=h=h1_H$ for all $h \in H$. Since any element $h \in H$ is also in $G$, $h1_G=h=h1_H$. So, by Proposition 10.7^[[[10 - Groups]]], $1_H=1_G$.
>>2. ($2 \implies 3$) Condition 3.1 and condition 2.1 are identical, so we must only prove the others. Let $a,b \in H$. By 2.3, $b^{-1} \in H$, so by 2.2, $ab^{-1} \in H$.
>>3. ($3 \implies 1$) To complete this, we just assume condition 3.1 and 3.2, and prove the four axioms for groups^[[[10 - Groups]]]:
>>	1. Closure: If $x,y \in H$, then $x, y^{-1} \in H$ by the inverse axiom proven below. Then apply condition 3.2 with $a=x, b=y^{-1}$ to obtain that $x(y^{-1})^{-1}=xy \in H$.
>>	2. Associativity: If $x,y,z \in H \subset G$, then, because $G$ is a group, $x(yx)=(xy)z$.
>>	3. Identity: This is held with condition 3.1.
>>	4. Inverse: Consider $h \in H$, and apply condition 3.2 with $a=1, b=h$. Thus $h^{-1} \in H$. 
>
>>Subgroup proofs often use the 2nd set of criteria.
>
>>Note that this proves that all subgroups of a group $G$ at least contain the identity element of $G$.

**Date:** January 23, 2024
**Class Page:** [[MATH 5250 - Modern Algebra]]
**Previous Assignment:** [[MATH 5250 - Lecture 3]]
**Next Assignment:** [[MATH 5250 - Lecture 5]]