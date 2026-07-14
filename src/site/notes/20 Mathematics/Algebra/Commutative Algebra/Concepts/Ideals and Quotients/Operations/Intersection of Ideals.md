---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Intersection of Ideals/","title":"Intersection of Ideals","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Intersection of Ideals","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Intersection of Ideals

The intersection of any family of [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|ideals]] $\{\mathfrak a_i\}_{i\in I}$ in a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is again an ideal:

$$
\bigcap_{i\in I}\mathfrak a_i.
$$

It is the largest ideal contained in every $\mathfrak a_i$.

Together with arbitrary [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Sum of Ideals\|sums]], intersections make the ideals of $A$ a complete lattice under inclusion.

## Examples

- In $\mathbb Z$,

$$
(m)\cap(n)=(\operatorname{lcm}(m,n)).
$$

- $(x)\cap(y)=(xy)$ in $k[x,y]$.
- $\mathfrak a\cap A=\mathfrak a$ and $\mathfrak a\cap(0)=(0)$.

## Relation to products

Always

$$
\mathfrak a\mathfrak b\subseteq\mathfrak a\cap\mathfrak b,
$$

because each generator $ab$ lies in both factors. Equality may fail: in $\mathbb Z$, $(2)(4)=(8)$ but $(2)\cap(4)=(4)$.

If $\mathfrak a$ and $\mathfrak b$ are [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Comaximal Ideal\|comaximal]], then

$$
\mathfrak a\cap\mathfrak b=\mathfrak a\mathfrak b.
$$

This equality is central to the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Chinese Remainder Theorem\|Chinese Remainder Theorem]].

## Source

- 01_06_operations_on_ideals.pdf, printed pp. 6-7 (intersections and the comaximal equality).

