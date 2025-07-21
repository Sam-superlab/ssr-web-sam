---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/14 - Field Extensions/Field Extensions/"}
---


# Field Extensions

## Introduction

The study of Galois theory begins with the concept of a field containing another field. Field extensions provide the foundation for understanding how fields can be built up from simpler fields, and they are essential for the study of polynomial equations and their solutions.

## Basic Definitions

### Field Extension

**Definition 14.1**: A **field extension** is a pair of fields $L/K$ (or $L:K$) such that $K$ is a subfield of $L$. We call $L$ an **extension field** of $K$.

Given an extension $L/K$, $L$ can be viewed as a vector space over the field $K$. The **degree** of the extension, denoted $[L:K]$, is the dimension of $L$ as a $K$-vector space. An extension is **finite** if its degree is finite; otherwise, it is **infinite**.

### Examples

- $\mathbb{C}/\mathbb{R}$ is a field extension of degree 2
- $\mathbb{R}/\mathbb{Q}$ is an infinite field extension
- $\mathbb{Q}(\sqrt{2})/\mathbb{Q}$ is a field extension of degree 2
- $\mathbb{F}_{p^n}/\mathbb{F}_p$ is a field extension of degree $n$

## Algebraic and Transcendental Elements

### Definition

**Definition 14.2**: Let $L/K$ be a field extension. An element $\alpha \in L$ is **algebraic over $K$** if it is a root of some non-zero polynomial with coefficients in $K$. If $\alpha$ is not algebraic, it is **transcendental over $K$**.

An extension $L/K$ is an **algebraic extension** if every element of $L$ is algebraic over $K$.

### Properties

- Every finite extension is algebraic
- The converse is not true; for example, the field of all algebraic numbers is an infinite algebraic extension of $\mathbb{Q}$

### Minimal Polynomial

If $\alpha$ is algebraic over $K$, there is a unique monic irreducible polynomial in $K[x]$ of which $\alpha$ is a root. This is called the **minimal polynomial** of $\alpha$ over $K$. If the degree of the minimal polynomial is $n$, then the smallest field containing both $K$ and $\alpha$, denoted $K(\alpha)$, has degree $[K(\alpha):K] = n$.

### Examples

**Example 1**: The element $\sqrt{2}$ is algebraic over $\mathbb{Q}$ with minimal polynomial $x^2 - 2$.

**Example 2**: The element $\pi$ is transcendental over $\mathbb{Q}$.

**Example 3**: The element $i$ is algebraic over $\mathbb{R}$ with minimal polynomial $x^2 + 1$.

## Simple Extensions

### Definition

A field extension $L/K$ is **simple** if there exists an element $\alpha \in L$ such that $L = K(\alpha)$. The element $\alpha$ is called a **primitive element** of the extension.

### Construction

If $\alpha$ is algebraic over $K$ with minimal polynomial $f(x)$, then:

$$K(\alpha) \cong K[x]/(f(x))$$

This isomorphism is given by sending $\alpha$ to the coset $x + (f(x))$.

### Examples

**Example 1**: $\mathbb{Q}(\sqrt{2}) = \{a + b\sqrt{2} \mid a, b \in \mathbb{Q}\}$

**Example 2**: $\mathbb{Q}(i) = \{a + bi \mid a, b \in \mathbb{Q}\}$

**Example 3**: $\mathbb{F}_2(\alpha)$ where $\alpha$ is a root of $x^2 + x + 1$ is the field with 4 elements.

## Degree of Extensions

### Multiplicativity of Degree

**Theorem 14.3 (Tower Law)**: Let $K \subseteq L \subseteq M$ be fields. Then:

$$[M:K] = [M:L][L:K]$$

This theorem is fundamental for understanding the structure of field extensions.

### Examples

**Example 1**: Consider the tower $\mathbb{Q} \subseteq \mathbb{Q}(\sqrt{2}) \subseteq \mathbb{Q}(\sqrt{2}, \sqrt{3})$. We have:
- $[\mathbb{Q}(\sqrt{2}):\mathbb{Q}] = 2$
- $[\mathbb{Q}(\sqrt{2}, \sqrt{3}):\mathbb{Q}(\sqrt{2})] = 2$ (since $\sqrt{3}$ is not in $\mathbb{Q}(\sqrt{2})$)
- $[\mathbb{Q}(\sqrt{2}, \sqrt{3}):\mathbb{Q}] = 4$

