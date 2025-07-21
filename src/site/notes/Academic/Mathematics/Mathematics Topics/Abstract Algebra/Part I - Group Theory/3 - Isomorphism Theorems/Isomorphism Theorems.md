---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Mathematics Topics/Abstract Algebra/Part I - Group Theory/3 - Isomorphism Theorems/Isomorphism Theorems/"}
---


# Isomorphism Theorems and Composition Series

## Introduction

The isomorphism theorems are the fundamental tools for analyzing the structure of quotient groups and understanding the relationships between different groups. They function as the "conservation laws" of group theory, allowing us to relate subgroups, quotients, and homomorphisms in a precise way.

## Group Homomorphisms and Isomorphisms

### Definition

A **homomorphism** is a map $\phi: G \to H$ between two groups that preserves the group structure, meaning $\phi(g_1 g_2) = \phi(g_1) \phi(g_2)$ for all $g_1, g_2 \in G$.

### Important Sets Associated with Homomorphisms

Two important sets associated with a homomorphism are:

1. **Kernel**: $\ker(\phi) = \{g \in G \mid \phi(g) = e_H\}$, which is always a normal subgroup of $G$
2. **Image**: $\text{Im}(\phi) = \{\phi(g) \mid g \in G\}$, which is always a subgroup of $H$

### Isomorphisms

An **isomorphism** is a bijective homomorphism. If an isomorphism exists between two groups, they are said to be **isomorphic** (denoted $G \cong H$) and are considered structurally identical from an algebraic perspective.

## The Isomorphism Theorems

The three main isomorphism theorems, sometimes attributed to Emmy Noether, describe the fundamental relationships between quotient groups, normal subgroups, and homomorphisms.

### First Isomorphism Theorem

**Theorem 3.1 (First Isomorphism Theorem)**: Let $\phi: G \to H$ be a group homomorphism. Then the quotient group $G/\ker(\phi)$ is isomorphic to the image of $\phi$.

$$G/\ker(\phi) \cong \text{Im}(\phi)$$

This theorem is arguably the most important in group theory. It provides a direct link between homomorphisms and quotient groups, showing that factoring a group by the kernel of a map precisely captures the structure of the map's image.

#### Example
Consider the homomorphism $\phi: \mathbb{Z} \to \mathbb{Z}_6$ defined by $\phi(n) = n \bmod 6$. Then:
- $\ker(\phi) = 6\mathbb{Z}$
- $\text{Im}(\phi) = \mathbb{Z}_6$
- By the First Isomorphism Theorem: $\mathbb{Z}/6\mathbb{Z} \cong \mathbb{Z}_6$

### Second Isomorphism Theorem

**Theorem 3.2 (Second Isomorphism Theorem)**: Let $G$ be a group, $S$ a subgroup of $G$, and $N$ a normal subgroup of $G$. Then the product $SN = \{sn \mid s \in S, n \in N\}$ is a subgroup of $G$, the intersection $S \cap N$ is a normal subgroup of $S$, and the following isomorphism holds:

$$(SN)/N \cong S/(S \cap N)$$

This theorem is often called the "Diamond Isomorphism Theorem" due to the shape of the corresponding subgroup lattice diagram.

#### Example
Let $G = S_4$, $S = \langle (1,2,3) \rangle$ (cyclic subgroup of order 3), and $N = A_4$ (alternating group). Then:
- $SN = S_4$ (since $S_4 = A_4 \cup A_4(1,2,3)$)
- $S \cap N = \{e\}$
- By the Second Isomorphism Theorem: $S_4/A_4 \cong \langle (1,2,3) \rangle / \{e\} \cong \mathbb{Z}_3$

### Third Isomorphism Theorem

**Theorem 3.3 (Third Isomorphism Theorem)**: Let $G$ be a group and let $N$ and $K$ be normal subgroups of $G$ with $N \subseteq K$. Then $N$ is a normal subgroup of $K$, $K/N$ is a normal subgroup of $G/N$, and the following isomorphism holds:

$$(G/N)/(K/N) \cong G/K$$

This theorem provides a "cancellation" rule for quotients. It also establishes a one-to-one correspondence between the subgroups of $G/N$ and the subgroups of $G$ that contain $N$, known as the **Correspondence Theorem** or **Lattice Theorem**.

