#topic 
>16.1) Definition^[[[MATH 5250 - Lecture 3]]]: A **congruence class** is the relation of congruence modulo $n$, and is technically an equivalence class^[[[13 - Relations]]]. 
>
>>This is written as $[1]_3$, where this represents all numbers that give remainder $1$ when divided by $3$. 

>16.2) Definition^[[[MATH 5250 - Lecture 3]]]:
>1. Addition of Congruence Classes: $$[x]_{n}  +[y]_{n}=[x+y]_{n}$$
>and $$ \text{if } [x_{1}]_{n} = [x_{2}]_{n} \text{ and } [y_{1}]_{n} = [y_{2}]_{n}, \text{ then } [x_{1}+y_{1}]_{n} = [x_{2}+y_{2}]_{n}$$
>2. Multiplication of Congruence Classes: $$[x]_{n}[y]_{n}=[xy]_{n}$$
>and $$ \text{if } [x_{1}]_{n} = [x_{2}]_{n} \text{ and } [y_{1}]_{n} = [y_{2}]_{n}, \text{ then } [x_{1}y_{1}]_{n} = [x_{2}y_{2}]_{n}$$
>>Proof: Suppose that $[x_1]_n=[x_2]_n$ and $[y_1]_n=[y_2]_n$, so that $n$ divides $x_1-x_2$ and also $n$ divides $y_1-y_2$. Thus we have $x_1 - x_2=nr$ and $y_1-y_2=ns$ for some integers $r$ and $s$. Then we have $(x_1+y_1)-(x_2+y_2)=(x_1-x_2)+(y_1-y_2)=n(r+s)$ so that $n$ divides $(x_1+y_1)-(x_2+y_2)$ and so $[x_1+y_1]_n=[x_2+y_2]_n$.
>>The proof for multiplication follows similarly.

>16.3) Fact^[[[MATH 5250 - Lecture 3]]]: The set $Z_n$ is an abelian group^[[[10 - Groups]]] under the operation of addition of congruence classes.