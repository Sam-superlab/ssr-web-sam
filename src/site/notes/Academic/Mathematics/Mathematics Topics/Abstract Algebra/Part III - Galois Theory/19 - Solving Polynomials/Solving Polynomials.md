---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/19 - Solving Polynomials/Solving Polynomials/"}
---


# Solving Polynomials and the Insolvability of the Quintic

## Introduction

We now apply the full power of Galois theory to its original motivation: determining which polynomial equations can be solved using a formula involving only arithmetic operations and roots.

## Solvability by Radicals

### Definition

**Definition 19.1**: A polynomial $f(x) \in K[x]$ is **solvable by radicals** if its roots can be expressed using elements of $K$ and a finite sequence of operations of addition, subtraction, multiplication, division, and taking $n$-th roots.

### Examples

**Example 1**: The quadratic equation $ax^2 + bx + c = 0$ is solvable by radicals:
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

**Example 2**: The cubic equation $x^3 + px + q = 0$ is solvable by radicals (Cardano's formula):
$$x = \sqrt[3]{\frac{-q}{2} + \sqrt{\frac{q^2}{4} + \frac{p^3}{27}}} + \sqrt[3]{\frac{-q}{2} - \sqrt{\frac{q^2}{4} + \frac{p^3}{27}}}$$

**Example 3**: The quartic equation is also solvable by radicals, though the formula is more complex.

## Galois's Criterion

The connection between this concept and group theory is the central result.

**Theorem 19.2 (Galois's Criterion)**: A polynomial $f(x) \in K[x]$ (where $K$ has characteristic 0) is solvable by radicals if and only if its Galois group, $\text{Gal}(L/K)$ (where $L$ is the splitting field of $f(x)$), is a solvable group.

### Proof Sketch

The proof involves showing that a field extension can be built by successively adjoining radicals if and only if its Galois group has a composition series with abelian (in fact, cyclic) factors, which is the definition of a solvable group.

## The Insolvability of the Quintic

This leads to the celebrated historical result.

**Theorem 19.3 (Insolvability of the Quintic)**: There is no general formula in terms of radicals for the roots of a polynomial of degree five or higher with arbitrary coefficients.

### Proof Sketch

1. **Consider the "general" polynomial** of degree $n$, whose coefficients are indeterminates over a field. The Galois group of this general polynomial is the full symmetric group, $S_n$.

2. **For $n \geq 5$**, the symmetric group $S_n$ is not a solvable group because its composition series contains the non-abelian simple group $A_n$.

3. **By Galois's Criterion**, since the Galois group $S_n$ (for $n \geq 5$) is not solvable, the general polynomial of degree $n$ is not solvable by radicals.

### Important Note

This does not mean that no quintic equation can be solved. For example, $x^5 - 2 = 0$ is solvable by radicals. It means there is no single formula, analogous to the quadratic formula, that will work for all quintic equations.

## Examples

### Example 1: Solvable Quintic

The polynomial $f(x) = x^5 - 2$ is solvable by radicals. Its splitting field is $\mathbb{Q}(\sqrt[5]{2}, \omega)$ where $\omega$ is a primitive 5th root of unity. The Galois group is isomorphic to the semidirect product $\mathbb{Z}_5 \rtimes \mathbb{Z}_4$, which is solvable.

### Example 2: Insolvable Quintic

The polynomial $f(x) = x^5 - x - 1$ is not solvable by radicals. Its Galois group is $S_5$, which is not solvable.

### Example 3: Cyclotomic Polynomials

The cyclotomic polynomial $\Phi_p(x) = \frac{x^p - 1}{x - 1}$ is solvable by radicals for any prime $p$, as its Galois group is abelian.

## Applications

### Application 1: Understanding Solvability

Galois theory provides the precise tool to determine, for any specific polynomial, whether it is solvable by radicals by computing its Galois group and checking for solvability.

### Application 2: Constructibility

The insolvability of the quintic is related to geometric constructibility problems. For example, the regular pentagon is constructible (because the 5th cyclotomic polynomial is solvable), but the regular heptagon is not.

### Application 3: Number Theory

The solvability of polynomials by radicals has implications for the arithmetic of number fields and the study of Diophantine equations.

## Advanced Topics

### Radical Extensions

A **radical extension** is a field extension that can be built by successively adjoining roots. The structure of radical extensions is closely related to the structure of solvable groups.

### Solvable Groups

A group $G$ is **solvable** if it has a composition series with abelian factors. This is equivalent to the derived series terminating in the trivial group.

### Examples of Solvable Groups

- All abelian groups are solvable
- All finite $p$-groups are solvable
- The symmetric group $S_n$ is solvable for $n \leq 4$ but not for $n \geq 5$

## Historical Context

### The Problem

The problem of finding formulas for the roots of polynomial equations dates back to ancient times. The quadratic formula was known to the Babylonians, and formulas for cubic and quartic equations were discovered in the 16th century.

### Galois's Contribution

Évariste Galois (1811-1832) revolutionized the study of polynomial equations by introducing the concept of a Galois group and showing that the solvability of a polynomial is determined by the structure of its Galois group.

### Abel's Work

Niels Henrik Abel (1802-1829) independently proved the insolvability of the general quintic equation, though his methods were different from Galois's.

## Summary

Galois theory provides a complete answer to the question of which polynomial equations can be solved by radicals. The key insight is that solvability by radicals corresponds to the Galois group being solvable.

The insolvability of the general quintic equation is one of the most famous results in mathematics, demonstrating the power of abstract algebra to solve concrete problems.

This theory has applications throughout mathematics, from number theory to algebraic geometry to cryptography, and continues to be an active area of research. 