#### Example
Let $G = \mathbb{Z}$, $N = 12\mathbb{Z}$, and $K = 4\mathbb{Z}$. Then:
- $G/N = \mathbb{Z}/12\mathbb{Z}$
- $K/N = 4\mathbb{Z}/12\mathbb{Z} \cong \mathbb{Z}_3$
- $G/K = \mathbb{Z}/4\mathbb{Z}$
- By the Third Isomorphism Theorem: $(\mathbb{Z}/12\mathbb{Z})/(4\mathbb{Z}/12\mathbb{Z}) \cong \mathbb{Z}/4\mathbb{Z}$

## Composition Series and Simple Groups

The isomorphism theorems allow us to deconstruct groups. This process of decomposition leads to the idea of fundamental, indivisible building blocks.

### Simple Groups

**Definition 3.4**: A group $G$ is **simple** if its only normal subgroups are the trivial subgroup $\{e\}$ and the group $G$ itself.

Simple groups are the "atoms" of group theory. They cannot be simplified further by forming non-trivial quotient groups. Key examples include:
- The cyclic groups $\mathbb{Z}_p$ for a prime $p$
- The alternating groups $A_n$ for $n \geq 5$

### Subnormal Series

**Definition 3.5**: A **subnormal series** of a group $G$ is a finite sequence of subgroups:

$$\{e\} = H_0 \trianglelefteq H_1 \trianglelefteq \cdots \trianglelefteq H_n = G$$

where each $H_i$ is a normal subgroup of $H_{i+1}$. The quotient groups $H_{i+1}/H_i$ are called the **factors** of the series.

### Composition Series

A **composition series** is a subnormal series where all the factors $H_{i+1}/H_i$ are simple groups.

The existence of a composition series for every finite group can be shown by starting with $G$ and finding a maximal normal subgroup $H_{n-1}$; then finding a maximal normal subgroup of $H_{n-1}$, and so on, until the trivial group is reached. The maximality at each step ensures the corresponding factor group is simple.

### Analogy with Prime Factorization

This process is analogous to the prime factorization of an integer. An integer is factored into primes; a finite group is "factored" via a composition series into simple groups. This analogy provides the entire motivation for one of the monumental achievements of 20th-century mathematics: the classification of all finite simple groups.

Just as understanding prime numbers is key to number theory, understanding simple groups is key to understanding all finite groups.

## Examples

### Example 1: Composition Series of $\mathbb{Z}_{12}$

A composition series for $\mathbb{Z}_{12}$ is:
$$\{0\} \trianglelefteq \langle 6 \rangle \trianglelefteq \langle 2 \rangle \trianglelefteq \mathbb{Z}_{12}$$

The factors are:
- $\langle 6 \rangle / \{0\} \cong \mathbb{Z}_2$
- $\langle 2 \rangle / \langle 6 \rangle \cong \mathbb{Z}_3$
- $\mathbb{Z}_{12} / \langle 2 \rangle \cong \mathbb{Z}_2$

### Example 2: Composition Series of $S_4$

A composition series for $S_4$ is:
$$\{e\} \trianglelefteq V \trianglelefteq A_4 \trianglelefteq S_4$$

where $V = \{e, (1,2)(3,4), (1,3)(2,4), (1,4)(2,3)\}$ is the Klein four-group.

The factors are:
- $V / \{e\} \cong \mathbb{Z}_2 \times \mathbb{Z}_2$
- $A_4 / V \cong \mathbb{Z}_3$
- $S_4 / A_4 \cong \mathbb{Z}_2$

### Example 3: Using the First Isomorphism Theorem

Consider the homomorphism $\phi: \mathbb{R}^* \to \mathbb{R}^*$ defined by $\phi(x) = x^2$. Then:
- $\ker(\phi) = \{\pm 1\}$
- $\text{Im}(\phi) = \mathbb{R}^+$ (positive real numbers)
- By the First Isomorphism Theorem: $\mathbb{R}^* / \{\pm 1\} \cong \mathbb{R}^+$

## Applications

### Application 1: Understanding Group Structure

The isomorphism theorems help us understand the structure of groups by relating them to simpler groups through quotients and homomorphisms.

### Application 2: Proving Isomorphisms

The theorems provide powerful tools for proving that two groups are isomorphic without having to construct an explicit isomorphism.

### Application 3: Classification of Groups

Composition series and simple groups are fundamental to the classification of finite groups, which is one of the major achievements of 20th-century mathematics.

## Summary

The isomorphism theorems provide the fundamental tools for understanding group structure by relating homomorphisms, normal subgroups, and quotient groups. Composition series allow us to break down finite groups into simple building blocks, analogous to prime factorization of integers. These concepts are essential for the deeper study of group theory and its applications in Galois theory and other areas of mathematics. 