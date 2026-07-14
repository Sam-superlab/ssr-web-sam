---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/06 Operations on Ideals/Radical as an Intersection of Prime Ideals/","dg-note-properties":{}}
---


# Radical as an Intersection of Prime Ideals

For every [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] $\mathfrak a$ of a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|Ring]] $A$,

$$
\sqrt{\mathfrak a}
=
\bigcap_{\substack{\mathfrak p\supseteq\mathfrak a\\
\mathfrak p\text{ prime}}}
\mathfrak p.
$$

In words: the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/06 Operations on Ideals/Radical of an Ideal\|Radical of an Ideal]] is the intersection of all [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/04 Prime and Maximal Ideals/Prime Ideal\|prime ideals]] containing it.

## Proof

Let $\pi:A\to A/\mathfrak a$ be the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Canonical Projection\|Canonical Projection]]. The radical is the inverse image of the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/05 Nilradical and Jacobson Radical/Nilradical\|Nilradical]] of the quotient:

$$
\sqrt{\mathfrak a}
=
\pi^{-1}\!\left(\operatorname{Nil}(A/\mathfrak a)\right).
$$

By Proposition 1.8, the nilradical of $A/\mathfrak a$ is the intersection of all prime ideals of that quotient. The [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]] identifies those primes with the prime ideals of $A$ containing $\mathfrak a$. Taking inverse images gives the formula.

## Consequences

- An ideal is radical exactly when it is an intersection of prime ideals.
- $\sqrt{\mathfrak a}$ is the smallest radical ideal containing $\mathfrak a$.
- Two ideals have the same containing prime ideals exactly when they have the same radical.
- In the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Zariski Topology\|Zariski Topology]], $V(\mathfrak a)=V(\sqrt{\mathfrak a})$; radicals retain vanishing sets while discarding multiplicity.

## Source

- 01_06_operations_on_ideals.pdf, printed p. 9; Proposition 1.14, deduced from Proposition 1.8.

