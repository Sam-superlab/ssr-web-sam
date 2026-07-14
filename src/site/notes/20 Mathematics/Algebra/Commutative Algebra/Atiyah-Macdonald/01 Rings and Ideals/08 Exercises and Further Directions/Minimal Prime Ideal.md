---
{"dg-publish":true,"permalink":"/20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Minimal Prime Ideal/","dg-note-properties":{}}
---


# Minimal Prime Ideal

A **minimal prime ideal** of a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/01 Rings and Ring Homomorphisms/Ring\|Ring]] $A$ is a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/04 Prime and Maximal Ideals/Prime Ideal\|Prime Ideal]] minimal under inclusion among all prime ideals of $A$.

More generally, a prime $\mathfrak p$ is minimal over an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/02 Ideals and Quotient Rings/Ideal\|Ideal]] $\mathfrak a$ if $\mathfrak a\subseteq\mathfrak p$ and no smaller prime still contains $\mathfrak a$.

## Existence

Every prime ideal contains a minimal prime. One applies Zorn's lemma to the set of prime ideals contained in a fixed prime, ordered by reverse inclusion. The intersection of a descending chain of prime ideals is prime: if $xy$ lies in every member and $x$ fails to lie in one member, the chain condition forces $y$ into every sufficiently comparable member and hence into the intersection.

For a nonzero ring, the [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/04 Prime and Maximal Ideals/Maximal Ideal Theorem\|Maximal Ideal Theorem]] provides prime ideals, so minimal primes exist.

## Examples

- In an [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/03 Zero Divisors Nilpotents and Units/Integral Domain\|Integral Domain]], $(0)$ is the unique minimal prime.
- In $k[x,y]/(xy)$, the images of $(x)$ and $(y)$ are the two minimal primes.
- In a [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/05 Nilradical and Jacobson Radical/Reduced Ring\|Reduced Ring]], the intersection of all minimal primes is $(0)$.

## Geometry

The [[20 Mathematics/Algebra/Commutative Algebra/Atiyah-Macdonald/01 Rings and Ideals/08 Exercises and Further Directions/Irreducible Component\|irreducible components]] of $\operatorname{Spec}(A)$ are exactly

$$
V(\mathfrak p)
$$

for the minimal prime ideals $\mathfrak p$.

## Source

- 01_08_exercises.pdf, printed pp. 11 and 13; Exercises 8 and 20(iv).

