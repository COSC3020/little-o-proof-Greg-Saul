[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

### little-o proof

Little-o definition </br>
$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$ </br> </br>
Big-O definition </br>
$f(n)\in o(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) \leq c g(n)$ </br> </br>



The little-o definition, says that all elements need to be a positive constant and the big-O definition says that at least one eleement
should be a positive constant. This would imply that if all conditions are met for the little-o definition, then the big-O definition would also be true because there is guaranteed to have at least one positive constant given that little-o requires all parts to be a positive constant.

The inequalities of the relationship between the $f(x)$ and $g(x)$ are another difference. In the little-o definition $f(n) < c g(n)$ and in the big-O definition $f(n) \leq c g(n)$. This implies that the asymptotic time of $f(x)$ will always be less than the time of $g(x)$ in little-o. Since $f(x)$ will always be less than or equal to $g(x)$ in big-O, little-o will always imply big-O because it is a subset of big-O.

I used Zach's repository https://github.com/COSC3020/little-o-proof-ZachRenz to find the definition of big-O notation.













