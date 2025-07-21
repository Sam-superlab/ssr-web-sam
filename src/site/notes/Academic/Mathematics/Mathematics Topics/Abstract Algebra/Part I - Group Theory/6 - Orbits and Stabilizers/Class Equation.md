---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Class Equation/"}
---


# Class Equation

## Introduction

The Class Equation is a powerful numerical tool that reveals deep information about the structure of finite groups. It arises from applying the Orbit-Stabilizer Theorem to the conjugation action of a group on itself.

## Definition

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

## Applications

### Application 1: p-Groups Have Non-trivial Centers

The Class Equation is a powerful numerical tool. Since each term $[G : C_G(y_j)]$ must divide $|G|$, it imposes strong constraints on the structure of a finite group.

A famous consequence is that any group whose order is a power of a prime $p$ (a **p-group**) must have a non-trivial center. This is because $|G|$ and each index $[G : C_G(y_j)]$ are powers of $p$, so for the equation to balance, $|Z(G)|$ must also be divisible by $p$.

### Application 2: Understanding Group Structure

The Class Equation helps us understand the internal structure of groups by revealing information about conjugacy classes and centralizers.

### Application 3: Proving Simplicity

The Class Equation can be used to prove that certain groups are simple by showing that they cannot have non-trivial normal subgroups.

### Application 4: Sylow Theorems

The Class Equation is fundamental in the proof of the Sylow theorems, particularly in establishing the existence of Sylow subgroups.

## Properties

### Divisibility Constraints
Each term $[G : C_G(y_j)]$ in the class equation must divide $|G|$, providing strong constraints on possible group structures.

### Center Size
The size of the center $|Z(G)|$ must be a divisor of $|G|$ and must be at least 1 (since the identity is always in the center).

### Abelian Groups
For abelian groups, all conjugacy classes have size 1, so the class equation becomes $|G| = |Z(G)| = |G|$.

## Related Concepts

- [[Conjugacy Classes\|Conjugacy Classes]]
- [[Centralizers\|Centralizers]]
- [[Center of a Group\|Center of a Group]]
- [[Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/6 - Orbits and Stabilizers/Orbit-Stabilizer Theorem\|Orbit-Stabilizer Theorem]]
- [[Sylow Theorems\|Sylow Theorems]] 