**Example 2**: Consider the tower $\mathbb{Q} \subseteq \mathbb{Q}(\sqrt[3]{2}) \subseteq \mathbb{Q}(\sqrt[3]{2}, \omega)$ where $\omega$ is a primitive cube root of unity. We have:
- $[\mathbb{Q}(\sqrt[3]{2}):\mathbb{Q}] = 3$
- $[\mathbb{Q}(\sqrt[3]{2}, \omega):\mathbb{Q}(\sqrt[3]{2})] = 2$
- $[\mathbb{Q}(\sqrt[3]{2}, \omega):\mathbb{Q}] = 6$

## Algebraic Closures

### Definition

**Definition 14.4**: A field $F$ is **algebraically closed** if every non-constant polynomial in $F[x]$ has a root in $F$. An **algebraic closure** of a field $K$, denoted $\overline{K}$ or $K^{\text{alg}}$, is an algebraic extension of $K$ that is algebraically closed.

### Properties

- Every field has an algebraic closure, and it is unique up to isomorphism
- The field of complex numbers $\mathbb{C}$ is the algebraic closure of $\mathbb{R}$
- The field of algebraic numbers is the algebraic closure of $\mathbb{Q}$

## Finite Fields

### Classification

**Theorem 14.5 (Classification of Finite Fields)**: 
- The order (number of elements) of a finite field is a power of a prime, $p^n$, where $p$ is the characteristic of the field
- For every prime power $p^n$, there exists a unique field of order $p^n$ (up to isomorphism), denoted $\text{GF}(p^n)$ or $\mathbb{F}_{p^n}$
- This field $\mathbb{F}_{p^n}$ can be constructed as the splitting field of the polynomial $x^{p^n} - x$ over the prime field $\mathbb{F}_p$

### Examples

- $\mathbb{F}_2 = \{0, 1\}$ with addition and multiplication modulo 2
- $\mathbb{F}_4 = \{0, 1, \alpha, \alpha + 1\}$ where $\alpha$ is a root of $x^2 + x + 1$
- $\mathbb{F}_9 = \{0, 1, 2, \alpha, \alpha + 1, \alpha + 2, 2\alpha, 2\alpha + 1, 2\alpha + 2\}$ where $\alpha$ is a root of $x^2 + 1$

## Applications

### Application 1: Constructibility

Field extensions are fundamental to the study of geometric constructibility. A number is constructible if and only if it lies in a field extension of $\mathbb{Q}$ of degree a power of 2.

### Application 2: Solvability by Radicals

Field extensions are essential for understanding when polynomial equations can be solved by radicals. This leads to Galois theory and the study of solvable groups.

### Application 3: Algebraic Number Theory

Field extensions are central to algebraic number theory, where one studies the arithmetic properties of algebraic numbers and their relationships.

## Advanced Topics

### Transcendence Degree

For infinite extensions, the concept of transcendence degree provides a measure of "size" analogous to degree for finite extensions.

### Separable Extensions

An algebraic extension $L/K$ is **separable** if the minimal polynomial of every element in $L$ has no repeated roots. Separability is crucial for Galois theory.

### Normal Extensions

An algebraic extension $L/K$ is **normal** if every irreducible polynomial in $K[x]$ that has at least one root in $L$ splits completely into linear factors in $L$. Normal extensions are the setting for Galois theory.

## Summary

Field extensions provide the foundation for understanding how fields can be built up from simpler fields. The degree of an extension measures its "size," and the tower law provides a powerful tool for understanding the structure of extensions.

Algebraic and transcendental elements play crucial roles, with algebraic elements being roots of polynomials and transcendental elements being "independent" of the base field. Simple extensions provide the building blocks for more complex extensions.

These concepts are fundamental to Galois theory and have applications throughout mathematics, from number theory to algebraic geometry to cryptography. 