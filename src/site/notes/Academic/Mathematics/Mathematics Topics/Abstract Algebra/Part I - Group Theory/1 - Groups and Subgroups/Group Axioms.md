---
dg-publish: true
---

# Group Axioms

## Introduction

A **group** is an ordered pair $(G, \cdot)$, where $G$ is a non-empty set and $\cdot$ is a binary operation on $G$, satisfying the following four axioms.

## The Four Group Axioms

### 1. Closure
For all $a, b \in G$, the result of the operation, $a \cdot b$, is also in $G$.

### 2. Associativity
For all $a, b, c \in G$, the equation $(a \cdot b) \cdot c = a \cdot (b \cdot c)$ holds.

### 3. Identity Element
There exists a unique element $e \in G$, called the **identity element**, such that for every element $a \in G$, the equation $e \cdot a = a \cdot e = a$ holds.

### 4. Inverse Element
For each element $a \in G$, there exists an element $b \in G$, denoted $a^{-1}$, called the **inverse of $a$**, such that $a \cdot a^{-1} = a^{-1} \cdot a = e$.

## Additional Properties

### Commutativity
If the group operation is also **commutative** (i.e., $a \cdot b = b \cdot a$ for all $a, b \in G$), the group is called an **abelian group** or a **commutative group**.

### Order
- The number of elements in a group is called its **order**, denoted $|G|$
- If the order is finite, the group is a **finite group**
- If the order is infinite, the group is an **infinite group**

## Motivation: Symmetry

The group axioms are not an arbitrary collection of rules; rather, they are a precise formalization of the essential properties common to all systems of symmetry transformations.

Consider the set of symmetries of a geometric object:
- The composition of two symmetries is another symmetry (**Closure**)
- The composition of functions is inherently associative (**Associativity**)
- The transformation that does nothing is a symmetry (**Identity**)
- Any symmetry can be undone by reversing the transformation (**Inverse**)

Thus, the set of symmetries of any object forms a group, known as its **symmetry group**. This insight frames group theory as the abstract study of symmetry itself.

## Examples

### Example 1: The Integers under Addition
$(\mathbb{Z}, +)$ is a group:
- **Closure**: The sum of two integers is an integer
- **Associativity**: $(a + b) + c = a + (b + c)$ for all $a, b, c \in \mathbb{Z}$
- **Identity**: $0$ is the identity element
- **Inverses**: The inverse of $a$ is $-a$
- **Abelian**: Addition is commutative

### Example 2: The Non-zero Rationals under Multiplication
$(\mathbb{Q}^*, \cdot)$ is a group:
- **Closure**: The product of two non-zero rationals is non-zero rational
- **Associativity**: $(a \cdot b) \cdot c = a \cdot (b \cdot c)$ for all $a, b, c \in \mathbb{Q}^*$
- **Identity**: $1$ is the identity element
- **Inverses**: The inverse of $a$ is $\frac{1}{a}$
- **Abelian**: Multiplication is commutative

### Example 3: The Symmetric Group $S_3$
The group of permutations of three elements:
- **Closure**: Composition of permutations is a permutation
- **Associativity**: Function composition is associative
- **Identity**: The identity permutation
- **Inverses**: Every permutation has an inverse
- **Non-abelian**: Permutation composition is not commutative

## Basic Properties

### Uniqueness of Identity
The identity element in a group is unique.

### Uniqueness of Inverses
For each element $a \in G$, the inverse $a^{-1}$ is unique.

### Cancellation Laws
In a group, if $ab = ac$, then $b = c$ (left cancellation), and if $ba = ca$, then $b = c$ (right cancellation).

### Inverse of a Product
For any elements $a, b \in G$, we have $(ab)^{-1} = b^{-1}a^{-1}$.

## Related Concepts

- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Subgroups\|Subgroups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Group Homomorphisms\|Group Homomorphisms]]
- [[Cyclic Groups\|Cyclic Groups]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Symmetric Groups\|Symmetric Groups]] 