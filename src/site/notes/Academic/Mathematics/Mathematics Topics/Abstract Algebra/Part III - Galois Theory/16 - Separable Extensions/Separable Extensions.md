---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/16 - Separable Extensions/Separable Extensions/"}
---


# Separable Extensions and Finite Fields

## Introduction

A second crucial condition for the main theorem of Galois theory is separability, which ensures that polynomials have distinct roots. This property is essential for the development of Galois theory and has important implications for the structure of field extensions.

## Separable Polynomials and Extensions

### Definition

**Definition 16.1**: An irreducible polynomial $p(x) \in K[x]$ is **separable** if it has no repeated roots in its splitting field. An algebraic extension $L/K$ is a **separable extension** if the minimal polynomial of every element in $L$ is separable.

### Properties

- In a field of characteristic 0 (like $\mathbb{Q}$, $\mathbb{R}$, $\mathbb{C}$), every irreducible polynomial is separable
- Inseparability can only occur in fields of prime characteristic $p > 0$
- Fields where every algebraic extension is separable are called **perfect fields**
- All fields of characteristic 0 and all finite fields are perfect

### Examples

**Example 1**: The polynomial $x^2 - 2$ is separable over $\mathbb{Q}$ because it has distinct roots $\sqrt{2}$ and $-\sqrt{2}$.

**Example 2**: The polynomial $x^2 + 1$ is separable over $\mathbb{R}$ because it has distinct roots $i$ and $-i$.

**Example 3**: In characteristic $p$, the polynomial $x^p - a$ is inseparable if $a$ is not a $p$-th power.

## Galois Extensions

### Definition

A **Galois extension** is a field extension that is both normal and separable.

### Properties

- For finite extensions, being Galois is equivalent to being the splitting field of a separable polynomial
- Galois extensions are the setting for the fundamental theorem of Galois theory
- The order of the Galois group equals the degree of the extension

### Examples

**Example 1**: $\mathbb{Q}(\sqrt{2})/\mathbb{Q}$ is a Galois extension because it is the splitting field of the separable polynomial $x^2 - 2$.

**Example 2**: $\mathbb{Q}(\sqrt[3]{2}, \omega)/\mathbb{Q}$ is a Galois extension because it is the splitting field of the separable polynomial $x^3 - 2$.

## Finite Fields

### Classification

**Theorem 16.2 (Classification of Finite Fields)**: 
- The order (number of elements) of a finite field is a power of a prime, $p^n$, where $p$ is the characteristic of the field
- For every prime power $p^n$, there exists a unique field of order $p^n$ (up to isomorphism), denoted $\text{GF}(p^n)$ or $\mathbb{F}_{p^n}$
- This field $\mathbb{F}_{p^n}$ can be constructed as the splitting field of the polynomial $x^{p^n} - x$ over the prime field $\mathbb{F}_p$

### Properties

- Every finite field is perfect
- The multiplicative group of a finite field is cyclic
- Every finite field has a primitive element (an element whose powers generate the multiplicative group)

### Examples

**Example 1**: $\mathbb{F}_2 = \{0, 1\}$ with addition and multiplication modulo 2.

**Example 2**: $\mathbb{F}_4 = \{0, 1, \alpha, \alpha + 1\}$ where $\alpha$ is a root of $x^2 + x + 1$.

**Example 3**: $\mathbb{F}_9 = \{0, 1, 2, \alpha, \alpha + 1, \alpha + 2, 2\alpha, 2\alpha + 1, 2\alpha + 2\}$ where $\alpha$ is a root of $x^2 + 1$.

## Inseparable Extensions

### Definition

An algebraic extension $L/K$ is **inseparable** if there exists an element in $L$ whose minimal polynomial over $K$ is inseparable.

### Properties

- Inseparability can only occur in fields of positive characteristic
- Inseparable extensions have different properties than separable extensions
- The theory of inseparable extensions is more complex and less well-behaved

### Examples

**Example 1**: Let $K = \mathbb{F}_p(t)$ be the field of rational functions over $\mathbb{F}_p$. The extension $K(\sqrt[p]{t})/K$ is inseparable because the minimal polynomial of $\sqrt[p]{t}$ is $x^p - t = (x - \sqrt[p]{t})^p$.

## Applications

### Application 1: Galois Theory

Separable extensions are essential for Galois theory. The fundamental theorem of Galois theory only holds for Galois extensions, which must be separable.

### Application 2: Algebraic Number Theory

Separable extensions are important in algebraic number theory, where one studies the arithmetic properties of algebraic numbers and their relationships.

### Application 3: Cryptography

Finite fields are fundamental to many cryptographic protocols, including elliptic curve cryptography and the Advanced Encryption Standard (AES).

## Examples

### Example 1: Separable Extensions

- $\mathbb{Q}(\sqrt{2})/\mathbb{Q}$ is separable
- $\mathbb{Q}(\sqrt[3]{2}, \omega)/\mathbb{Q}$ is separable
- $\mathbb{F}_{p^n}/\mathbb{F}_p$ is separable for any $n$

### Example 2: Inseparable Extensions

- $\mathbb{F}_p(t)(\sqrt[p]{t})/\mathbb{F}_p(t)$ is inseparable
- Any purely inseparable extension in characteristic $p$

### Example 3: Galois Extensions

- $\mathbb{Q}(\sqrt{2})/\mathbb{Q}$ is Galois
- $\mathbb{Q}(\sqrt[3]{2}, \omega)/\mathbb{Q}$ is Galois
- $\mathbb{F}_{p^n}/\mathbb{F}_p$ is Galois

## Advanced Topics

### Purely Inseparable Extensions

An extension $L/K$ is **purely inseparable** if every element in $L$ is purely inseparable over $K$ (i.e., its minimal polynomial has only one root).

### Separable Degree

The **separable degree** of an extension $L/K$ is the number of distinct $K$-embeddings of $L$ into an algebraic closure of $K$.

### Inseparable Degree

The **inseparable degree** of an extension $L/K$ is the degree divided by the separable degree.

## Summary

Separable extensions are the "well-behaved" extensions that are essential for Galois theory. They ensure that polynomials have distinct roots, which is crucial for the development of the theory.

Finite fields provide important examples of perfect fields and have applications throughout mathematics, particularly in cryptography and coding theory.

The distinction between separable and inseparable extensions is fundamental to understanding the structure of field extensions and has profound implications for Galois theory and algebraic number theory. 