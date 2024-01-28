#topic
>8.1) Fact^[[Topology - Assignment 1]]: If a given function^[[[11 - Functions (or Maps)]]] *f* is bijective^[[[9 - Injective and Surjective Functions]]], then *f* has a unique inverse, denoted by $f^{-1}$ and it is also bijective.

>8.2) Fact^[[[MATH 5250 - Lecture 2]]]: Given a function $f: X \mapsto Y$, we say that $f$ has an inverse map, $f^{-1}$, if there is a map $g: Y \mapsto X$ such that $g \circ f= {id}_x$ and $f \circ g= {id}_x$.

>8.3) Theorem^[[[MATH 5250 - Lecture 2]]]: If a given map has an inverse, it will be unique. 
>>Proof: Suppose that $g$ and $h$ are both inverses for $f$. This implies $g \circ f = h \circ f = id_x$  and $f \circ g = f \circ h = id_y$. Then $$h = h \circ id_y = h \circ ( f \circ g)
 = (h \circ f) \circ g =id_x \circ g = g$$