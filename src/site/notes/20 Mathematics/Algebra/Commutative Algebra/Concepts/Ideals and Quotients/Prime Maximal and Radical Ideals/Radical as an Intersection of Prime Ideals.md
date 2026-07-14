---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Radical as an Intersection of Prime Ideals/","title":"Radical as an Intersection of Prime Ideals","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Radical as an Intersection of Prime Ideals","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Radical as an Intersection of Prime Ideals

For every [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a$ of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$,

$$
\sqrt{\mathfrak a}
=
\bigcap_{\substack{\mathfrak p\supseteq\mathfrak a\\
\mathfrak p\text{ prime}}}
\mathfrak p.
$$

In words: the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Radical of an Ideal\|Radical of an Ideal]] is the intersection of all [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|prime ideals]] containing it.

## Proof

Let $\pi:A\to A/\mathfrak a$ be the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Canonical Projection\|Canonical Projection]]. The radical is the inverse image of the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Nilradical\|Nilradical]] of the quotient:

$$
\sqrt{\mathfrak a}
=
\pi^{-1}\!\left(\operatorname{Nil}(A/\mathfrak a)\right).
$$

By Proposition 1.8, the nilradical of $A/\mathfrak a$ is the intersection of all prime ideals of that quotient. The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Quotients and Correspondence/Correspondence Theorem for Ideals\|Correspondence Theorem for Ideals]] identifies those primes with the prime ideals of $A$ containing $\mathfrak a$. Taking inverse images gives the formula.

## Consequences

- An ideal is radical exactly when it is an intersection of prime ideals.
- $\sqrt{\mathfrak a}$ is the smallest radical ideal containing $\mathfrak a$.
- Two ideals have the same containing prime ideals exactly when they have the same radical.
- In the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Core/Zariski Topology\|Zariski Topology]], $V(\mathfrak a)=V(\sqrt{\mathfrak a})$; radicals retain vanishing sets while discarding multiplicity.

## Source

- 01_06_operations_on_ideals.pdf, printed p. 9; Proposition 1.14, deduced from Proposition 1.8.

