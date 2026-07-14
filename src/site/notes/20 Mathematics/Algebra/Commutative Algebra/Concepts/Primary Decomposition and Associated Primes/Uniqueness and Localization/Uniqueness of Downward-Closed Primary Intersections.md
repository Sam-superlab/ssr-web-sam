---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Uniqueness and Localization/Uniqueness of Downward-Closed Primary Intersections/","title":"Uniqueness of Downward-Closed Primary Intersections","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/primary-decomposition-and-associated-primes"],"dg-note-properties":{"title":"Uniqueness of Downward-Closed Primary Intersections","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/primary-decomposition-and-associated-primes"],"aliases":["Second Uniqueness Theorem for Primary Decomposition"]}}
---


# Uniqueness of Downward-Closed Primary Intersections
Let $\Sigma$ be a set of [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Associated Primes and Components/Associated Prime\|associated primes]] of a decomposable ideal $\mathfrak a$ that is downward closed under inclusion: if $\mathfrak p'\subseteq\mathfrak p$ with $\mathfrak p\in\Sigma$ and $\mathfrak p'$ associated, then $\mathfrak p'\in\Sigma$.

In any [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Primary Ideals and Decompositions/Minimal Primary Decomposition\|Minimal Primary Decomposition]], the intersection of the primary components whose radicals lie in $\Sigma$ is independent of the chosen decomposition.

## Why localization proves it

Take

$$
S=A\setminus\bigcup_{\mathfrak p\in\Sigma}\mathfrak p.
$$

Under [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Localization and Fractions/Core/Localization of a Ring\|localization]], exactly the components indexed by $\Sigma$ survive. Their intersection is therefore the contraction of $S^{-1}\mathfrak a$, which depends only on $\mathfrak a$.

## Consequence

Each component belonging to an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Associated Primes and Components/Minimal Associated Prime\|Minimal Associated Prime]] is unique. Components belonging to [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Primary Decomposition and Associated Primes/Associated Primes and Components/Embedded Prime\|embedded primes]] may vary even though their radicals are fixed.

## Source

- 04_00_primary_decomposition.pdf, A&M Theorem 4.10 and Corollary 4.11, printed p. 54.
