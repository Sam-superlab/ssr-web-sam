---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/11 - Unique Factorization Domains/Eisenstein's Criterion/"}
---


# Eisenstein's Criterion

## Introduction

Eisenstein's Criterion is a practical tool for determining if a polynomial is irreducible over a field. It is particularly useful for polynomials with integer coefficients and provides a simple test for irreducibility.

## Statement

**Theorem 11.3 (Eisenstein's Criterion)**: Let $R$ be a UFD with field of fractions $F$. Let $f(x) = a_n x^n + \cdots + a_1 x + a_0$ be a polynomial in $R[x]$. If there exists a prime element $p \in R$ such that:

1. $p$ divides $a_i$ for all $i \in \{0, 1, \ldots, n-1\}$
2. $p$ does not divide $a_n$
3. $p^2$ does not divide $a_0$

then $f(x)$ is irreducible over the field of fractions $F$.

## Proof Sketch

The proof uses contradiction:
1. Assume $f(x)$ is reducible: $f(x) = g(x)h(x)$ where $\deg(g), \deg(h) < n$
2. Consider the polynomial modulo $p$: $\overline{f}(x) = \overline{a_n}x^n$ in $(R/pR)[x]$
3. Since $f(x) = g(x)h(x)$, we have $\overline{f}(x) = \overline{g}(x)\overline{h}(x)$
4. This implies that $\overline{g}(x) = bx^k$ and $\overline{h}(x) = cx^m$ for some constants $b, c$
5. This means that $p$ divides all coefficients of $g(x)$ and $h(x)$ except possibly the leading coefficients
6. But then $p^2$ would divide the constant term of $f(x)$, contradicting condition 3

## Examples

### Example 1: Cyclotomic Polynomials

For any prime $p$, the $p$-th cyclotomic polynomial $\Phi_p(x) = \frac{x^p - 1}{x - 1} = x^{p-1} + \cdots + x + 1$ is irreducible over $\mathbb{Q}$.

While the criterion does not apply to $\Phi_p(x)$ directly, it applies to $\Phi_p(x+1)$, which is sufficient to prove the irreducibility of the original polynomial.

### Example 2: Polynomials of the Form $x^n - p$

The polynomial $x^n - p$ is irreducible over $\mathbb{Q}$ for any prime $p$ and any positive integer $n$. This follows directly from Eisenstein's Criterion with the prime $p$.

### Example 3: Polynomials with Prime Constant Term

The polynomial $x^3 + 2x^2 + 4x + 2$ is irreducible over $\mathbb{Q}$ by Eisenstein's Criterion with $p = 2$.

## Applications

### Application 1: Constructing Irreducible Polynomials

Eisenstein's Criterion provides a simple way to construct irreducible polynomials over $\mathbb{Q}$.

### Application 2: Field Extensions

Irreducible polynomials are crucial for constructing field extensions, and Eisenstein's Criterion helps identify them.

### Application 3: Algebraic Number Theory

The criterion is useful in algebraic number theory for studying minimal polynomials of algebraic numbers.

### Application 4: Galois Theory

Irreducible polynomials are fundamental to Galois theory, and Eisenstein's Criterion helps identify them.

## Limitations

### Not Always Applicable

Eisenstein's Criterion is not always applicable. Many irreducible polynomials do not satisfy the conditions of the criterion.

### Requires UFD

The criterion requires the coefficient ring to be a UFD, which limits its applicability.

### Field of Fractions

The criterion only guarantees irreducibility over the field of fractions, not necessarily over the original ring.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/11 - Unique Factorization Domains/Unique Factorization Domains\|Unique Factorization Domains]]
- [[Irreducible Polynomials\|Irreducible Polynomials]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/12 - Polynomial Rings/Polynomial Rings\|Polynomial Rings]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/14 - Field Extensions/Field Extensions\|Field Extensions]]
- [[Cyclotomic Polynomials\|Cyclotomic Polynomials]] 