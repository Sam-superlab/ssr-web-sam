---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/12 - Polynomial Rings/Polynomial Rings/"}
---


# Polynomial Rings and Factorization

## Introduction

A central question in ring theory is whether properties of a ring $R$ are inherited by the polynomial ring $R[x]$. For unique factorization, the answer is yes, and this provides a powerful tool for understanding the structure of polynomial rings.

## Gauss's Lemma and its Consequences

### Statement

**Theorem 12.1 (Gauss's Lemma and its Corollary)**: If $R$ is a UFD, then the polynomial ring $R[x]$ is also a UFD.

### Proof Strategy

The proof of this cornerstone result is non-trivial. It involves several key steps:

1. **Content of a Polynomial**: Define the content of a polynomial as the greatest common divisor of its coefficients.
2. **Primitive Polynomials**: A polynomial is primitive if its content is a unit.
3. **Gauss's Lemma**: The product of two primitive polynomials is primitive.
4. **Lifting Factorization**: Relate factorization in $R[x]$ to factorization in $F[x]$, where $F$ is the field of fractions of $R$.

### Key Definitions

- **Content**: For a polynomial $f(x) = a_n x^n + \cdots + a_1 x + a_0 \in R[x]$, the content $\text{cont}(f)$ is $\gcd(a_0, a_1, \ldots, a_n)$.
- **Primitive Polynomial**: A polynomial $f(x) \in R[x]$ is primitive if $\text{cont}(f)$ is a unit in $R$.

### Gauss's Lemma

**Lemma 12.2 (Gauss's Lemma)**: The product of two primitive polynomials is primitive.

This lemma is the key technical result that allows us to lift factorization from the field of fractions back to the original ring.

### Consequences

This theorem is immensely powerful as it provides a vast supply of UFDs. For example:
- Since $\mathbb{Z}$ is a UFD, so is $\mathbb{Z}[x]$
- By induction, polynomial rings in any number of variables over a UFD are also UFDs
- Examples: $\mathbb{Z}[x_1, \ldots, x_n]$, $F[x_1, \ldots, x_n]$ for a field $F$

## Eisenstein's Criterion

To work with these polynomial rings, we need practical tools to determine if a polynomial is irreducible.

### Statement

**Theorem 12.3 (Eisenstein's Criterion)**: Let $R$ be a UFD with field of fractions $F$. Let $f(x) = a_n x^n + \cdots + a_1 x + a_0$ be a polynomial in $R[x]$. If there exists a prime element $p \in R$ such that:

1. $p$ divides $a_i$ for all $i \in \{0, 1, \ldots, n-1\}$
2. $p$ does not divide $a_n$
3. $p^2$ does not divide $a_0$

then $f(x)$ is irreducible over the field of fractions $F$.

### Examples

**Example 1**: The polynomial $f(x) = x^5 + 6x^3 + 9x + 3$ is irreducible over $\mathbb{Q}$ by Eisenstein's criterion with $p = 3$.

**Example 2**: The cyclotomic polynomial $\Phi_p(x) = \frac{x^p - 1}{x - 1} = x^{p-1} + \cdots + x + 1$ is irreducible over $\mathbb{Q}$ for any prime $p$. While the criterion does not apply to $\Phi_p(x)$ directly, it applies to $\Phi_p(x+1)$, which is sufficient to prove the irreducibility of the original polynomial.

## Irreducibility Tests

### Rational Root Test

**Theorem 12.4 (Rational Root Test)**: Let $f(x) = a_n x^n + \cdots + a_1 x + a_0$ be a polynomial with integer coefficients. If $\frac{p}{q}$ is a rational root of $f(x)$ in lowest terms, then $p$ divides $a_0$ and $q$ divides $a_n$.

### Reduction Modulo p

**Theorem 12.5**: Let $f(x) \in \mathbb{Z}[x]$ be a monic polynomial. If there exists a prime $p$ such that the reduction of $f(x)$ modulo $p$ is irreducible in $\mathbb{F}_p[x]$, then $f(x)$ is irreducible in $\mathbb{Z}[x]$.

### Examples

**Example 1**: The polynomial $f(x) = x^3 + x + 1$ is irreducible over $\mathbb{Z}$ because its reduction modulo 2 is $x^3 + x + 1$ in $\mathbb{F}_2[x]$, which is irreducible.

**Example 2**: The polynomial $f(x) = x^4 + 1$ is irreducible over $\mathbb{Z}$ because its reduction modulo 3 is $x^4 + 1$ in $\mathbb{F}_3[x]$, which is irreducible.

## Factorization in Specific Rings

### Polynomial Rings over Fields

For any field $F$, the polynomial ring $F[x]$ is a Euclidean domain with the degree function as the Euclidean norm. Therefore, it is also a PID and a UFD.

**Key Properties**:
- Every non-zero polynomial has a unique factorization into irreducible polynomials
- The irreducible polynomials are exactly the prime elements
- The division algorithm holds: for any $f(x), g(x) \in F[x]$ with $g(x) \neq 0$, there exist $q(x), r(x) \in F[x]$ such that $f(x) = q(x)g(x) + r(x)$ with $\deg(r) < \deg(g)$

### Polynomial Rings over UFDs

When $R$ is a UFD, the polynomial ring $R[x]$ inherits the UFD property, but it is not necessarily a PID.

**Example**: $\mathbb{Z}[x]$ is a UFD but not a PID. The ideal $(2, x)$ is not principal.

## Applications

### Application 1: Algebraic Number Theory

Polynomial rings are fundamental in algebraic number theory. The ring of integers in a number field is often studied through its relationship to polynomial rings.

### Application 2: Algebraic Geometry

Polynomial rings in multiple variables are the coordinate rings of affine varieties. Understanding their factorization properties is crucial for understanding the geometry of these varieties.

### Application 3: Cryptography

Polynomial rings over finite fields are used in many cryptographic protocols, including elliptic curve cryptography and lattice-based cryptography.

## Advanced Topics

### Multivariate Polynomial Rings

For a UFD $R$, the polynomial ring $R[x_1, \ldots, x_n]$ in $n$ variables is also a UFD. This follows by induction from the single-variable case.

### Power Series Rings

The ring of formal power series $R[[x\|x]]$ over a ring $R$ has different properties than the polynomial ring $R[x]$. For example, if $R$ is a field, then $R[[x\|x]]$ is a local ring with a unique maximal ideal.

### Laurent Polynomial Rings

The ring of Laurent polynomials $R[x, x^{-1}]$ consists of finite sums of the form $\sum_{i=-n}^{m} a_i x^i$. These rings are important in many areas of mathematics, including representation theory and algebraic geometry.

## Examples and Counterexamples

### Example 1: Irreducible Polynomials in $\mathbb{Q}[x]$

- $x^2 + 1$ is irreducible over $\mathbb{Q}$
- $x^3 - 2$ is irreducible over $\mathbb{Q}$ (by Eisenstein's criterion with $p = 2$)
- $x^4 + 1$ is irreducible over $\mathbb{Q}$ (by reduction modulo 3)

### Example 2: Factorization in $\mathbb{Z}[x]$

The polynomial $f(x) = 2x^2 + 4x + 2$ factors as $2(x^2 + 2x + 1) = 2(x + 1)^2$ in $\mathbb{Z}[x]$. Note that the factor 2 is a unit in $\mathbb{Q}[x]$ but not in $\mathbb{Z}[x]$.

### Example 3: A Polynomial that is Irreducible over $\mathbb{Z}$ but Reducible over $\mathbb{Q}$

The polynomial $f(x) = 2x^2 + 2$ is irreducible over $\mathbb{Z}$ (as a polynomial with integer coefficients), but it factors as $2(x^2 + 1)$ over $\mathbb{Q}$.

## Summary

Polynomial rings provide a rich source of examples and applications in ring theory. The fact that UFDs are preserved when passing to polynomial rings (Gauss's Lemma) is one of the most important results in commutative algebra.

Eisenstein's criterion and other irreducibility tests provide practical tools for determining when polynomials are irreducible. These concepts are fundamental to many areas of mathematics, including algebraic number theory, algebraic geometry, and cryptography.

The study of polynomial rings continues to be an active area of research, with connections to many other areas of mathematics including representation theory, homological algebra, and computational algebra. 