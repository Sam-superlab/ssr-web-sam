---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbits and Stabilizers/"}
---


# Orbits, Stabilizers, and the Class Equation

## Introduction

When a group acts on a set, it imposes a structure on that set, partitioning it into disjoint pieces. The study of these pieces provides a powerful counting tool that reveals deep information about the group itself.

## Orbits and Stabilizers

### Definitions

**Definition 6.1**: Let a group $G$ act on a set $X$.

- The **orbit** of an element $x \in X$ is the set of all elements in $X$ that $x$ can be moved to by the action of $G$. It is denoted $\text{Orb}_G(x)$ or $G \cdot x$:
  $$\text{Orb}_G(x) = \{g \cdot x \mid g \in G\}$$

- The **stabilizer** of an element $x \in X$ is the set of all elements in $G$ that fix $x$. It is a subgroup of $G$, denoted $\text{Stab}_G(x)$ or $G_x$:
  $$\text{Stab}_G(x) = \{g \in G \mid g \cdot x = x\}$$

### Key Properties

1. **Partition Property**: The orbits form a partition of the set $X$. This means that every element of $X$ belongs to exactly one orbit, and any two orbits are either identical or disjoint.

2. **Subgroup Property**: The stabilizer of any element is a subgroup of $G$.

3. **Relationship**: These two concepts are fundamentally linked by one of the most useful theorems in group theory.

## The Orbit-Stabilizer Theorem

**Theorem 6.2 (Orbit-Stabilizer Theorem)**: Let a finite group $G$ act on a set $X$. For any $x \in X$, the size of the orbit of $x$ is equal to the index of its stabilizer subgroup:

$$|\text{Orb}_G(x)| = \frac{|G|}{|\text{Stab}_G(x)|}$$

This theorem provides a powerful formula: $|G| = |\text{Orb}_G(x)| \cdot |\text{Stab}_G(x)|$.

### Proof Sketch

The proof uses the fact that there is a bijection between the orbit of $x$ and the set of left cosets of the stabilizer of $x$. Specifically, the map $g \cdot x \mapsto g\text{Stab}_G(x)$ is a well-defined bijection.

## The Class Equation

A particularly insightful application of the Orbit-Stabilizer Theorem arises when a group $G$ acts on itself by conjugation. The action is defined by $g \cdot x = gxg^{-1}$ for $g, x \in G$.

### Conjugacy Classes

- The orbit of an element $x$ under this action is its **conjugacy class**, denoted $\text{cl}(x) = \{gxg^{-1} \mid g \in G\}$.
- The stabilizer of $x$ is the set of elements that commute with $x$, known as the **centralizer** of $x$, denoted $C_G(x) = \{g \in G \mid gx = xg\}$.

### Applying the Orbit-Stabilizer Theorem

Applying the Orbit-Stabilizer Theorem to this action yields $|\text{cl}(x)| = [G : C_G(x)]$.

### Partitioning the Group

The set $G$ is partitioned by its conjugacy classes. We can separate the elements whose conjugacy class has size 1. These are the elements for which $gxg^{-1} = x$ for all $g \in G$, which is precisely the definition of the **center** of the group, $Z(G)$.

### The Class Equation

Summing the sizes of all the distinct conjugacy classes gives the order of the group:

$$|G| = \sum_{i=1}^{k} |\text{cl}(x_i)|$$

where $x_1, \ldots, x_k$ are representatives from each distinct conjugacy class. By separating the center, we arrive at the **Class Equation**:

$$|G| = |Z(G)| + \sum_{j=1}^{m} [G : C_G(y_j)]$$

where $y_1, \ldots, y_m$ are representatives from the distinct conjugacy classes of size greater than 1.

## Applications of the Class Equation

### Application 1: p-Groups Have Non-trivial Centers

The Class Equation is a powerful numerical tool. Since each term $[G : C_G(y_j)]$ must divide $|G|$, it imposes strong constraints on the structure of a finite group.

A famous consequence is that any group whose order is a power of a prime $p$ (a **p-group**) must have a non-trivial center. This is because $|G|$ and each index $[G : C_G(y_j)]$ are powers of $p$, so for the equation to balance, $|Z(G)|$ must also be divisible by $p$.

