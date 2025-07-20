---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/1 - Groups and Subgroups/Groups and Subgroups/"}
---


# Groups and Subgroups

## Introduction

The concept of a group is central to abstract algebra. Its power lies in its simplicity and ubiquity; a vast array of mathematical and physical systems can be modeled by groups.

## Formal Definition of a Group

A **group** is an ordered pair $(G, \cdot)$, where $G$ is a non-empty set and $\cdot$ is a binary operation on $G$, satisfying the following four axioms:

### Group Axioms

1. **Closure**: For all $a, b \in G$, the result of the operation, $a \cdot b$, is also in $G$
2. **Associativity**: For all $a, b, c \in G$, the equation $(a \cdot b) \cdot c = a \cdot (b \cdot c)$ holds
3. **Identity Element**: There exists a unique element $e \in G$, called the identity element, such that for every element $a \in G$, the equation $e \cdot a = a \cdot e = a$ holds
4. **Inverse Element**: For each element $a \in G$, there exists an element $b \in G$, denoted $a^{-1}$, called the inverse of $a$, such that $a \cdot a^{-1} = a^{-1} \cdot a = e$

### Additional Properties

- If the group operation is also **commutative** (i.e., $a \cdot b = b \cdot a$ for all $a, b \in G$), the group is called an **abelian group** or a **commutative group**
- The number of elements in a group is called its **order**, denoted $|G|$
- If the order is finite, the group is a **finite group**

## Motivation: Symmetry

The group axioms are not an arbitrary collection of rules; rather, they are a precise formalization of the essential properties common to all systems of symmetry transformations.

Consider the set of symmetries of a geometric object:
- The composition of two symmetries is another symmetry (**Closure**)
- The composition of functions is inherently associative (**Associativity**)
- The transformation that does nothing is a symmetry (**Identity**)
- Any symmetry can be undone by reversing the transformation (**Inverse**)

Thus, the set of symmetries of any object forms a group, known as its **symmetry group**. This insight frames group theory as the abstract study of symmetry itself.

## Subgroups

Within a group, there often exist smaller groups.

### Definition

A **subgroup** $H$ of a group $G$ is a non-empty subset of $G$ that itself forms a group under the binary operation of $G$. This is denoted by $H \leq G$.

- If $H$ is a proper subset of $G$ ($H \neq G$), it is a **proper subgroup**, denoted $H < G$
- The subgroup $\{e\}$ consisting of only the identity element is the **trivial subgroup**

### Subgroup Tests

To verify that a non-empty subset $H \subseteq G$ is a subgroup, one can use the following tests:

#### Two-Step Test
$H$ is a subgroup if and only if:
1. It is closed under the group operation (for all $a, b \in H$, $ab \in H$)
2. It is closed under inverses (for all $a \in H$, $a^{-1} \in H$)

#### One-Step Test
$H$ is a subgroup if and only if for all $a, b \in H$, the element $ab^{-1}$ is also in $H$

#### Finite Subgroup Test
If $H$ is a finite, non-empty subset of $G$, it is a subgroup if and only if it is closed under the group operation.

## Key Examples

### Example 1: Dihedral Groups ($D_n$)

The dihedral groups are among the simplest and most important examples of finite, non-abelian groups. They are the symmetry groups of regular polygons.

#### Geometric Definition
The dihedral group $D_n$ is the group of symmetries of a regular $n$-gon. For $n \geq 3$, this group consists of:
- $n$ rotational symmetries
- $n$ reflectional symmetries

The order of $D_n$ is $2n$.

#### Algebraic Presentation
The structure of $D_n$ can be captured by two generators: a rotation $r$ and a reflection $s$. The group is defined by the relations these generators satisfy:

$$D_n = \langle r, s \mid r^n = s^2 = e, \text{ and } srs^{-1} = r^{-1} \rangle$$

The relation $srs^{-1} = r^{-1}$ (or equivalently, $sr = r^{-1}s$) algebraically encodes the geometric fact that reflecting a rotation is equivalent to rotating in the opposite direction.

#### Example: The Group $D_4$

The group $D_4$ represents the symmetries of a square and has order $2 \times 4 = 8$. Its elements are:

**Four rotations**: $\{e, r, r^2, r^3\}$, corresponding to rotations by $0°, 90°, 180°, 270°$ counterclockwise

**Four reflections**: $\{s, sr, sr^2, sr^3\}$, corresponding to reflections across the horizontal, main diagonal, vertical, and anti-diagonal axes, respectively

The group operation is function composition, which is not commutative. For example, a rotation by $90°$ followed by a horizontal flip $(sr)$ is not the same as a horizontal flip followed by a $90°$ rotation $(rs)$.

### Example 2: Permutation Groups ($S_n$)

Permutation groups are not just another class of examples; they are central to the entire theory of finite groups.

#### Definition
- A **permutation** of a set $M$ is a bijection from $M$ to itself
- The set of all permutations of $M$ forms a group under function composition, called the **symmetric group** on $M$, denoted $\text{Sym}(M)$
- If $M = \{1, 2, \ldots, n\}$, the group is denoted $S_n$ and is called the **symmetric group on $n$ letters**
- Its order is $|S_n| = n!$
- A **permutation group** is any subgroup of a symmetric group

#### Notation
Permutations are commonly written in **cycle notation**. A cycle $(a_1, a_2, \ldots, a_k)$ represents the permutation that sends $a_1 \to a_2$, $a_2 \to a_3$, ..., $a_k \to a_1$, and fixes all other elements.

Any permutation can be written as a product of disjoint cycles. For example, the permutation in $S_5$ that sends $1 \to 2$, $2 \to 5$, $5 \to 1$, $3 \to 4$, and $4 \to 3$ is written as $(1,2,5)(3,4)$.

#### Cayley's Theorem

**Theorem**: Every group is isomorphic to a subgroup of some symmetric group.

This theorem has profound implications. It establishes that every abstract group, no matter how it is defined (geometrically, through generators and relations, etc.), can be concretely realized as a group of permutations. This means that the study of permutation groups is, in a deep sense, the study of all groups.

## Examples of Subgroups

### Example 1: Subgroups of $(\mathbb{Z}, +)$
- The set of even integers $2\mathbb{Z} = \{0, \pm2, \pm4, \ldots\}$ is a subgroup
- For any $n \in \mathbb{N}$, the set $n\mathbb{Z} = \{0, \pm n, \pm 2n, \ldots\}$ is a subgroup

### Example 2: Subgroups of $D_4$
- The set of rotations $\{e, r, r^2, r^3\}$ is a subgroup
- The set $\{e, r^2\}$ is a subgroup (rotations by $0°$ and $180°$)
- The set $\{e, s\}$ is a subgroup (identity and horizontal reflection)

### Example 3: Subgroups of $S_3$
- The alternating group $A_3 = \{e, (1,2,3), (1,3,2)\}$ is a subgroup
- Any cyclic subgroup generated by a single element, e.g., $\langle (1,2) \rangle = \{e, (1,2)\}$

## Summary

Groups provide a unified framework for studying symmetry and algebraic structure. The concept of subgroups allows us to understand the internal structure of groups, while examples like dihedral and symmetric groups give concrete realizations of abstract group theory. Cayley's theorem shows that permutation groups are fundamental to understanding all finite groups. 