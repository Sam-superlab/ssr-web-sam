---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/15 - Normal Extensions/Normal Extensions/"}
---


# Normal Extensions and Splitting Fields

## Introduction

Galois theory focuses on extensions that are "well-behaved" with respect to the roots of polynomials. These are the normal extensions, which are equivalent to splitting fields for finite extensions.

## Splitting Fields

### Definition

**Definition 15.1**: Let $p(x)$ be a polynomial in $K[x]$. A field extension $L$ of $K$ is a **splitting field** for $p(x)$ over $K$ if:

1. $p(x)$ factors into linear factors (or "splits") in $L[x]$
2. $L$ is the smallest such field, meaning $L$ is generated over $K$ by the roots of $p(x)$

### Properties

- Splitting fields always exist and are unique up to isomorphism
- The degree of a splitting field is finite
- A splitting field is always a normal extension

### Examples

**Example 1**: The splitting field of $x^2 - 2$ over $\mathbb{Q}$ is $\mathbb{Q}(\sqrt{2})$.

**Example 2**: The splitting field of $x^3 - 2$ over $\mathbb{Q}$ is $\mathbb{Q}(\sqrt[3]{2}, \omega)$ where $\omega$ is a primitive cube root of unity.

**Example 3**: The splitting field of $x^4 + 1$ over $\mathbb{Q}$ is $\mathbb{Q}(\sqrt{2}, i)$.

## Normal Extensions

### Definition

**Definition 15.2**: An algebraic extension $L/K$ is a **normal extension** if every irreducible polynomial in $K[x]$ that has at least one root in $L$ splits completely into linear factors in $L$.

### Equivalence for Finite Extensions

For finite extensions, the concepts of a normal extension and a splitting field are equivalent.

**Theorem 15.3**: A finite extension $L/K$ is normal if and only if $L$ is the splitting field of some polynomial over $K$.

### Examples

**Example 1**: $\mathbb{Q}(\sqrt{2})$ is a normal extension of $\mathbb{Q}$ because it is the splitting field of $x^2 - 2$.

**Example 2**: $\mathbb{Q}(\sqrt[3]{2})$ is not normal over $\mathbb{Q}$ because the minimal polynomial $x^3 - 2$ has one real root, $\sqrt[3]{2}$, but its two complex roots are not in the field.

**Example 3**: The smallest normal extension containing $\mathbb{Q}(\sqrt[3]{2})$ is its normal closure, which is the splitting field of $x^3 - 2$, namely $\mathbb{Q}(\sqrt[3]{2}, \omega)$.

## Normal Closure

### Definition

**Definition 15.4**: Let $L/K$ be an algebraic extension. The **normal closure** of $L$ over $K$ is the smallest normal extension of $K$ containing $L$.

### Construction

The normal closure can be constructed by adjoining all the roots of the minimal polynomials of the elements of $L$ over $K$.

### Examples

**Example 1**: The normal closure of $\mathbb{Q}(\sqrt[3]{2})$ over $\mathbb{Q}$ is $\mathbb{Q}(\sqrt[3]{2}, \omega)$.

**Example 2**: The normal closure of $\mathbb{Q}(\sqrt[4]{2})$ over $\mathbb{Q}$ is $\mathbb{Q}(\sqrt[4]{2}, i)$.

## Properties of Normal Extensions

### Fixed Field Property

**Theorem 15.5**: Let $L/K$ be a normal extension and let $\sigma: L \to L$ be a $K$-automorphism. Then $\sigma$ maps $L$ to itself.

### Conjugate Roots

In a normal extension, if $\alpha$ is a root of an irreducible polynomial $f(x) \in K[x]$, then all other roots of $f(x)$ (the conjugates of $\alpha$) are also in the extension.

### Examples

**Example 1**: In $\mathbb{Q}(\sqrt{2})$, the conjugates of $\sqrt{2}$ are $\sqrt{2}$ and $-\sqrt{2}$, both of which are in the field.

**Example 2**: In $\mathbb{Q}(\sqrt[3]{2}, \omega)$, the conjugates of $\sqrt[3]{2}$ are $\sqrt[3]{2}$, $\omega\sqrt[3]{2}$, and $\omega^2\sqrt[3]{2}$, all of which are in the field.

## Applications

### Application 1: Galois Theory

Normal extensions are the setting for Galois theory. The fundamental theorem of Galois theory establishes a correspondence between intermediate fields of a normal extension and subgroups of the Galois group.

### Application 2: Solvability by Radicals

Normal extensions are essential for understanding when polynomial equations can be solved by radicals. The Galois group of a normal extension provides information about the solvability of the corresponding polynomial.

### Application 3: Algebraic Number Theory

Normal extensions are important in algebraic number theory, where one studies the arithmetic properties of algebraic numbers and their relationships.

## Examples

### Example 1: Quadratic Extensions

All quadratic extensions of $\mathbb{Q}$ are normal. For example, $\mathbb{Q}(\sqrt{d})$ is the splitting field of $x^2 - d$ over $\mathbb{Q}$.

### Example 2: Cyclotomic Extensions

The cyclotomic extension $\mathbb{Q}(\zeta_n)$, where $\zeta_n$ is a primitive $n$-th root of unity, is normal over $\mathbb{Q}$. It is the splitting field of the cyclotomic polynomial $\Phi_n(x)$.

### Example 3: Cubic Extensions

Not all cubic extensions are normal. For example, $\mathbb{Q}(\sqrt[3]{2})$ is not normal, but $\mathbb{Q}(\sqrt[3]{2}, \omega)$ is normal.

## Advanced Topics

### Infinite Normal Extensions

The concept of normality can be extended to infinite extensions, but this requires more sophisticated tools from field theory.

### Separable Normal Extensions

A **Galois extension** is a field extension that is both normal and separable. These are the extensions for which the fundamental theorem of Galois theory holds.

### Normal Basis Theorem

**Theorem 15.6 (Normal Basis Theorem)**: Let $L/K$ be a finite Galois extension with Galois group $G$. Then there exists an element $\alpha \in L$ such that $\{\sigma(\alpha) \mid \sigma \in G\}$ is a basis for $L$ as a $K$-vector space.

## Summary

Normal extensions are the "well-behaved" extensions that are essential for Galois theory. They are characterized by the property that every irreducible polynomial with a root in the extension splits completely in the extension.

Splitting fields provide a concrete way to construct normal extensions, and for finite extensions, the concepts are equivalent. Normal closures allow us to "complete" non-normal extensions to normal ones.

These concepts are fundamental to understanding the structure of field extensions and have profound applications in Galois theory, algebraic number theory, and the study of polynomial equations. 