---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/11 - Unique Factorization Domains/Gauss's Lemma/"}
---


# Gauss's Lemma

## Introduction

Gauss's Lemma is a cornerstone result in ring theory that establishes the relationship between factorization in a ring and factorization in its polynomial ring. It is fundamental to understanding unique factorization in polynomial rings.

## Statement

**Theorem 11.2 (Gauss's Lemma and its Corollary)**: If $R$ is a UFD, then the polynomial ring $R[x]$ is also a UFD.

## Key Concepts

### Content of a Polynomial

The **content** of a polynomial $f(x) = a_n x^n + \cdots + a_1 x + a_0$ in $R[x]$ is the greatest common divisor of its coefficients: $\text{cont}(f) = \gcd(a_n, \ldots, a_0)$.

### Primitive Polynomial

A polynomial $f(x) \in R[x]$ is **primitive** if its content is a unit in $R$, i.e., $\text{cont}(f) = 1$.

## Gauss's Lemma

**Gauss's Lemma**: The product of two primitive polynomials is primitive.

### Proof Sketch

The proof involves:
1. Assuming that the product of two primitive polynomials is not primitive
2. Using the fact that $R$ is a UFD to find a prime element that divides all coefficients of the product
3. Deriving a contradiction by showing that this prime must divide all coefficients of one of the original polynomials

## Corollary: UFD Property

Using Gauss's Lemma, one can prove that if $R$ is a UFD, then $R[x]$ is also a UFD.

### Proof Strategy

1. **Define the content**: For any polynomial $f(x) \in R[x]$, write $f(x) = \text{cont}(f) \cdot f_1(x)$ where $f_1(x)$ is primitive.

2. **Relate to field of fractions**: Consider factorization in $F[x]$, where $F$ is the field of fractions of $R$.

3. **Lift factorization**: Use Gauss's Lemma to lift the unique factorization from $F[x]$ back to $R[x]$.

## Consequences

This theorem is immensely powerful as it provides a vast supply of UFDs. For example:
- Since $\mathbb{Z}$ is a UFD, so is $\mathbb{Z}[x]$
- By induction, the polynomial ring in any number of variables over a UFD, such as $\mathbb{Z}[x_1, \ldots, x_n]$ or $F[x_1, \ldots, x_n]$ for a field $F$, is also a UFD

## Examples

### Example 1: Polynomial Rings over Fields

For any field $F$, the polynomial ring $F[x]$ is a UFD. This follows from the fact that $F$ is a UFD and applying Gauss's Lemma.

### Example 2: Multivariable Polynomial Rings

The polynomial ring $\mathbb{Z}[x, y]$ is a UFD, even though it is not a PID. The ideal $(x, y)$ is not principal.

### Example 3: Polynomial Rings over UFDs

If $R$ is any UFD, then $R[x_1, \ldots, x_n]$ is also a UFD for any number of variables.

## Applications

### Application 1: Polynomial Factorization

Gauss's Lemma is fundamental to understanding polynomial factorization over different rings.

### Application 2: Algebraic Number Theory

The result is crucial in algebraic number theory for understanding factorization in rings of integers.

### Application 3: Algebraic Geometry

Polynomial rings over UFDs are important in algebraic geometry for studying coordinate rings of varieties.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/11 - Unique Factorization Domains/Unique Factorization Domains\|Unique Factorization Domains]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/12 - Polynomial Rings/Polynomial Rings\|Polynomial Rings]]
- [[Content of Polynomials\|Content of Polynomials]]
- [[Primitive Polynomials\|Primitive Polynomials]]
- [[Field of Fractions\|Field of Fractions]] 