### Application 2: Understanding Group Structure

The Class Equation helps us understand the internal structure of groups by revealing information about conjugacy classes and centralizers.

### Application 3: Proving Simplicity

The Class Equation can be used to prove that certain groups are simple by showing that they cannot have non-trivial normal subgroups.

## Examples

### Example 1: Class Equation for $S_3$

Consider the symmetric group $S_3$ of order 6. The conjugacy classes are:
- $\{e\}$ (size 1)
- $\{(1,2), (1,3), (2,3)\}$ (size 3)
- $\{(1,2,3), (1,3,2)\}$ (size 2)

The center $Z(S_3) = \{e\}$, so the class equation is:
$$6 = 1 + 3 + 2$$

### Example 2: Class Equation for $D_4$

Consider the dihedral group $D_4$ of order 8. The conjugacy classes are:
- $\{e\}$ (size 1)
- $\{r^2\}$ (size 1)
- $\{r, r^3\}$ (size 2)
- $\{s, sr^2\}$ (size 2)
- $\{sr, sr^3\}$ (size 2)

The center $Z(D_4) = \{e, r^2\}$, so the class equation is:
$$8 = 2 + 2 + 2 + 2$$

### Example 3: p-Group Example

Consider a group $G$ of order $p^2$ where $p$ is prime. By the class equation, $|Z(G)|$ must be divisible by $p$. Since $Z(G) \leq G$, we have $|Z(G)| = p$ or $|Z(G)| = p^2$. If $|Z(G)| = p^2$, then $G$ is abelian. If $|Z(G)| = p$, then $G/Z(G)$ has order $p$ and is therefore cyclic, which implies that $G$ is abelian. Therefore, every group of order $p^2$ is abelian.

## Burnside's Lemma

Another important application of group actions is **Burnside's Lemma** (also known as the Cauchy-Frobenius Lemma), which counts the number of orbits.

### Statement

**Theorem 6.3 (Burnside's Lemma)**: Let a finite group $G$ act on a finite set $X$. The number of orbits is equal to the average number of fixed points:

$$\text{Number of orbits} = \frac{1}{|G|} \sum_{g \in G} |\text{Fix}(g)|$$

where $\text{Fix}(g) = \{x \in X \mid g \cdot x = x\}$ is the set of elements fixed by $g$.

### Applications

Burnside's Lemma is particularly useful in combinatorics for counting objects up to symmetry. For example, it can be used to count:
- The number of distinct colorings of a cube with $n$ colors
- The number of distinct necklaces with $n$ beads of different colors
- The number of distinct arrangements of objects under symmetry

## Examples of Burnside's Lemma

### Example 1: Counting Cube Colorings

How many distinct ways can we color the faces of a cube with 2 colors (red and blue)?

The group of symmetries of a cube has order 24. We need to count the fixed points of each symmetry:
- Identity: fixes all $2^6 = 64$ colorings
- Rotations by $90°$ about face axes: fix $2^3 = 8$ colorings each
- Rotations by $180°$ about face axes: fix $2^4 = 16$ colorings each
- Rotations by $120°$ about vertex axes: fix $2^2 = 4$ colorings each
- Rotations by $180°$ about edge axes: fix $2^3 = 8$ colorings each

By Burnside's Lemma:
$$\text{Number of orbits} = \frac{1}{24}(64 + 6 \cdot 8 + 3 \cdot 16 + 8 \cdot 4 + 6 \cdot 8) = \frac{1}{24}(64 + 48 + 48 + 32 + 48) = \frac{240}{24} = 10$$

So there are 10 distinct colorings.

## Summary

The study of orbits and stabilizers provides powerful tools for understanding group actions and their applications. The Orbit-Stabilizer Theorem relates the size of orbits to the index of stabilizers, while the Class Equation reveals the internal structure of groups through their conjugacy classes. Burnside's Lemma provides a method for counting objects up to symmetry.

These concepts are fundamental to group theory and have applications throughout mathematics, from combinatorics to geometry to number theory. 