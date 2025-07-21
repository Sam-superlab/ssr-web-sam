---
dg-publish: true
---

# Rings

## Introduction

A ring is an algebraic structure that generalizes the arithmetic of the integers. It is a set where one can add, subtract, and multiply, subject to a set of familiar rules.

## Definition

A **ring** is a set $R$ equipped with two binary operations, typically called addition $(+)$ and multiplication $(\cdot)$, satisfying the following axioms:

### Axioms for Addition

$(R, +)$ is an abelian group:
- **Associativity of addition**: $(a + b) + c = a + (b + c)$
- **Commutativity of addition**: $a + b = b + a$
- **Additive identity**: There exists an element $0 \in R$ such that $a + 0 = a$
- **Additive inverse**: For each $a \in R$, there exists $-a \in R$ such that $a + (-a) = 0$

### Axioms for Multiplication

$(R, \cdot)$ is a monoid:
- **Associativity of multiplication**: $(a \cdot b) \cdot c = a \cdot (b \cdot c)$
- **Multiplicative identity**: There exists an element $1 \in R$ such that $a \cdot 1 = 1 \cdot a = a$

### Distributivity

Multiplication is distributive over addition:
- **Left distributivity**: $a \cdot (b + c) = (a \cdot b) + (a \cdot c)$
- **Right distributivity**: $(b + c) \cdot a = (b \cdot a) + (c \cdot a)$

### Commutative Rings

A ring is **commutative** if its multiplication is commutative. Throughout this part, unless otherwise specified, rings are assumed to be commutative.

## Examples

### Example 1: The Integers
$(\mathbb{Z}, +, \cdot)$ is a commutative ring with identity.

### Example 2: Polynomial Rings
For any ring $R$, the set $R[x]$ of polynomials with coefficients in $R$ forms a ring under polynomial addition and multiplication.

### Example 3: Matrix Rings
The set $M_n(R)$ of $n \times n$ matrices with entries in a ring $R$ forms a ring under matrix addition and multiplication (non-commutative for $n > 1$).

### Example 4: Function Rings
The set of all functions from a set $X$ to a ring $R$ forms a ring under pointwise addition and multiplication.

### Example 5: Modular Arithmetic
The set $\mathbb{Z}/n\mathbb{Z}$ of integers modulo $n$ forms a ring under modular addition and multiplication.

## Special Types of Rings

### Integral Domains

A ring $R$ is an **integral domain** if it is commutative, has an identity, and has no zero divisors (i.e., if $ab = 0$, then either $a = 0$ or $b = 0$).

**Examples**:
- $\mathbb{Z}$ is an integral domain
- $\mathbb{Z}[x]$ is an integral domain
- $\mathbb{Z}/6\mathbb{Z}$ is not an integral domain (since $2 \cdot 3 = 0$)

### Fields

A **field** is a commutative ring with identity where every non-zero element has a multiplicative inverse.

**Examples**:
- $\mathbb{Q}$, $\mathbb{R}$, $\mathbb{C}$ are fields
- $\mathbb{Z}/p\mathbb{Z}$ is a field when $p$ is prime
- $\mathbb{Z}$ is not a field

### Division Rings

A **division ring** (or **skew field**) is a ring where every non-zero element has a multiplicative inverse, but multiplication need not be commutative.

**Examples**:
- The quaternions $\mathbb{H}$ form a division ring
- All fields are division rings

## Properties

### Zero Divisors

A **zero divisor** in a ring $R$ is a non-zero element $a$ such that there exists a non-zero element $b$ with $ab = 0$ or $ba = 0$.

### Units

A **unit** in a ring $R$ is an element $a$ that has a multiplicative inverse, i.e., there exists $b \in R$ such that $ab = ba = 1$.

### Characteristic

The **characteristic** of a ring $R$ is the smallest positive integer $n$ such that $n \cdot 1 = 0$, or $0$ if no such integer exists.

## Applications

### Application 1: Number Theory

Rings provide the algebraic foundation for number theory, particularly through the study of integers and modular arithmetic.

### Application 2: Algebraic Geometry

Rings correspond to geometric objects, establishing a deep connection between algebra and geometry.

### Application 3: Linear Algebra

Matrix rings are fundamental to linear algebra and the study of linear transformations.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/9 - Rings and Ideals/Ideals\|Ideals]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/9 - Rings and Ideals/Ring Homomorphisms\|Ring Homomorphisms]]
- [[Integral Domains\|Integral Domains]]
- [[Fields\|Fields]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part II - Ring and Field Theory/9 - Rings and Ideals/Quotient Rings\|Quotient Rings]] 