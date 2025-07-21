---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part III - Galois Theory/21 - Algebraic Closures/Algebraic Closures/"}
---


# Algebraic Closures and Transcendence

## Introduction

While algebraic extensions are central to Galois theory, not all extensions are algebraic. The study of algebraic closures and transcendence provides important tools for understanding the structure of fields and their extensions.

## Algebraic Closures

### Definition

**Definition 21.1**: A field $F$ is **algebraically closed** if every non-constant polynomial in $F[x]$ has a root in $F$. An **algebraic closure** of a field $K$, denoted $\overline{K}$ or $K^{\text{alg}}$, is an algebraic extension of $K$ that is algebraically closed.

### Properties

- Every field has an algebraic closure, and it is unique up to isomorphism
- The field of complex numbers $\mathbb{C}$ is the algebraic closure of $\mathbb{R}$
- The field of algebraic numbers is the algebraic closure of $\mathbb{Q}$

### Construction

Using Zorn's Lemma, one can prove that every field has an algebraic closure. The construction involves taking the union of all algebraic extensions of the field.

### Examples

**Example 1**: $\mathbb{C}$ is the algebraic closure of $\mathbb{R}$.

**Example 2**: The field of algebraic numbers is the algebraic closure of $\mathbb{Q}$.

**Example 3**: For any finite field $\mathbb{F}_q$, its algebraic closure is the union of all finite fields $\mathbb{F}_{q^n}$ for $n \geq 1$.

## Transcendence

### Definition

**Definition 21.2**: A subset $S$ of an extension field $L/K$ is **algebraically independent over $K$** if its elements do not satisfy any non-trivial polynomial equation with coefficients in $K$. A **transcendence basis** for $L/K$ is a maximal algebraically independent subset of $L$ over $K$.

### Properties

- All transcendence bases for a given extension have the same cardinality, which is called the **transcendence degree** of the extension
- An extension $L/K$ can always be decomposed into a purely transcendental extension followed by an algebraic extension: $K \subseteq K(S) \subseteq L$, where $S$ is a transcendence basis

### Examples

**Example 1**: The set $\{\pi\}$ is algebraically independent over $\mathbb{Q}$, so the transcendence degree of $\mathbb{Q}(\pi)/\mathbb{Q}$ is 1.

**Example 2**: The set $\{e, \pi\}$ is algebraically independent over $\mathbb{Q}$, so the transcendence degree of $\mathbb{Q}(e, \pi)/\mathbb{Q}$ is 2.

**Example 3**: For the field of rational functions $K(x_1, \ldots, x_n)$, the set $\{x_1, \ldots, x_n\}$ is a transcendence basis over $K$.

## Applications

### Application 1: Field Theory

Algebraic closures provide a natural setting for studying field extensions and their properties.

### Application 2: Algebraic Geometry

Transcendence theory is important in algebraic geometry for understanding the structure of function fields and varieties.

### Application 3: Model Theory

The study of algebraically closed fields is fundamental to model theory and the study of first-order theories.

## Examples

### Example 1: Algebraic Numbers

The field of algebraic numbers is the algebraic closure of $\mathbb{Q}$. It contains all roots of polynomials with rational coefficients.

### Example 2: Function Fields

The field of rational functions $K(x_1, \ldots, x_n)$ has transcendence degree $n$ over $K$.

### Example 3: Transcendental Numbers

Numbers like $\pi$ and $e$ are transcendental over $\mathbb{Q}$, meaning they are not roots of any non-zero polynomial with rational coefficients.

## Advanced Topics

### Transcendence Degree

The transcendence degree provides a measure of "size" for infinite extensions, analogous to degree for finite extensions.

### Lüroth's Theorem

**Theorem 21.3 (Lüroth's Theorem)**: Let $K$ be a field and let $L$ be a field between $K$ and $K(x)$ for some transcendental element $x$. Then $L = K(f(x))$ for some rational function $f(x) \in K(x)$.

### The Ax-Grothendieck Theorem

**Theorem 21.4 (Ax-Grothendieck Theorem)**: Let $K$ be an algebraically closed field and let $f: K^n \to K^n$ be an injective polynomial map. Then $f$ is surjective.

## Summary

Algebraic closures provide a natural completion of fields with respect to polynomial equations, while transcendence theory provides tools for understanding the structure of infinite extensions.

These concepts are fundamental to field theory and have applications throughout mathematics, from algebraic geometry to model theory to number theory.

The study of algebraic closures and transcendence continues to be an active area of research with connections to many other areas of mathematics. 