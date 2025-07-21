---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/10 - Special Ideals and Domains/Prime and Maximal Ideals/"}
---


# Prime and Maximal Ideals

## Introduction

Prime and maximal ideals are special types of ideals that play a crucial role in ring theory. They correspond to integral domains and fields in quotient rings, respectively, and provide important structural information about rings.

## Definitions

**Definition 10.1**: Let $R$ be a commutative ring.

- A proper ideal $P \subset R$ is a **prime ideal** if for any $a, b \in R$, whenever $ab \in P$, then either $a \in P$ or $b \in P$.
- A proper ideal $M \subset R$ is a **maximal ideal** if there is no other ideal $I$ such that $M \subset I \subset R$.

## Characterizations

These definitions have elegant characterizations in terms of quotient rings:

- An ideal $P$ is prime if and only if the quotient ring $R/P$ is an integral domain (a commutative ring with no zero divisors).
- An ideal $M$ is maximal if and only if the quotient ring $R/M$ is a field.

Since every field is an integral domain, it follows that every maximal ideal is also a prime ideal. The converse is not always true; for example, in the ring of integers $\mathbb{Z}$, the ideal $(0)$ is prime but not maximal.

## Examples

### Example 1: Integers

In $\mathbb{Z}$, the prime ideals are $(0)$ and $(p)$ for prime numbers $p$. The maximal ideals are exactly $(p)$ for prime numbers $p$.

### Example 2: Polynomial Rings

In $\mathbb{R}[x]$, the prime ideals are $(0)$ and $(f(x))$ where $f(x)$ is irreducible. The maximal ideals are exactly $(f(x))$ where $f(x)$ is irreducible.

### Example 3: Zero Ideal

The zero ideal $(0)$ is prime if and only if the ring $R$ is an integral domain.

### Example 4: Principal Ideals

In a principal ideal domain, the prime ideals are $(0)$ and $(p)$ where $p$ is a prime element.

## Properties

### Prime Ideals

- The intersection of prime ideals is a radical ideal
- The preimage of a prime ideal under a ring homomorphism is prime
- In a Noetherian ring, every ideal is contained in a maximal ideal

### Maximal Ideals

- Every proper ideal is contained in a maximal ideal (Zorn's Lemma)
- The preimage of a maximal ideal under a surjective ring homomorphism is maximal
- In a commutative ring with identity, maximal ideals are prime

## Applications

### Application 1: Quotient Ring Structure

Prime and maximal ideals determine the structure of quotient rings, which is fundamental in algebra.

### Application 2: Algebraic Geometry

Prime ideals correspond to irreducible varieties in algebraic geometry.

### Application 3: Number Theory

In algebraic number theory, prime ideals generalize the concept of prime numbers.

### Application 4: Field Theory

Maximal ideals are crucial for constructing field extensions through quotient rings.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/9 - Rings and Ideals/Ideals\|Ideals]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/9 - Rings and Ideals/Quotient Rings\|Quotient Rings]]
- [[Integral Domains\|Integral Domains]]
- [[Fields\|Fields]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/9 - Rings and Ideals/Ring Homomorphisms\|Ring Homomorphisms]] 