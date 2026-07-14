---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Minimal Prime Ideal/","title":"Minimal Prime Ideal","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"],"dg-note-properties":{"title":"Minimal Prime Ideal","type":"concept","tags":["mathematics/commutative-algebra","mathematics/commutative-algebra/ideals-and-quotients"]}}
---


# Minimal Prime Ideal

A **minimal prime ideal** of a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Foundations and Morphisms/Ring\|Ring]] $A$ is a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Prime Ideal\|Prime Ideal]] minimal under inclusion among all prime ideals of $A$.

More generally, a prime $\mathfrak p$ is minimal over an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Operations/Ideal\|Ideal]] $\mathfrak a$ if $\mathfrak a\subseteq\mathfrak p$ and no smaller prime still contains $\mathfrak a$.

## Existence

Every prime ideal contains a minimal prime. One applies Zorn's lemma to the set of prime ideals contained in a fixed prime, ordered by reverse inclusion. The intersection of a descending chain of prime ideals is prime: if $xy$ lies in every member and $x$ fails to lie in one member, the chain condition forces $y$ into every sufficiently comparable member and hence into the intersection.

For a nonzero ring, the [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Ideals and Quotients/Prime Maximal and Radical Ideals/Krull's Maximal Ideal Theorem\|Krull's Maximal Ideal Theorem]] provides prime ideals, so minimal primes exist.

## Examples

- In an [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Integral Domain\|Integral Domain]], $(0)$ is the unique minimal prime.
- In $k[x,y]/(xy)$, the images of $(x)$ and $(y)$ are the two minimal primes.
- In a [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Rings and Morphisms/Elements and Special Rings/Reduced Ring\|Reduced Ring]], the intersection of all minimal primes is $(0)$.

## Geometry

The [[20 Mathematics/Algebra/Commutative Algebra/Concepts/Spectra and Geometry/Irreducibility/Irreducible Component\|irreducible components]] of $\operatorname{Spec}(A)$ are exactly

$$
V(\mathfrak p)
$$

for the minimal prime ideals $\mathfrak p$.

## Source

- 01_08_exercises.pdf, printed pp. 11 and 13; Exercises 8 and 20(iv).

