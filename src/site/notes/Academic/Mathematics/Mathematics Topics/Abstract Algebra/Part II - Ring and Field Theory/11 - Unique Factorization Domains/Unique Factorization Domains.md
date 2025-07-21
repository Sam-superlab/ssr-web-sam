---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/11 - Unique Factorization Domains/Unique Factorization Domains/"}
---


# Unique Factorization Domains

## Introduction

The Fundamental Theorem of Arithmetic states that every integer (greater than 1) can be uniquely factored into a product of prime numbers. This property of unique factorization is one of the most important in number theory, and we can generalize it to abstract rings.

## Definition

**Definition 11.1**: An integral domain $R$ is a **Unique Factorization Domain (UFD)** if every non-zero, non-unit element of $R$ can be written as a product of irreducible elements, and this factorization is unique up to the order of the factors and multiplication by units.

An element is **irreducible** if it cannot be factored into a product of two non-units. In a UFD, an element is irreducible if and only if it is prime (an element $p$ is prime if whenever $p$ divides $ab$, then $p$ divides $a$ or $p$ divides $b$).

## Key Properties

1. **Existence of Factorization**: Every non-zero, non-unit element can be written as a product of irreducibles.
2. **Uniqueness of Factorization**: This factorization is unique up to order and units.
3. **Irreducible = Prime**: In a UFD, an element is irreducible if and only if it is prime.

## Relationship to Other Domains

The relationship between the classes of domains introduced so far is a beautiful hierarchy:

$$\text{Euclidean Domains} \implies \text{Principal Ideal Domains} \implies \text{Unique Factorization Domains}$$

Each implication is strict, meaning there are examples of PIDs that are not EDs, and UFDs that are not PIDs. For example, $\mathbb{Z}[x]$ is a UFD but not a PID, as the ideal $(2, x)$ is not principal.

## Examples

### Example 1: The Ring of Integers

The ring $\mathbb{Z}$ is a UFD. Every integer greater than 1 can be uniquely factored into a product of prime numbers. This is the Fundamental Theorem of Arithmetic.

### Example 2: Polynomial Rings over Fields

For any field $F$, the polynomial ring $F[x]$ is a UFD. This is a consequence of the fact that $F[x]$ is a Euclidean domain.

### Example 3: Gaussian Integers

The ring of Gaussian integers $\mathbb{Z}[i] = \{a + bi \mid a, b \in \mathbb{Z}\}$ is a UFD. This allows us to prove results about ordinary integers, such as Fermat's theorem on sums of two squares.

### Example 4: A UFD that is not a PID

The ring $\mathbb{Z}[x]$ is a UFD but not a PID. The ideal $(2, x)$ is not principal, showing that not every UFD is a PID.

## Applications

### Application 1: Number Theory

A classic application of UFDs is in number theory. The ring of Gaussian integers, $\mathbb{Z}[i] = \{a + bi \mid a, b \in \mathbb{Z}\}$, is a Euclidean domain, and therefore a UFD. Studying factorization in this ring allows one to prove results about ordinary integers, such as Fermat's theorem on sums of two squares, which states that an odd prime $p$ can be written as a sum of two squares if and only if $p \equiv 1 \pmod{4}$.

### Application 2: Algebraic Geometry

UFDs are important in algebraic geometry because they correspond to smooth varieties. The coordinate ring of a smooth affine variety is often a UFD.

### Application 3: Cryptography

The unique factorization property is fundamental to many cryptographic protocols, including RSA, which relies on the difficulty of factoring large integers.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/10 - Special Ideals and Domains/Euclidean Domains\|Euclidean Domains]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/10 - Special Ideals and Domains/Principal Ideal Domains\|Principal Ideal Domains]]
- [[Irreducible Elements\|Irreducible Elements]]
- [[Prime Elements\|Prime Elements]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/11 - Unique Factorization Domains/Gauss's Lemma\|Gauss's Lemma]] 