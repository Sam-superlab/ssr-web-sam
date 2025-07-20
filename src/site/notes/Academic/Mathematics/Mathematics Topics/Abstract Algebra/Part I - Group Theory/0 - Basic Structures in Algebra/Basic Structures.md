---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/0 - Basic Structures in Algebra/Basic Structures/"}
---


# Basic Structures in Algebra

## Introduction

Before delving into the abstract framework of group theory, it is prudent to review the foundational algebraic structures that provide both the motivation and the primary examples for the concepts to follow. These structures—sets of numbers and vector spaces—are the building blocks upon which more abstract theories are built.

## Sets of Numbers and Operations

The most familiar algebraic structures are sets of numbers equipped with binary operations. These include:

- **The integers**, denoted by $\mathbb{Z}$, with the operations of addition $(+)$ and multiplication $(\cdot)$
- **The rational numbers**, denoted by $\mathbb{Q}$, which are quotients of integers
- **The real numbers**, denoted by $\mathbb{R}$
- **The complex numbers**, denoted by $\mathbb{C}$

Each of these sets, when paired with an operation like addition or multiplication, exhibits certain structural properties. For example, the integers under addition, $(\mathbb{Z}, +)$, form a structure where:

- Addition is **associative**: $(a + b) + c = a + (b + c)$
- There is an **identity element** $(0)$: $0 + a = a + 0 = a$
- Every element has an **inverse**: $a + (-a) = (-a) + a = 0$

These properties will be abstracted to define a group.

## Vector Spaces

A **vector space** over a field $F$ (such as $\mathbb{R}$) is a set $V$ of vectors, equipped with two operations:
- **Vector addition**: $V \times V \to V$
- **Scalar multiplication**: $F \times V \to V$

This structure is more complex than a simple set of numbers, as it involves two distinct sets (vectors and scalars) and their interactions.

### Key Properties of Vector Spaces

1. **Closure under addition**: If $\mathbf{u}, \mathbf{v} \in V$, then $\mathbf{u} + \mathbf{v} \in V$
2. **Associativity of addition**: $(\mathbf{u} + \mathbf{v}) + \mathbf{w} = \mathbf{u} + (\mathbf{v} + \mathbf{w})$
3. **Commutativity of addition**: $\mathbf{u} + \mathbf{v} = \mathbf{v} + \mathbf{u}$
4. **Identity element**: There exists $\mathbf{0} \in V$ such that $\mathbf{v} + \mathbf{0} = \mathbf{v}$
5. **Inverse elements**: For each $\mathbf{v} \in V$, there exists $-\mathbf{v} \in V$ such that $\mathbf{v} + (-\mathbf{v}) = \mathbf{0}$

The set of vectors in a vector space, together with the operation of vector addition, forms an **abelian group**. This demonstrates that groups are often found embedded within more elaborate algebraic structures.

## The Concept of an Algebraic Structure

In the most general sense, an **algebraic structure** is a non-empty set endowed with one or more binary operations that satisfy a given set of axioms.

### Key Characteristics

- **Abstraction**: By studying these structures in the abstract, we can prove theorems that apply to all systems satisfying the axioms
- **Universality**: Results apply regardless of the specific nature of their elements
- **Progressive Complexity**: This course will proceed by defining progressively richer structures:
  - **Groups**: A set with one operation
  - **Rings**: A set with two operations (addition and multiplication)
  - **Fields**: Rings where division is possible (except by zero)

## Historical Development

The historical development of group theory was driven by three main sources:

1. **Number Theory**: The study of integers and their properties
2. **Theory of Algebraic Equations**: The quest to find general solutions for polynomial equations
3. **Geometry**: The study of geometric transformations and symmetries

The quest to find general solutions for high-degree polynomial equations, pioneered by mathematicians like Lagrange and Abel, led Évariste Galois to establish a profound connection between group theory and field theory, now known as **Galois theory**.

This connection reveals that the solvability of a polynomial is determined by the structure of its associated group of symmetries, which is the ultimate destination of this course.

## Examples

### Example 1: Integers under Addition
$(\mathbb{Z}, +)$ forms a group because:
- **Closure**: $a + b \in \mathbb{Z}$ for all $a, b \in \mathbb{Z}$
- **Associativity**: $(a + b) + c = a + (b + c)$
- **Identity**: $0 + a = a + 0 = a$
- **Inverses**: $a + (-a) = (-a) + a = 0$

### Example 2: Real Numbers under Multiplication
$(\mathbb{R}^*, \cdot)$ where $\mathbb{R}^* = \mathbb{R} \setminus \{0\}$ forms a group because:
- **Closure**: $a \cdot b \in \mathbb{R}^*$ for all $a, b \in \mathbb{R}^*$
- **Associativity**: $(a \cdot b) \cdot c = a \cdot (b \cdot c)$
- **Identity**: $1 \cdot a = a \cdot 1 = a$
- **Inverses**: $a \cdot \frac{1}{a} = \frac{1}{a} \cdot a = 1$

### Example 3: Vector Space Example
Consider $\mathbb{R}^2$ as a vector space over $\mathbb{R}$:
- Vectors: $(x, y)$ where $x, y \in \mathbb{R}$
- Addition: $(x_1, y_1) + (x_2, y_2) = (x_1 + x_2, y_1 + y_2)$
- Scalar multiplication: $c \cdot (x, y) = (cx, cy)$

The set $(\mathbb{R}^2, +)$ forms an abelian group under vector addition.

## Summary

These basic structures provide the foundation for understanding more abstract algebraic concepts. The properties we observe in familiar number systems and vector spaces will be formalized and generalized in the study of groups, rings, and fields. 