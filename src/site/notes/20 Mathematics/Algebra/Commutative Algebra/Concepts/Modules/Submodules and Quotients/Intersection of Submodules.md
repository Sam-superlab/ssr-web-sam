---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Intersection of Submodules/","title":"Intersection of Submodules","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"],"dg-note-properties":{"title":"Intersection of Submodules","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/modules"]}}
---


# Intersection of Submodules

For any family $(M_i)_{i\in I}$ of submodules of $M$, the set-theoretic intersection

$$\bigcap_{i\in I}M_i$$

is again a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Submodule\|Submodule]]. It is the largest submodule contained in every $M_i$.

Together with the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Modules/Submodules and Quotients/Sum of Submodules\|Sum of Submodules]], intersections make the submodules of $M$ into a complete lattice. For two submodules, the intersection appears as the obstruction to their sum being direct:

$$M_1+M_2=M_1\oplus M_2\quad\Longleftrightarrow\quad M_1\cap M_2=0.$$

It also controls the canonical isomorphism

$$M_2/(M_1\cap M_2)\cong(M_1+M_2)/M_1.$$

## Source

- `02_03_operations_on_submodules.pdf`, printed p. 19; Proposition 2.1(ii).
