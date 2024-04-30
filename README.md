[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/QM7QGF1q)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Consider the following graphs: 

G1 = [
    a -> b, b -> a,
    c -> d, d -> c
]

G2 = [
    v -> y, y -> v, 
    x -> w, w -> x
]

So then we can say:
f(a) = v,
f(b) = y,
f(c) = w,
f(d) = x,

And we can also say: 
$(a, b) \in E_1 \rightarrow (v,y) \in E_2$
$(c, d) \in E_1 \rightarrow (w,x) \in E_2$

So because every vertex in G1 has a corresponding vertex in G2 and for every edge in G1 there is a corresponding edge in G2, we know that G1 and G2 are isomorphic graphs. However, G1 isn't connected since neither a nor b has an edge connecting to either c or b. And G2 isn't connected since neither v nor y has an edge connecting to either x or w. Thus G1 and G2 are not connected and are isomorphic graphs.