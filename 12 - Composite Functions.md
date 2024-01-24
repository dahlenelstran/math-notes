#topic

>12.1) Definition^[Lecture 1, 01-14-2024, [[Topology by Munkres]]]: Given functions $f:A \mapsto B$ and $g:A \mapsto B$, we define the **composite** $g \circ f$ of *f* and *g* as the function $g \circ f: A \mapsto C$ defined by the equation $(g \circ f)(a) = g(f(a))$.
>>A formal definition: $g \circ f: A \mapsto C$ is the function whose rule is $\{(a,c) | \text{ For some } b \in B, f(a) = b \text{ and } g(b) = c\}$ 
>>A useful image from [[Topology by Munkres]]: ![[Composite Functions Diagram.png]]
>>Another definition^[Lecture 2, 01-11-2024, [[A Course in Group Theory by Humphreys]]]: Given maps $f: X \mapsto Y$ and $g: Y \mapsto Z$, the composite map $g \circ f: X \mapsto Z$ is defined by $g \circ f(x) = g(f(x))$ for all $x \in X$.

>12.2) Example^[Lecture 2, 01-11-2024, [[A Course in Group Theory by Humphreys]]]: $f_2(a)=a, f_2(b)=a, f_3(a)=b, f_3(b)=b$
>>$f_2 \circ f_3(a) = f_2(b) = a$
>>$f_2 \circ f_3(b) = f_2(b)=a$
>>>Therefore, $f_2 \circ f_3 = f_2$ because they have the same *rule of assignment* ([[11 - Functions (or Maps)]]).

>12.3) Proposition: Given map $f: X \mapsto Y$, $g: Y \mapsto Z$, and $h: Z \mapsto W$ the composite maps $(h \circ g) \circ f: X \mapsto W$ and $h \circ (g \circ f): X \mapsto W$ are equal.
>>Proof: By definition, for all $x \in X$,
>>$$((h \circ g) \circ f)(x) = (h \circ g)(f(x)) = h(g((f(x))) = h(g \circ f(x)) = (h\circ(g\circ f))(x)$$
>>It follows that $(h \circ g) \circ f$ and $h \circ (g \circ f)$ are equal.

